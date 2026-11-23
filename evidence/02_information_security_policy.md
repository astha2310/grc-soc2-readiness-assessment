# Brightline Corp: Information Security Policy

| Field | Value |
|---|---|
| Document ID | POL-SEC-001 |
| Version | 1.3 |
| Owner | Head of Security |
| Approved by | — |
| Approval date | — |
| Last reviewed | 2024-03-11 |
| Next review due | 2025-03-11 |
| Applies to | All employees, contractors and systems |

---

## 1. Purpose
This policy sets the minimum security requirements that protect Brightline's systems and our customers' data.

## 2. Policy governance
2.1 This policy must be **reviewed at least once every 12 months** and **approved by the CTO or CEO**.
2.2 Approved exceptions to any requirement must be recorded in the **Security Exceptions Register** with a reason, an approver (Head of Security or CTO), compensating controls and an expiry date.

## 3. Access control
3.1 Access to production and privileged systems (AWS, GitHub, Entra ID admin roles, NetLedger approver roles) must be **reviewed every quarter** by the system owner. Reviews must be recorded with reviewer name, date and decision for every account.
3.2 When an employee or contractor leaves, **all access must be removed within 1 business day** of their termination date.
3.3 Access must follow least privilege.

## 4. Authentication
4.1 **Multi-factor authentication (MFA) is required for all user, administrator and service accounts** that can sign in to company systems.
4.2 Accounts that technically cannot use MFA require an **approved exception** (see 2.2) with compensating controls.

## 5. Security awareness
5.1 New employees must complete security awareness training **within 30 days of their start date**.
5.2 All employees must complete annual security awareness training **by October 31** each year.
5.3 Phishing simulations must be run **at least once per quarter**.

## 6. Vulnerability management
6.1 Production systems are scanned at least weekly.
6.2 Vulnerabilities must be fixed within these deadlines from first detection:

| Severity | Deadline |
|---|---|
| Critical | 15 days |
| High | 30 days |
| Medium | 90 days |
| Low | 180 days |

6.3 A vulnerability that can't be fixed in time may be **risk-accepted** by the CTO for a maximum of 6 months, documented with a reason and compensating controls.

## 7. Change management
7.1 Every production change requires a change ticket and **approval from someone other than the author before deployment**.
7.2 **Emergency changes** may be deployed first, but must be **approved by the CTO within 24 hours** of deployment.

## 8. Vendor management
8.1 Vendors that store or access **customer or employee data** must have a **security risk assessment before onboarding**.
8.2 For those vendors, Security must obtain and review a **current SOC 2 report** (or equivalent) **at least every 12 months**. A report is current if its period ended within the last 12 months.

## 9. Incident response
9.1 The Incident Response Plan must be **reviewed every 12 months**.
9.2 A **tabletop exercise** testing the plan must be held at least **once every 12 months**.
9.3 Corrective actions from incidents must be tracked to completion.

## 10. Backup and recovery
10.1 Production databases must be **backed up daily**.
10.2 A **restore test** must be performed at least **once per quarter** and the result recorded.

## 11. Logging and monitoring
11.1 Security logs from production systems and Entra ID must be sent to the central SIEM.
11.2 Logs must be retained for **at least 365 days**, with the most recent **90 days** immediately searchable.

## 12. Encryption
12.1 Customer data must be **encrypted at rest** (AES-256 or equivalent).
12.2 Data in transit must use **TLS 1.2 or higher**.
