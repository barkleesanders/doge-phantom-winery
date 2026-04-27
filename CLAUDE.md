# Project Instructions for AI Agents

This file provides instructions and context for AI coding agents working on this project.

<!-- BEGIN BEADS INTEGRATION v:1 profile:minimal hash:ca08a54f -->
## Beads Issue Tracker

This project uses **bd (beads)** for issue tracking. Run `bd prime` to see full workflow context and commands.

### Quick Reference

```bash
bd ready              # Find available work
bd show <id>          # View issue details
bd update <id> --claim  # Claim work
bd close <id>         # Complete work
```

### Rules

- Use `bd` for ALL task tracking — do NOT use TodoWrite, TaskCreate, or markdown TODO lists
- Run `bd prime` for detailed command reference and session close protocol
- Use `bd remember` for persistent knowledge — do NOT use MEMORY.md files

## Session Completion

**When ending a work session**, you MUST complete ALL steps below. Work is NOT complete until `git push` succeeds.

**MANDATORY WORKFLOW:**

1. **File issues for remaining work** - Create issues for anything that needs follow-up
2. **Run quality gates** (if code changed) - Tests, linters, builds
3. **Update issue status** - Close finished work, update in-progress items
4. **PUSH TO REMOTE** - This is MANDATORY:
   ```bash
   git pull --rebase
   bd dolt push
   git push
   git status  # MUST show "up to date with origin"
   ```
5. **Clean up** - Clear stashes, prune remote branches
6. **Verify** - All changes committed AND pushed
7. **Hand off** - Provide context for next session

**CRITICAL RULES:**
- Work is NOT complete until `git push` succeeds
- NEVER stop before pushing - that leaves work stranded locally
- NEVER say "ready to push when you are" - YOU must push
- If push fails, resolve and retry until it succeeds
<!-- END BEADS INTEGRATION -->


## Build & Test

_Add your build and test commands here_

```bash
# Example:
# npm install
# npm test
```

## Architecture Overview

GitHub Pages publishes from **`/docs` only** (configured at repo level, source: `main` branch, path: `/docs`). The repo root holds `archive/`, `evidence/`, `submissions/`, `skill/` — these are NOT served by Pages.

- Live URL: `https://barkleesanders.github.io/doge-phantom-winery/` → maps to `/docs/`
- `archive/` (105 cached source pages, screenshots, PDFs) lives at repo root for git history clarity, NOT under `/docs/`
- Anything in `docs/*.html` that needs to reference `archive/` MUST link to the GitHub repo URL, not a relative path

## Conventions & Patterns

### Linking to archive/ from docs/ HTML (MANDATORY)

**NEVER use `../archive/...` relative paths from inside `docs/*.html`.** They 404 on the live Pages site because Pages doesn't see anything outside `/docs/`. This bit us once — fix in commit cd9af26 rewrote 79 broken links.

Use GitHub repo URLs instead:

| Target | URL pattern |
|--------|-------------|
| File (PDF, HTML, JSON, MD) | `https://github.com/barkleesanders/doge-phantom-winery/blob/main/archive/<path>` |
| Folder | `https://github.com/barkleesanders/doge-phantom-winery/tree/main/archive/<path>` |

PDFs render inline on github.com, HTML shows source, folders show file listing — all fine for "sourced links" UX.

### Pre-push verification for docs/

Before pushing changes to `docs/*.html`, run:

```bash
# Should return 0 — any hit is a future 404
grep -c '"\.\./archive/' docs/*.html
```

If you add a NEW directory at repo root that needs to be linked from `docs/`, either (a) move it under `docs/`, or (b) link via the GitHub repo URL pattern above. Don't reach across the `/docs/` boundary with `../`.

### archive/INDEX.md and MANIFEST.json (MANDATORY)

`archive/INDEX.md` lives at `archive/INDEX.md`. **Local-archive cells in INDEX.md MUST use full GitHub blob URLs**, not relative paths like `archive/court/X.pdf`. A relative `archive/...` from inside `archive/INDEX.md` resolves to `archive/archive/...` on github.com → 404. This bit us in commit 14d78f0.

URL patterns for INDEX rows:

| Cell | Pattern |
|------|---------|
| Local archive | `https://github.com/barkleesanders/doge-phantom-winery/blob/main/archive/<category>/<file>` |
| Wayback snapshot | `https://web.archive.org/web/*/<url>` (search redirect — finds latest snapshot or shows search) |

**Never use** `https://web.archive.org/web/2026*/<url>` — the `2026*` wildcard opens an empty calendar view, not a snapshot. Use `web/*/` instead, or query `https://archive.org/wayback/available?url=<url>` for the real timestamp.

### Archive completeness honesty (MANDATORY)

Every entry in `MANIFEST.json` has an `archive_status`:

- ✅ full HTML / full PDF / JSON / PNG — real backup
- 📝 note only — markdown summary because upstream blocked capture (Akamai/etc)
- 🤖 bot-blocked — captured response is the bot challenge page, not real content (sub-1KB Incapsula stub)
- 🔒 login-walled — LinkedIn / paywalled, can't archive without auth
- 🔧 asset CDN — fonts / non-source assets
- ❌ no archive — listed but never fetched

**Rule:** if a fetch returns <800 bytes for HTML, contains `_Incapsula_Resource`, or is a CDN response, status MUST be set to the appropriate non-✅ value. Never claim "full backup" for a stub.

To regenerate INDEX.md after manifest changes, use the regenerator pattern in commit 14d78f0 (was at `/tmp/regen-index.py` during fix; promote to `tools/regen-archive-index.py` if reused).
