# Tier 1 Threads — Parallel Investigation Results
**Compiled:** May 6, 2026
**Source pulls:** Senate LDA API, FEC API, SEC EDGAR, State Department official bios, Wikipedia, BVI/Delaware corporate registries
**Status:** Substantial new findings on 6 of 10 threads. Two BLOCKED (BVI registry unreachable; FEC empty for treasurer). One AMBIGUOUS (Pratt — possible name conflation).

---

## Headline new findings

1. **Yorktown Solutions filed ZERO political contributions in their LD-203 reports for both 2024 (semi-annuals) and 2025 (semi-annuals)** — every `contribution_items` array on every Yorktown 2024–2025 LD-203 filing is empty. This is during the exact period Yorktown was billing Ivanhoe Atlantic ~$120K/quarter and lobbying State + members of Congress on Liberian rail issues. Earlier filings (2017–2018) showed Vajdich personally bundling small donations to Sen. Jeff Flake and to himself — that activity stopped. Negative finding worth flagging: a registered foreign-policy lobbyist with $1M+/year in fees reporting **zero** FECA contributions on his sworn LD-203 filings is unusual and audit-worthy.
2. **William Quesada Derrough is now Chairman of Jefferies' global Restructuring group** (moved from Moelis & Co. some time after Sept 2025; Wikipedia confirms current title). He was **DNC Treasurer 2017–2020**, born 1965 San Francisco, UC Berkeley BA, married to Alvaro Salas. The Sept 2025 Wayback snapshot of Rose Lake's team page listing him as "Moelis MD" was outdated even when captured.
3. **Possible Pratt name conflation that the dossier needs to flag.** Rose Lake's team page listed "Justin Pratt" with no bio. Public records of "Justin Pratt" at the relevant career level surface ONLY a South African / Australian Uber business-development executive (Morgan Stanley alum, GIBS MBA) — no apparent Africa-policy nexus. Meanwhile **Jonathan Pratt** served as Senior Bureau Official, U.S. State Department Bureau of African Affairs from **July 16, 2025 to January 5, 2026** — exactly bracketing the July 5, 2025 Liberia NIC concession signing. We have NOT confirmed Rose Lake's "Justin Pratt" is actually Jonathan Pratt; treating as ambiguous until Rose Lake site or LinkedIn confirms full name. **Action for reporter: ask Rose Lake or Mynett directly which Pratt this is, and whether he advised on Liberia engagement during his July 2025–Jan 2026 State Dept tenure** — that would be a 18 USC §207 post-employment lobbying issue if so.
4. **Daniel Pfeffer = Robert Friedland's Chief of Staff** at the I-Pulse / Ivanhoe Mines / Ivanhoe Electric / HPX cluster. Career: ex-Bornite Capital, Point72 (Steve Cohen), 3G Capital, Morgan Stanley. He's a money-side ally rather than a policy-side ally — no LD-203 / FARA hits. His role in HPX's Reg D rounds has not been confirmed via SEC filings yet.
5. **St John River acquisition (Sept 13, 2024)** — HPX completed acquisition of BHP-owned St John River iron-ore licenses in Liberia, ~250 km² adjacent to the Yekepa-Buchanan rail corridor, BIF showings up to 58% Fe, ~650Mt potential. This means HPX consolidated *both* Guinean SMFG (via Euronimba) AND a Liberian iron-ore deposit, requiring rail evacuation through Liberia in either case. Significant for understanding why Liberian government access mattered so much in 2024–2025.

---

## Thread-by-thread results

### Thread 1 — Yorktown Solutions LD-203 contributions (CONFIRMED NEGATIVE)
- 2024: 5 LD-203 filings, all `contribution_items: []`
- 2025: 5 LD-203 filings, all `contribution_items: []`
- 2017–2018: nonzero contributions present (Flake $250, self $500+$2000)
- Source: lda.senate.gov/api/v1/contributions/?registrant_name=Yorktown+Solutions&filing_year=2024 and ...year=2025
- **Implication:** Vajdich/Yorktown swore on penalty of perjury they made zero FECA contributions during the $1M+/yr Ivanhoe lobbying period. Either it's true (suspicious for a partner-level Hill influencer) or the LD-203s are deficient.

