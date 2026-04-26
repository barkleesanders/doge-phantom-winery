# Submission Status — 2026-04-25

## ✅ COMPLETED — Sent successfully

| # | Recipient | Method | Confirmation | Message ID |
|---|-----------|--------|--------------|------------|
| 1 | Wall Street Journal (`wsjcontact@wsj.com`) | Composio Gmail | ✅ Sent | 19dc73a35008fbe5 |
| 2 | Washington Free Beacon (`comments@freebeacon.com`) | Composio Gmail | ✅ Sent | 19dc73a477eea4e2 |
| 3 | Daily Caller (`tips@dailycaller.com`) | Composio Gmail | ✅ Sent | 19dc73a4c88d5e5e |
| 4 | ProPublica (`propublica.org/tips`) | unbrowse + secure form | ✅ "Thanks for submitting a tip." | n/a |
| 5 | House Ethics Committee (`ethics.house.gov`) | unbrowse + Gravity Forms | ✅ "The House Committee on Ethics has received your submission and it will be reviewed by non-partisan staff." | n/a |

## ⏳ READY-BUT-PENDING-USER (CAPTCHA / PII)

### CA AG Consumer Complaint
- **URL:** https://oag.ca.gov/contact/consumer-complaint-against-business-or-company
- **Status:** Form fully populated in browser session `5ef2a298-2aa1-4329-9ea6-042869ca7f68`
- **All fields set:** Name, address (1070 Bridgeview Way #310 SF 94158), eStCru company info, complaint description, reasonable resolution, all required radios.
- **Blocker:** Google reCAPTCHA v2 — must be solved by human
- **To finish:** Open the browser session, solve the reCAPTCHA, click Submit.
- **Or:** Re-fill from `submissions/06-ca-ag-complaint.md`

### SEC TCR (Tip, Complaint, or Referral)
- **URL:** https://www.sec.gov/submit-tip-or-complaint/tcr-disclaimer
- **Status:** Narrative drafted in `submissions/01-sec-tcr-narrative.md`
- **Why not submitted live:** SEC's Drupal multi-page wizard requires PII (name, address, phone, optional SSN for award eligibility) and an Altcha CAPTCHA at end of page 1. Multi-page state was difficult to drive via automation.
- **To finish:** Manually paste narrative through pages 1-7 of the wizard. Submit will return a confirmation number; preserve it. Within 30 days, optionally file Form WB-APP to perfect award eligibility.

## Notes

- All 3 emails sent from `barkleesanders@gmail.com` via Composio.
- All form submissions used the `unbrowse` browser session created by /unbrowse skill.
- Public dossier link in every submission: https://github.com/barkleesanders/doge-phantom-winery
- Live magazine link: https://barkleesanders.github.io/doge-phantom-winery/

## Distribution rationale (recap)

- **Tier 1 (highest leverage, potential whistleblower award):** SEC TCR — strongest legal theory (§80b-3 / §230.503 / §10(b) provable from public record alone)
- **Tier 2 (most actionable parallel):** Investigative journalists with editorial reach + legal review (WSJ, Free Beacon, Daily Caller, ProPublica)
- **Tier 3 (paper trail / situational awareness):** House Ethics, CA AG — low-cost, creates a record, agencies already aware
