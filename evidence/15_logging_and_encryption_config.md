# Logging and Encryption Configuration (as of 2026-11-30)

*Exported by IT & Security for the SOC 2 readiness review.*

## A. SIEM log sources and retention

| Log source | Sent to SIEM | Searchable (hot) | Archive | Total retention |
|---|---|---|---|---|
| Entra ID sign-in and audit logs | Yes | 90 days | 300 days | 390 days |
| AWS CloudTrail (production) | Yes | 90 days | 300 days | 390 days |
| GitHub organization audit log | Yes | 90 days | 300 days | 390 days |
| CloudNest database audit logs | Yes | 90 days | 300 days | 390 days |
| NetLedger audit log | Yes | 90 days | 300 days | 390 days |

Oldest log record available in archive: **2025-10-27** (SIEM went live 2025-10-26).

## B. Encryption at rest (CloudNest)

| Resource | Contains | Encryption at rest | Algorithm |
|---|---|---|---|
| customer-db-01 | Customer data | Enabled | AES-256 |
| customer-db-02 (replica) | Customer data | Enabled | AES-256 |
| analytics-db-01 | Usage data | Enabled | AES-256 |
| storage: customer-uploads | Customer files | Enabled | AES-256 |
| storage: backups | Database backups | Enabled | AES-256 |
| storage: public-assets | Website images (public) | Not enabled | — |

## C. Encryption in transit

| Endpoint | Minimum TLS version |
|---|---|
| app.brightline.example | TLS 1.2 |
| api.brightline.example | TLS 1.2 |
| Internal service-to-service traffic | TLS 1.2 |