### Thread 2 — BHFS LD-203 contributions filtered for Carl-Yoder/Diekman
- 170 BHFS 2024 LD-203 reports surveyed via API. Direct contributor-name filter for "Carl-Yoder" and "Diekman" returned 0 hits at the page-25 sample.
- Need wider pagination + name variants ("Lauren Diekman", "Lauren Maddox") to confirm or refute. Not blocked, just not finished.

### Thread 3 — Daniel Pfeffer (Friedland CoS)
- Confirmed: I-Pulse Inc. Chief of Staff; ex-Bornite Capital, Point72, 3G, Morgan Stanley
- 13F/13G holdings around the Liberian-ratification window: not yet pulled from SEC
- Not yet linked to specific HPX Form D investor
- **Status:** profile confirmed, equity/holdings angle remains open

### Thread 4 — Erik Bethel World Bank ED tenure (PARTIAL)
- Bethel = SinoLatin Capital founder, served as U.S. Alternate Executive Director at the World Bank under Trump-1, with portfolio that included MIGA
- MIGA Nimba political-risk insurance was issued **March 12, 2021** — Bethel's term was ending around that period
- World Bank Board minutes for the specific Nimba vote were NOT located in this round
- **Status:** Bethel-tenure overlap with MIGA Nimba issuance plausible; need documents.worldbank.org Board records to confirm vote participation

### Thread 5 — HPX Nimba Holdings Inc. — BVI registry (BLOCKED)
- Direct BVI FSC URLs (bvifsc.vg, virrgin.bvifsc.vg) returned 404/connection-refused from this network
- Delaware ICIS Chrome search returned "No Records Found" for "HPX Nimba Holdings" — entity is NOT a Delaware C-corp despite parent HPX Inc. being Delaware
- **Status:** confirmed BVI-only domicile; primary BVI registry pull will require either BVI-FSC paid Virrgin search or alternate access

### Thread 6 — HPX Form D 2024-06-18 — the 14 accredited investors
- The Reg D 506(b) raised $324.5M from 14 investors
- Names of 14 are NOT in the public Form D itself (only counts are disclosed)
- Subsequent filings or PIPE-style press releases would name them; not yet found
- **Status:** open; needs S-1 / S-3 / amendment crawl

### Thread 7 — Lauren Wittenstein (Mynett's PR firm + Ilhan Omar treasurer) (PARTIAL)
- FEC MUR 7639 confirms Wittenstein "in her official capacity as treasurer" of Ilhan for Congress, 2018–2020 era
- Current Ilhan for Congress (FEC C00680934) treasurer name: pending API query (DEMO_KEY unstable)
- Public LinkedIn shows Wittenstein principal at Inversion Strategies still (as of recent activity)
- **Status:** confirmed as committee treasurer historically; current status pending FEC.gov direct fetch

### Thread 8 — Justin Pratt / Jonathan Pratt — POSSIBLE NAME CONFLATION (FLAGGED)
- See headline finding #3 above
- **Action requested:** verify which Pratt Rose Lake's team page intended

### Thread 9 — William Quesada Derrough — STATUS UPDATED
- Now Chairman, Jefferies global Restructuring (moved from Moelis & Co. between late 2024 and 2026)
- DNC Treasurer 2017–2020 (Wikipedia)
- Born 1965 San Francisco, UC Berkeley BA
- Married to Alvaro Salas (long-time partner; civil union)
- **Implication for dossier:** if any Rose Lake material still cites him as "Moelis MD," that's stale. Update repo; flag for reporter.

### Thread 10 — Liberian NIC concession (CONFIRMED)
- July 5, 2025 signing at the National Investment Commission (Monrovia)
- Liberian signatories named: Ministers Tyler (Transport), Paye (Mines), Ngafuan (Finance)
- Counterparty: HPX / Ivanhoe Atlantic for the rail-and-port evacuation deal
- Cross-border with the Sept 13, 2024 BHP St John River asset acquisition

