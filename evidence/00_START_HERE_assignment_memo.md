# MEMO: SOC 2 Readiness Assessment

**To:** Astha Patel, GRC Analyst
**From:** Dana Ortiz, Head of Security
**Date:** December 1, 2026
**Subject:** Your first assignment: are we ready for SOC 2?

---

Welcome to Brightline!

Three of our biggest customers (two healthcare networks and a regional bank) have told us they won't renew next year unless we give them a **SOC 2 Type I report**. We've booked an external audit firm for **March 2027**.

Before the auditors arrive, I need an honest answer: **if they tested us today, what would they find?**

## Your assignment
Test the 13 controls below. For each one:
1. Read what our **policy** requires (`02_information_security_policy.md`).
2. Review the **evidence** in this folder.
3. Decide whether the control is **Effective** or **Deficient**, and write down exactly what you found.
4. For every deficiency, assess the **risk** and recommend a fix.

Some evidence will look bad but turn out fine. Some will look fine but hide a problem. Check the details. Auditors will.

**Important:** if you find anything that looks like an **active security incident**, don't wait for the report. Tell me right away.

## What I need from you
1. **Control testing worksheet:** one row per control, with your test, evidence, result and finding
2. **Risk register:** one row per risk, with likelihood, impact, score, owner, treatment and target date
3. **Executive summary:** 1–2 pages for the CEO and CTO: are we ready, what are the top risks, and what must be fixed before March?

## Scope
- **Framework:** SOC 2, Security criteria (Common Criteria) only
- **Evidence date:** as of **November 30, 2026**
- **Systems:** Entra ID, AWS production, GitHub, NetLedger (finance), CloudNest-hosted production databases

## Controls to test

| ID | Control | SOC 2 | NIST CSF 2.0 | Evidence |
|---|---|---|---|---|
| C1 | Security policy is reviewed and approved every year | CC5.3 | GV.PO | 02 |
| C2 | Privileged access is reviewed every quarter | CC6.2, CC6.3 | PR.AA | 03 |
| C3 | Access is removed within 1 business day when someone leaves | CC6.2 | PR.AA | 03, 04, 05 |
| C4 | MFA is required for all accounts | CC6.1 | PR.AA | 06, 07 |
| C5 | Employees complete security awareness training | CC2.2 | PR.AT | 08 |
| C6 | Phishing simulations run every quarter | CC2.2 | PR.AT | 09 |
| C7 | Vulnerabilities are fixed within policy deadlines | CC7.1 | ID.RA | 10 |
| C8 | Production changes are approved before deployment | CC8.1 | PR.PS | 11 |
| C9 | Vendors are risk-assessed and reviewed every year | CC9.2 | GV.SC | 12 |
| C10 | The incident response plan is reviewed and tested every year | CC7.4 | RS.MA | 14 |
| C11 | Backups are taken daily and restores are tested | CC7.5 | PR.DS, RC.RP | 13 |
| C12 | Security logs are kept as long as policy requires | CC7.2 | DE.CM, PR.PS | 15 |
| C13 | Data is encrypted at rest and in transit | CC6.1, CC6.7 | PR.DS | 15 |

## Files in this folder

| # | File |
|---|---|
| 01 | Company profile |
| 02 | Information security policy |
| 03 | Q3 2026 privileged access review |
| 04 | HR terminations, 2026 |
| 05 | Current privileged access (Nov 30, 2026) |
| 06 | MFA status export from Entra ID |
| 07 | Security exceptions register |
| 08 | Security training completion, 2026 |
| 09 | Phishing simulation log, 2026 |
| 10 | Vulnerability scan results (Nov 30, 2026) |
| 11 | Sample of production change tickets, Oct–Nov 2026 |
| 12 | Vendor inventory |
| 13 | Backup and restore log, 2026 |
| 14 | Incident response records |
| 15 | Logging and encryption configuration |

Thanks, and don't be afraid to tell me bad news. That's the whole point.

— Dana
