# Jersey FSC Order TR1995483 — Email Receipt Verification

**Source:** Gmail thread `19dff1ab88d97feb` from `donotreply-myregistry@jerseyfsc.org`, 25 messages received 2026-05-06 22:03 BST
**Account:** barkleesanders@gmail.com (Jersey FSC myRegistry account)
**Cost:** £0.00 (free public-register documents)
**Result:** 25/25 documents accounted for — every IN-reference in the email receipts matches a PDF in `pdfs/` and an entry in `download-urls.json`.

This file exists to cross-check the email-receipt metadata (independent of any OCR I did on the PDFs) so the document inventory is traceable end-to-end.

| # | Email IN-ref | Jersey FSC SR-number | Document type | Document date | PDF in repo |
|---|---|---|---|---|---|
| 1 | IN10747202 | SR1873949 | Special Resolution | 2020-05-29 | ✅ |
| 2 | IN10747203 | SR1623173 | Annual Return | 2017-02-17 | ✅ |
| 3 | IN10747204 | SR1530264 | Annual Return | 2015-02-27 | ✅ |
| 4 | IN10747205 | SR1799999 | Special Resolution | 2019-04-02 | ✅ |
| 5 | IN10747206 | SR1102218 | Special Resolution | 2007-09-20 | ✅ |
| 6 | IN10747207 | SR1903039 | Special Resolution | 2020-12-02 | ✅ |
| 7 | IN10747208 | SR1479205 | Register of Members | 2013-01-15 | ✅ ⚠️ withdrawn |
| 8 | IN10747209 | SR1854785 | Annual Return | 2020-02-19 | ✅ POST-HPX |
| 9 | IN10747210 | SR1263298 | Annual Return | 2010-05-10 | ✅ |
| 10 | IN10747211 | SR1205224 | Annual Return | 2009-02-27 | ✅ |
| 11 | IN10747212 | SR1803369 | Annual Return | 2019-02-25 | ✅ Last pre-HPX |
| 12 | IN10747213 | SR1569856 | Annual Return | 2016-02-17 | ✅ |
| 13 | IN10747214 | SR1478491 | Annual Return | 2014-02-28 | ✅ |
| 14 | IN10747215 | SR1129310 | Special Resolution | 2008-02-14 | ✅ Auth cap → $100M |
| 15 | IN10747216 | SR1355134 | Annual Return | 2012-02-17 | ✅ |
| 16 | IN10747217 | SR1221700 | Special Resolution | 2009-11-17 | ✅ |
| 17 | IN10747218 | SR2279063 | Special Resolution — Change of Shares | 2022-05-19 | ✅ Auth cap → $1B |
| 18 | IN10747219 | SR1876521 | Special Resolution | 2020-06-11 | ✅ Ratifies HPX issuance |
| 19 | IN10747220 | SR1805565 | Special Resolution | 2019-04-25 | ✅ |
| 20 | IN10747221 | SR1709154 | Annual Return | 2018-02-16 | ✅ Pre-HPX |
| 21 | IN10747222 | SR1571836 | Annual Return | 2016-02-17 | ✅ (2nd 2016 AR) |
| 22 | IN10747223 | SR1418298 | Annual Return | 2013-02-28 | ✅ |
| 23 | IN10747224 | SR1310913 | Annual Return | 2011-02-28 | ✅ |
| 24 | IN10747225 | SR1217933 | Special Resolution | 2009-09-09 | ✅ Auth cap → $200M |
| 25 | IN10747226 | SR1125976 | Annual Return | 2008-02-08 | ✅ |

## Special note on IN10747208 (Register of Members 2013-01-15, SR1479205)
This document was filed by Mourant on 2013-01-15 but **REMOVED FROM THE PUBLIC REGISTER on 13 March 2014** by JFSC notice — the rationale stated on the JFSC removal record is "filed in error." The PDF returned by the order is the JFSC removal/withdrawal notice, not the original Register of Members content.

Implication: the only date for which a complete Euronimba shareholder list was ever publicly registered (and is now withdrawn) was 15 January 2013. The Annual Returns 2008-2019 list shareholders by reference but the share counts are summarized rather than enumerated per holder. The Feb 19, 2020 AR (post-HPX) shows HPX Nimba Holdings Inc. as 100% holder of 20,753,489 ordinary shares.

This withdrawn 2013 Register would have been the most authoritative pre-HPX cap table snapshot. It is no longer available; recreating it would require a Mourant FOI/SAR-style request or a JFSC archival query.

## Coverage cross-check

| Source | Count |
|---|---|
| Gmail order-receipt emails | 25 |
| Unique IN-references in emails | 25 (IN10747202 → IN10747226 inclusive) |
| Unique TR (Transaction) reference | 1 (TR1995483) |
| PDFs in `pdfs/` directory | 25 |
| Entries in `download-urls.json` | 25 |
| In email but NOT in repo | **0** |
| In repo but NOT in email | **0** |

Verified: 2026-05-06.