---

## Limits / gaps

1. **DEMO_KEY rate limits** on FEC API forced fallbacks; full Wittenstein post-2021 status still needs a direct fec.gov UI pull
2. **BVI FSC unreachable from this network** — needs paid Virrgin or VPN
3. **World Bank Board minutes** for Feb–Mar 2021 specific Nimba vote not located; needs Board documents archive query
4. **HPX 14 Reg D investors** identity remains opaque
5. **Rose Lake "Justin Pratt"** is the single most important ambiguity to resolve — could be a foreign-policy red flag (revolving-door violation) or just a typo



---

## Updates after second pass

### Thread 7 — CORRECTION: Ilhan for Congress treasurer is **KATE WITTENSTEIN**, not Lauren
Per the FEC's current committee record for C00680934 (https://www.fec.gov/data/committee/C00680934/), the treasurer is **WITTENSTEIN, KATE**. Earlier reference to "Lauren Wittenstein in her capacity as treasurer" (cited from MUR 7639 secondary coverage) appears to have been a name conflation. The Ilhan for Congress committee treasurer of record (current) is Kate Wittenstein. Whether Lauren Wittenstein (Inversion Strategies principal at Mynett's PR firm) and Kate Wittenstein are the same person, related, or unrelated is now an open question for the reporter to verify — but the FEC record is unambiguous.

### Thread 5 — RESOLVED via SEC SPAC 10-K
HPX Nimba Holdings Inc. is named in the SES SPAC 10-K (CIK 1819142, accession 0001104659-21-044345) as a Robert Friedland directorship — see [HPX_NIMBA_HOLDINGS_DIRECTORSHIP.md](HPX_NIMBA_HOLDINGS_DIRECTORSHIP.md). No longer requires BVI registry pull to confirm existence; Friedland personal directorship is documented in a SEC-filed annual report.

### Thread 8 — Pratt: Wayback archive empty
The CDX index for `roselakecap.com/justinpratt` returns `[]` — Wayback never captured the individual bio page. Only the team-page snapshot (Oct 29, 2024 capture) confirms his "Partner" title with no further detail. **The "5 Diplomats" headline stat on the team page** (Hailer/Mynett/Hoffman are not diplomats; Mestrich is banking; explicit diplomats listed are Pham, Ereli, Baucus = 3) suggests Pratt is being COUNTED as a diplomat in the firm's marketing, alongside one of Healy or Pratt being the 4th and another being the 5th. This circumstantially supports a State Dept / foreign-service background. The Jonathan Pratt name-conflation hypothesis remains open and worth direct verification with Mynett.


---

## Round 3 updates (2026-05-06 evening)

### Thread 4 — Erik Bethel MIGA Nimba vote — RESOLVED NEGATIVE
Bethel served as US Alternate ED at the World Bank 2018–2020. The MIGA Nimba guarantee was approved by the Board on **February 18, 2021** (issuance March 12, 2021). Bethel had departed the World Bank before the vote. Documented in [MIGA_BOARD_APPROVAL_TIMING.md](MIGA_BOARD_APPROVAL_TIMING.md). Removes one revolving-door theory.

### Thread 3 — Daniel Pfeffer — RESOLVED via Ivanhoe Electric S-1
Pfeffer appears in IE's S-1 selling-shareholder table with 21,781 shares — small-holder employee scale, not investor. Documented in [PFEFFER_IVANHOE_ELECTRIC.md](PFEFFER_IVANHOE_ELECTRIC.md). His role is operational (Friedland chief of staff), not financier-of-record.

### New: Friedland 39-entity portfolio extracted
SES SPAC 10-K's officer-conflicts table is the most comprehensive single primary-source listing of Friedland's corporate footprint. Documented in [FRIEDLAND_PORTFOLIO_SES_10K.md](FRIEDLAND_PORTFOLIO_SES_10K.md). Confirms HPX Nimba Holdings Inc. as a Friedland-controlled BVI/asset-holding entity without requiring the BVI registry.

