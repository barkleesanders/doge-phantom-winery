# The Phantom Winery — A Public-Record Investigation

> A complete public-record audit of Tim Mynett's eStCru LLC, Rose Lake Capital LLC, E Street Group LLC, and the West Pike Inc. successor entity — with their connections to Rep. Ilhan Omar's congressional disclosures, the $9 billion Minnesota Medicaid fraud, the Feeding Our Future $250M+ scheme, and the Ivanhoe Atlantic / Liberty Corridor mining deal in Guinea/Liberia.
>
> Eight rounds of investigation. Every fact verified. Every URL fetched. No FOIA filed. No subpoena required.

[![License: CC-BY-4.0](https://img.shields.io/badge/License-CC--BY--4.0-blue.svg)](LICENSE)
[![Investigation Status: Public Record](https://img.shields.io/badge/Status-Public%20Record-green.svg)](#)
[![Last Updated: 2026-04-25](https://img.shields.io/badge/Updated-2026--04--25-orange.svg)](#)

---

## 📰 The Magazine

The full investigation is published as a 30-spread editorial magazine.

| Format | File | Size |
|---|---|---|
| **Interactive HTML** | [`docs/magazine.html`](docs/magazine.html) | 106 KB |
| **PDF (print-ready)** | [`docs/doge-quarterly-vol-2-final.pdf`](docs/doge-quarterly-vol-2-final.pdf) | 2.5 MB |

**View the HTML directly via GitHub Pages:** *(enable Pages on this repo to publish)*

## 📂 Repository Contents

```
doge-phantom-winery/
├── README.md                          # You are here
├── LICENSE                            # CC-BY-4.0 (analysis), MIT (skill code)
├── docs/
│   ├── magazine.html                  # 30-spread interactive magazine
│   └── doge-quarterly-vol-2-final.pdf # Print-ready PDF
├── evidence/
│   ├── SOURCES.md                     # Every URL with annotation
│   ├── EVIDENCE.md                    # Key facts mapped to sources
│   ├── TIMELINE.md                    # Chronological events 2018-2026
│   ├── DEFENDANT_ROSTER.md            # 56 named FOF defendants
│   ├── LEGAL_BRIEF.md                 # Statute-by-statute exposure
│   ├── NETWORK.md                     # The full connection map
│   └── FEC_CROSS_REFERENCE.md         # FOF ↔ Omar donor cross-reference results
└── skill/
    ├── SKILL.md                       # The /doge-service Claude Code skill
    ├── prompts/                       # Skill prompt templates
    └── references/                    # Skill reference material
```

## 🎯 The Headline Findings

1. **The Phantom Winery.** eStCru LLC — Tim Mynett's "California winery" — has its registered principal office at a **$10.99/month Postal Plus virtual mailbox** (422 Larkfield Center #400, Santa Rosa, CA 95403). Same address West Pike Inc. (the successor entity) uses today.

2. **The Sworn Filing vs. Walk-Back Fork.** Omar certified eStCru LLC + Rose Lake Capital LLC at a combined value of up to **$30 million** on her 2024 House Clerk Financial Disclosure (filed May 14, 2025, under penalty of perjury). On April 23, 2026 she told the New York Post the actual value is *"less than $100,000."* Either statement creates federal criminal exposure under 18 USC §1001.

3. **SEC EDGAR Returns Zero Hits.** Direct API queries against `efts.sec.gov` for "Rose Lake Capital", "eStCru", "E Street Group", "Timothy Mynett", "William Hailer", "EstVenture", and "West Pike Inc" all returned **zero matching filings**. Yet Rose Lake's website previously claimed *"$60 billion AUM"* and its Terms-of-Service admits *"All investment offerings are done within exemptions allowed under the SEC."*

4. **The Africa Conflict of Interest.** Rose Lake Capital's only known investment is **Ivanhoe Atlantic** — a $1.8 billion iron ore rail project in Guinea and Liberia. Omar served as Vice Chair of the House Foreign Affairs Subcommittee on Africa (which has direct jurisdiction over those exact two countries). The mining project's parent (Ivanhoe Mines) is **40% owned by Chinese-state-linked entities (CITIC + Zijin)** per a December 9, 2025 letter from Rep. John Moolenaar (Chair, House Select Committee on the CCP) to Secretary of State Rubio.

5. **The Quadruple-Hatted Advisor.** Dr. J. Peter Pham — listed on Rose Lake's Wayback team page — simultaneously serves as Chairman of HPX (Ivanhoe Atlantic's parent), Non-Executive Chairman of Ivanhoe Atlantic itself, advisor to Trump's Africa portfolio, and (per the Wayback snapshot) Rose Lake Capital advisor. He published an op-ed in the Liberian Daily Observer on December 9, 2024 publicly pressuring Liberia to ratify the rail deal — while holding all four hats.

6. **The MN Fraud Connection.** The Comer letter to Mynett opens: *"The Committee on Oversight and Government Reform is investigating widespread fraud in Minnesota's social services programs."* The $9 billion Minnesota Medicaid fraud (90%+ of charged defendants of Somali descent) traces to a COVID-era food bill **Omar sponsored** (HR 6187, MEALS Act), with proceeds laundered to **Kenya, UAE/Dubai, Istanbul, London**. Three of those four destinations match Comer's specific Item #4 in his letter to Mynett (UAE, Somalia, Kenya travel records).

7. **The FEC Cross-Reference Came Back Clean.** Direct FEC API queries against Omar's committee C00680934 (Ilhan for Congress) for **18 known FOF defendant surnames** returned **zero direct matches**. Money flow theory — if any — must route through Mynett's LLCs (which is exactly where Comer subpoenaed). Omar has only one campaign committee — no leadership PAC, no JFC.

## 📚 How To Use This Repo

**For journalists:**
- Read [`evidence/EVIDENCE.md`](evidence/EVIDENCE.md) for the fact-by-fact chain with citations
- Read [`evidence/TIMELINE.md`](evidence/TIMELINE.md) for chronology
- Use [`evidence/SOURCES.md`](evidence/SOURCES.md) to verify every claim independently

**For legal analysts:**
- Read [`evidence/LEGAL_BRIEF.md`](evidence/LEGAL_BRIEF.md) for the statute-by-statute exposure
- Comparable convictions are cited inline with case names + sentencing

**For investigators:**
- Read [`evidence/NETWORK.md`](evidence/NETWORK.md) for the full connection map
- Read [`evidence/DEFENDANT_ROSTER.md`](evidence/DEFENDANT_ROSTER.md) for the 56 named FOF defendants
- Read [`evidence/FEC_CROSS_REFERENCE.md`](evidence/FEC_CROSS_REFERENCE.md) for the donor cross-reference methodology + results

**For developers / fellow agents:**
- The [`skill/`](skill/) directory contains the reusable Claude Code skill (`/doge-service`) that powered this investigation
- Drop into `~/.claude/skills/doge-service/` to install
- Six-phase method, sitemap-intelligence layer, recategorization layer, hard rules against fabrication

## ⚖️ Legal Notice

**This is opinion, commentary, and analysis on matters of public concern regarding public figures.** All factual claims are based on publicly available sources including:

- Congressional disclosures filed with the Clerk of the U.S. House of Representatives
- Federal Election Commission API and bulk data
- SEC EDGAR full-text API
- California Secretary of State business records
- Federal court filings via DocumentCloud and DOJ press releases
- House Oversight Committee letters and reports
- Minnesota Office of the Legislative Auditor reports
- News reporting from CBS, NY Post, Washington Examiner, Minnesota Reformer, Liberian Observer, and others

**Where allegations are discussed, they represent claims made by third parties (lawsuits, congressional letters, news reports) and do not constitute assertions of guilt or wrongdoing by the maintainers of this repository.** All individuals referenced are presumed innocent unless and until proven otherwise in a court of law.

The connections drawn between dots are circumstantial unless explicitly stated otherwise. Where the public record contains contradictions (e.g., the May 2025 sworn filing vs. April 2026 walk-back), both sides are presented with citations.

## 🔬 Methodology

This investigation followed the **`/doge-service` skill methodology** included in [`skill/SKILL.md`](skill/SKILL.md):

1. **SOURCE** — Pull every relevant code, regulation, public filing
2. **MAP** — Identify every agency / commission / oversight body with authority
3. **RECEIPTS** — Find under-utilized enforcement hooks
4. **CONFRONT** — Cross-reference statute language against evidence
5. **DEMAND** — Single deliverable with cited violations + relief
6. **INNOVATE** — Public dashboards, recurring monitoring, citizen oversight

**Hard rules applied throughout:**
- ✓ Never fabricate citations
- ✓ Never substitute "go to the website" for an exact URL
- ✓ Always cite source URL for every regulation, code, form
- ✓ Always note legal/procedural risk
- ✓ Never advise illegal action

Tools used:
- **Exa MCP server** for semantic search + page crawling
- **SEC EDGAR full-text API** (efts.sec.gov)
- **FEC OpenAPI** (api.open.fec.gov)
- **Wayback Machine CDX API** (web.archive.org/cdx)
- **Direct curl** against domain endpoints for live status checks
- **Chrome headless** for PDF rendering
- **Claude Code (Opus 4.7)** as the orchestration layer

## 🤝 Contributing

This repository is a **frozen snapshot** of public-record evidence as of **April 25, 2026**.

Issues and pull requests welcome for:
- Broken links (URL rot is real)
- Newly surfaced public-record evidence
- Corrections to misstated facts
- Additional verified comparable convictions

Out of scope:
- Speculation beyond what the public record supports
- Fabricated citations or unverified claims
- Personal attacks on named individuals

## 📜 License

- **Analysis text** (READMEs, evidence files, magazine content): [Creative Commons Attribution 4.0](LICENSE) — share and adapt with credit
- **Skill code** (`skill/SKILL.md` and supporting files): MIT License — free to copy, modify, and redistribute

## 🔗 The Mantra

*"Every agency has a statute. Every statute has a deadline. Every deadline is a lever. Find the receipts."*

— DOGE Service skill, `~/.claude/skills/doge-service/SKILL.md`

---

**Compiled:** April 25, 2026
**Investigators:** DOGE Service (8 rounds of public-record audit)
**Repository:** This file is the entry point. Everything else is downstream of the receipts.
