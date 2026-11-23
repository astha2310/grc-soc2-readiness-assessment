# Security Exceptions Register

*Maintained by: IT & Security · Last updated: 2026-09-14*

| ID | Requirement | Account / system | Reason | Compensating controls | Approved by | Approved on | Expires |
|---|---|---|---|---|---|---|---|
| EX-2026-01 | 4.1 MFA | admin-breakglass@brightline.example | Emergency access account must work if MFA service is down | 30-character password stored in a sealed safe; any sign-in triggers an immediate SIEM alert to Head of Security; sign-ins reviewed monthly | Dana Ortiz (Head of Security) | 2026-01-12 | 2027-01-12 |
| EX-2026-02 | 4.1 MFA | svc-backup@brightline.example | Backup software does not support MFA | Can only sign in from the backup server's IP address; no interactive login; password rotated every 90 days | Dana Ortiz (Head of Security) | 2026-09-14 | 2027-03-14 |
| EX-2025-04 | 6.2 Patch deadline | finance-laptop-07 | Legacy accounting add-in incompatible with OS update | Device removed from network | Dana Ortiz (Head of Security) | 2025-05-02 | 2025-11-02 |

*No other exceptions are on file.*
