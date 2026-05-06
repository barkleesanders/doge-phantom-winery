# Reply to Andrew Kerr (Washington Free Beacon)

**To:** kerr@freebeacon.com
**From:** Barklee Sanders <barkleesanders@gmail.com>
**Subject:** Re: Rose Lake / Ivanhoe Atlantic — sourcing question
**Status:** Draft — review before send

---

Hi Andrew,

Thanks for catching this. You're reading it correctly. The "Rose Lake Capital invested in Ivanhoe Atlantic" line in my dossier was an inference from Pham's overlapping advisory roles, not a documented cap-table entry. I've spent the last several hours re-running every primary-source venue I can reach, and I want to walk you through what I actually have versus what I overreached on. Everything below is sourced and the underlying documents are now in the public repo at https://github.com/barkleesanders/doge-phantom-winery — I'll point to specific file paths.

## What I can and cannot prove

**Hard documented (with primary citations):**

1. **Pham is on the SEC record as an HPX/Ivanhoe Atlantic director.** HPX (CIK 0001662195) filed Form D on June 18, 2024 listing J. Peter Pham as Director — alongside Bronwyn Barnes (Executive Officer + Director), Tsang, Lau, Bohem, Bradley, and Sandenburgh. Same filing reports a $324.5M offering, $193M sold to 14 accredited investors only, equity, Reg D 506(b). File: `archive/sec-form-d/hpx_form-d_2024-06-18.xml`. Direct SEC link: `https://www.sec.gov/Archives/edgar/data/1662195/000166219524000001/primary_doc.xml`.

2. **Pham was also listed as an advisor on Rose Lake Capital's website** per the Sept 1, 2025 Wayback snapshot of `roselakecap.com` (since scrubbed Sept-Oct 2025). That's the personnel-overlap fact.

**Not documented (where I overreached):**

The chain "Pham advises Rose Lake → Pham chairs Ivanhoe Atlantic" doesn't establish that Rose Lake holds equity in Ivanhoe Atlantic. **No primary record I can locate puts Rose Lake Capital in the Ivanhoe Atlantic cap table.** The defensible framing is personnel overlap, not equity participation.

I'm correcting EVIDENCE.md and NETWORK.md to reflect this. Full correction memo: `evidence/2026-05-followup-kerr/CORRECTION_AND_NEW_FINDINGS.md`.

## What I checked (negative confirmations all in the repo)

- **All five HPX Form D filings (2015, 2019, 2021, 2022, 2024)** + I-Pulse's six Form Ds — no Mynett, Hoffman, or Rose Lake-affiliated person on any officer/director slate. `archive/sec-form-d/`
- **Comer's Feb 5, 2026 letter to Mynett** — does not mention Ivanhoe Atlantic, HPX, Liberia, Guinea, Pham, or Friedland anywhere. Comer's own words: *"these companies do not publicly list their investors or where their money comes from."* `archive/court-filings/comer-letter-to-mynett_2026-02-05.pdf`
- **Mohd v. eStCru complaint** (Sacramento Superior 23CV010043) — scoped strictly to wine fraud; no cross-reference to any other Mynett vehicle. `archive/court-filings/mohd-v-estcru_complaint_2023-10-17.pdf`
- **MIGA $123.3M Nimba political-risk guarantee** — issued directly to HPX (US), expired March 11, 2025. No Rose Lake in the structure. `archive/miga/miga_nimba-iron-ore_project-brief_2021.html`
- **UK Companies House — Ivanhoe Atlantic UK Limited #08248083** — 0 active PSCs; ceased PSC was Euronimba Limited (Jersey #49971), unwound April 6, 2016. No Mynett/Hailer. `archive/uk-companies-house/`
- **Jersey FSC — Euronimba Limited #49971** — Active, registered 23/04/1991; 46 documents on file. Public search confirms no Mynett-family directors.
- **FARA + Senate LDA + House LDA** — zero Rose Lake registrations
- **GLEIF (global LEI registry, 12.8 GB)** — no LEI for any HPX/I-Pulse/Ivanhoe-orbit entity, despite $325M+ in private placements
- **OpenOwnership Register** — closed Nov 29, 2024
- **Liberia LEITI BO portal** — no Ivanhoe / HPX / SMFG records (compliance gap)

## What I did newly find that's worth your time

These are separate findings I think your story should run with:

1. **$1.56M+ in registered Ivanhoe Atlantic federal lobbying — through Yorktown Solutions and Brownstein Hyatt, not Rose Lake.** I pulled the Senate LDA API directly. 20 filings. Yorktown Solutions (Daniel Vajdich's firm) has billed $120K/quarter since May 2023. BHFS has billed $50K/quarter since Q4 2023. The 2023 registration text lays out the entire policy ask verbatim — geopolitical importance of iron ore, China supply-chain competition, need for HPX rail access through Liberia, citing Liberian Presidential Executive Order 112. Full LDA dump: `archive/lda-filings/lda-api_ivanhoe-atlantic_full.json`.

2. **Samantha Carl-Yoder pipelined from BHFS lobbyist to Ivanhoe Atlantic non-executive director.** She was the registered BHFS lobbyist for the company from Q4 2023 through Q1 2026 (27 months) before being named to its board on Feb 17, 2026. That's a clean optics piece.

3. **MIGA's $123.3M Nimba political risk guarantee EXPIRED March 11, 2025** — meaning when the Liberian House ratified the rail concession on December 11, 2025, the political risk insurance backstop was no longer in force. I haven't seen anyone publish this.

4. **The Australian IPO (would have produced a substantial-shareholders disclosure) was shelved on December 16, 2025** specifically because of the China-CCP scrutiny from Moolenaar's Dec 9 letter. So the prospectus that would settle this question was never lodged. Source: Capital Brief, cached at `archive/capital-brief_ivanhoe-asx-shelved_2025-12-16.html`.

5. **Comer's Feb 19, 2026 deadline blew with no production and no follow-up subpoena.** As of today (May 6, 2026) there's no contempt referral, no follow-up letter, nothing. Comer's next Oversight subpoena went to AG Bondi on Epstein files.

6. **eStCru terminated April 4, 2026** in California, 9 days after Omar filed an amended FD writing eStCru down to zero net value. Washington Times reported this Apr 25, 2026.

7. **William Hailer is named "beneficial owner" of Rose Lake Capital DC branch** in the DC qualifying foreign-LLC filing (#C00007470247, native ID EXTUID_4329642, filed 29 Sept 2022). DC requires 25%+ beneficial-ownership disclosure on the qualifying form. Source: OpenCorporates DC entity record. Status now: Revoked. Same WeWork (80 M St SE FL 1, Washington DC 20003) is also the active address for Mynett's separate ESTREETCO LLC New York branch.

8. **Mynett's full LLC portfolio is bigger than the dossier covered.** OpenCorporates officer search returns 17 entities he's named on, including: Mynett Group (The) LLC (DC, 2014–2019); E Street Group LLC (DC + 4 state branches); ESTREETCO LLC (separate from E Street Group — CA parent + 6 state branches + a UK Limited at 1 Kings Avenue London); ESTCRU LLC (CA + NM + WV); EST VENTURES LLC (DC, with Hailer as beneficial owner); Rose Lake Capital LLC (DE + revoked DC).

9. **Zero LEIs across the entire HPX/Ivanhoe orbit.** I downloaded GLEIF's 12.8 GB SQLite and grepped — no Legal Entity Identifier for HPX, High Power Exploration, Ivanhoe Atlantic, I-Pulse, Euronimba, SMFG, Ivanhoe Liberia, or Rose Lake. That's an unusual absence for any operation raising hundreds of millions in private placements; most institutional investors require LEIs.

## Avenues left to actually settle the equity question

If you want to nail it cold:

- **Jersey FSC myRegistry** — free account; download Euronimba Limited #49971's Annual Returns + the 4 Special Resolutions clustered in May-Dec 2020 + the 15/01/2013 Register of Members. £0 per PDF. That's the highest-yield path.
- **MIGA Disclosure of Information Request** — get the annexes to the Nimba Contract of Guarantee.
- **Ivanhoe Atlantic's next U.S. Form D** — Feb 1, 2026 board press release said *"future capital raising to be primarily focused on the U.S."* — a new Reg D filing should land on EDGAR within months and any Mynett-affiliated subscriber would be detectable from related-person disclosures.

Happy to chat off the record — your number's in your signature, I can call any time today or tomorrow. Or barkleesanders@gmail.com if email is faster.

Best,
Barklee

---

**Repo with full sourcing:** https://github.com/barkleesanders/doge-phantom-winery
**Specific file with this analysis:** evidence/2026-05-followup-kerr/CORRECTION_AND_NEW_FINDINGS.md
