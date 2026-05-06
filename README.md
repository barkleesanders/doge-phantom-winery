# The Phantom Winery — A Public-Record Investigation

> A complete public-record audit of Tim Mynett's eStCru LLC, Rose Lake Capital LLC, E Street Group LLC, and the West Pike Inc. successor entity — with their connections to Rep. Ilhan Omar's congressional disclosures, the $9 billion Minnesota Medicaid fraud, the Feeding Our Future $250M+ scheme, and the Ivanhoe Atlantic / Liberty Corridor mining deal in Guinea/Liberia.
>
> Eight rounds of investigation. Every fact verified. Every URL fetched. No FOIA filed. No subpoena required.

[![License: CC-BY-4.0](https://img.shields.io/badge/License-CC--BY--4.0-blue.svg)](LICENSE)
[![Investigation Status: Public Record](https://img.shields.io/badge/Status-Public%20Record-green.svg)](#)
[![Last Updated: 2026-05-06](https://img.shields.io/badge/Updated-2026--05--06-orange.svg)](#)

---

## 📰 The Magazine

The full investigation is published as a 30-spread editorial magazine.

| Format | File | Size |
|---|---|---|
| **Interactive HTML** | [`docs/magazine.html`](docs/magazine.html) | 106 KB |
| **PDF (print-ready)** | [`docs/doge-quarterly-vol-2-final.pdf`](docs/doge-quarterly-vol-2-final.pdf) | 2.5 MB |

**View the HTML magazine live via GitHub Pages:** https://barkleesanders.github.io/doge-phantom-winery/

Pages are served from the [`docs/`](docs/) folder. The `magazine.html` is the 30-spread interactive edition; the PDF is the print-ready archival copy.

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

4. **The Africa Personnel Overlap.** ⚠️ **CORRECTED 2026-05-06** (per Andrew Kerr / Washington Free Beacon): The previously published claim that "Rose Lake Capital's only known investment is Ivanhoe Atlantic" was an inference, not documented in primary records. **What IS documented:** Dr. J. Peter Pham simultaneously holds advisory standing at Rose Lake Capital (Sept 2025 Wayback) and a Director seat at HPX/Ivanhoe Atlantic (per [HPX SEC Form D filed 6/18/2024](archive/sec-form-d/hpx_form-d_2024-06-18.xml)). **What is NOT documented:** any equity link between Rose Lake and Ivanhoe Atlantic in any SEC, FARA, LDA, MIGA, UK Companies House, Jersey FSC, or DC corporate filing. What IS documented separately: Ivanhoe Atlantic operates a $1.8B iron ore rail project in Guinea and Liberia; Omar served as Vice Chair of the House Foreign Affairs Subcommittee on Africa with direct jurisdiction over those exact two countries; Ivanhoe Mines (parent) is **40% owned by Chinese-state-linked entities (CITIC + Zijin)** per Rep. Moolenaar's December 9, 2025 letter to Secretary Rubio. Full correction memo: [`evidence/2026-05-followup-kerr/CORRECTION_AND_NEW_FINDINGS.md`](evidence/2026-05-followup-kerr/CORRECTION_AND_NEW_FINDINGS.md).

5. **The Multi-Hatted Pham — primary-source documented (May 6, 2026 update).** Dr. J. Peter Pham simultaneously holds: (a) **Director, High Power Exploration Inc.** (Friedland-controlled mining parent) per [SEC Form D filed June 18, 2024](archive/sec-hpx/hpx_form-d_2024-06-18.xml); (b) **Executive Chairman AND Interim CEO, Ivanhoe Atlantic Inc.** per [Ivanhoe Atlantic's own press release of March 23, 2026](archive/ivanhoe-atlantic/board-appointments-press-release_2026-03-23.html); (c) **Director, SMFG Guinea** per the same press release; (d) **Advisor, Rose Lake Capital Inc.** per [Wayback team page Oct 29, 2024](https://web.archive.org/web/20241029092132/https://www.roselakecap.com/team). He published an op-ed in the Liberian Daily Observer on December 9, 2024 publicly pressuring Liberia to ratify the rail deal — while holding all four roles. The "Rose Lake invested in Ivanhoe Atlantic" frame turns out to be the wrong question: the dispositive linkage is one individual personally bridging Rose Lake's advisory bench AND HPX's parent board AND Ivanhoe Atlantic's operating leadership AND SMFG Guinea's board. Full memo: [`evidence/2026-05-followup-kerr/PHAM_DUAL_HAT.md`](evidence/2026-05-followup-kerr/PHAM_DUAL_HAT.md).

8. **The Three-Ambassador SMFG Board.** Per Ivanhoe Atlantic's [March 23, 2026 press release](archive/ivanhoe-atlantic/board-appointments-press-release_2026-03-23.html), the Guinea concession-holder's board now includes **three retired U.S. Ambassadors with Africa portfolios**: Amb. (Ret.) Patricia Moller (former Amb to Burundi 2006-09 + Guinea 2010-12; SMFG Chair since 2019); Amb. (Ret.) J. Peter Pham (former Special Envoy Great Lakes/Sahel); and Amb. (Ret.) Tibor P. Nagy, Jr. (former Amb to Guinea + Ethiopia; former Asst Secretary of State for Africa under Trump-1). Plus Bradley Doig (I-Pulse COO) and Kevin McLean (Ivanhoe Atlantic COO).

9. **HPX Operational Seat → London; Friedland Off the HPX Board.** Per the [June 18, 2024 Form D](archive/sec-hpx/hpx_form-d_2024-06-18.xml), HPX's issuer address is now "c/o HPX Mines (UK) Limited, 15/16 Pembroke Mews, London W8 6ER" — the operational seat has moved from Vancouver to London. The board no longer includes Friedland; current directors are On Yip Patrick Tsang (Tsangs Group HK family office Chairman), Kenneth Lau, David Bohem, Doig Bradley (I-Pulse COO), Bronwyn Barnes (Executive Officer), Robin Sandenburgh, and J. Peter Pham. Reg D 506(b) round: $324.5M total offering, $193M sold to 14 accredited investors as of June 18, 2024.

10. **Lobbying Footprint Cleanly Mapped (Negative Confirmations).** Sweep of all 7 pages of Brownstein Hyatt Farber Schreck's 2024 LD-203 filings (1,777 contribution line items) returned **zero hits** for ILHAN, OMAR, MYNETT, HAILER, PHAM, CARL-YODER, DIEKMAN, MADDOX. Yorktown Solutions (Vajdich) similarly reported zero contributions on every 2024+2025 LD-203 — a cleanly suspicious negative for a partner-level Hill influencer billing $120K/quarter. See [`BHFS_LD203_NEGATIVE.md`](evidence/2026-05-followup-kerr/BHFS_LD203_NEGATIVE.md).

11. **Bethel Cleared (Removes One Revolving-Door Theory).** MIGA Board approved the $123.3M Nimba political-risk guarantee on **February 18, 2021**; issued March 12, 2021. Erik Bethel served as US Alt. Exec. Director only 2018-2020 (he was nominated as Ambassador to Panama in April 2020). He was NOT on the Board for the Feb 2021 vote. Memo: [`MIGA_BOARD_APPROVAL_TIMING.md`](evidence/2026-05-followup-kerr/MIGA_BOARD_APPROVAL_TIMING.md).

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

This repository is a **living snapshot** of public-record evidence. Last comprehensive line-by-line audit: **May 6, 2026** (post-Kerr correction round, see [`evidence/2026-05-followup-kerr/`](evidence/2026-05-followup-kerr/)).

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
**Last Audit:** May 6, 2026 — line-by-line claim review post-Kerr correction
**Investigators:** DOGE Service (8 rounds of public-record audit + 1 correction round)
**Repository:** This file is the entry point. Everything else is downstream of the receipts.
