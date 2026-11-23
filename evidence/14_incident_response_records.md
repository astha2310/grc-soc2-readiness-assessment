# Incident Response Records

## A. Incident Response Plan: document details

| Field | Value |
|---|---|
| Document | Incident Response Plan (IRP-001) |
| Version | 2.0 |
| Owner | Head of Security |
| Last reviewed | 2023-06-14 |
| Approved by | Miguel Alvarez (CTO), 2023-06-20 |

## B. Tabletop exercises

| Date | Scenario | Participants | Notes |
|---|---|---|---|
| 2022-11-03 | Ransomware on file server | IT, Engineering leads | Lessons learned documented |

*No tabletop exercises recorded since November 2022.*

## C. Incident log, 2026

| Incident | Date | Type | Summary | Containment | Corrective action | Action status |
|---|---|---|---|---|---|---|
| INC-2026-004 | 2026-03-22 | Malware | Adware found on a Marketing laptop via browser extension | Laptop reimaged | Block unapproved browser extensions | Closed 2026-04-30 |
| INC-2026-007 | 2026-09-18 | Account compromise | j.morales@brightline.example entered credentials on a fake "shared document" page. Attacker signed in from an overseas IP and created an inbox forwarding rule sending invoices to an external address. Detected 2 days later by a customer. | Password reset, sessions revoked, forwarding rule removed | Enforce MFA for this user; alert on new external forwarding rules | **Open** |
| INC-2026-009 | 2026-10-29 | Credential stuffing | Spike in failed logins on customer login API | Emergency rate-limiting deployed (CHG-1047) | Permanent bot protection on login API | In progress |
