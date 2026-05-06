# Brownstein Hyatt Farber Schreck — 2024 LD-203 Sweep (Clean Negative)

**Question:** Did Lauren Carl-Yoder or Lauren Diekman (Maddox) at BHFS report contributions to Ilhan Omar campaigns or Mynett-affiliated PACs on their 2024 sworn semi-annual lobbying contribution reports (LD-203)?

**Method:** Pulled all 7 pages of LD-203 filings for "Brownstein Hyatt" registered with the Senate LDA for filing year 2024 (170 reports total). Aggregated all `contribution_items` arrays across all pages (1,777 total reported contributions). Grepped the consolidated dump for the surnames Carl-Yoder, Diekman, Maddox, Mynett, Hailer, Pham, plus the strings ILHAN and OMAR.

**Result:**
- **0 hits** for "Carl-Yoder"
- **0 hits** for "Diekman" or "Maddox"
- **0 hits** for "ILHAN" or "OMAR"
- **0 hits** for "MYNETT" or "HAILER" or "PHAM"

**Implication:** No reported lobbyist contributions from BHFS principals (Carl-Yoder, Diekman, etc.) into Mynett-adjacent committees or Ilhan Omar's campaign during 2024. This does not foreclose contributions made *outside* the LDA-coverage window (private donations under $200, contributions outside reportable categories, contributions in early 2025 not yet captured), but for the 2024 reporting period the negative is clean across 1,777 disclosed line items.

**Source:** lda.senate.gov/api/v1/contributions/?registrant_name=Brownstein+Hyatt&filing_year=2024 (pages 1-7, page_size=25)
