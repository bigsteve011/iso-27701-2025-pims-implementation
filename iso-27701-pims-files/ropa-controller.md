# Records of Processing Activities (RoPA) — Controller Role
### Meridian HR Cloud — PIMS · ISO/IEC 27701:2025

| Field | Value |
|---|---|
| Document ID | PIMS-ROPA-C-001 |
| Version | 1.0 |
| Role | **PII Controller** (Meridian determines purposes & means) |
| Owner | Privacy Lead / DPO |
| Legal anchor | GDPR Art. 30(1); ISO/IEC 27701:2025 A.1.b |
| Review cycle | Semi-annual, or on new processing |
| Classification | Internal |

---

## 1. Scope of This Record

This RoPA covers processing where Meridian acts as **controller** — i.e., it decides *why* and *how* PII is processed. It excludes customer-directed processing, which is recorded separately in `ropa-processor.md`.

**Controller / DPO contact:** Privacy Office, privacy@[fictional-domain]

---

## 2. Processing Activities

### PA-C1 — Employee & HR Administration
| Attribute | Detail |
|---|---|
| Purpose | Employment administration, payroll, benefits, performance |
| PII principals | Current & former employees, contractors |
| PII categories | Identity, contact, financial (bank/tax), employment records, performance |
| Special categories | Health (sick leave), where applicable — elevated safeguards |
| Lawful basis | Contract (employment); legal obligation (tax/payroll); consent (optional benefits) |
| Recipients | Payroll provider, benefits carriers, tax authorities |
| Retention | Duration of employment + statutory retention post-exit |
| Transfers | Within region; any cross-border via approved mechanism |
| Safeguards | Access control, encryption at rest/in transit, minimization |

### PA-C2 — Recruitment & Candidate Management
| Attribute | Detail |
|---|---|
| Purpose | Sourcing, evaluating, and onboarding candidates |
| PII principals | Job applicants |
| PII categories | Identity, contact, CV/employment history, interview notes |
| Lawful basis | Legitimate interests (recruitment); consent (talent pool retention) |
| Recipients | Applicant tracking system provider |
| Retention | Duration of process + defined talent-pool period with consent |
| Transfers | As per ATS hosting region |
| Safeguards | Role-based access, retention purge, candidate transparency notice |

### PA-C3 — Sales & Marketing / Prospect Management
| Attribute | Detail |
|---|---|
| Purpose | Lead generation, marketing communications, event follow-up |
| PII principals | Prospects, business contacts |
| PII categories | Contact, company role, engagement/behavioral data |
| Lawful basis | Consent (electronic marketing); legitimate interests (B2B outreach) |
| Recipients | CRM provider, email marketing platform |
| Retention | Until consent withdrawal or defined inactivity threshold |
| Transfers | Per tooling hosting region; transfer mechanism where required |
| Safeguards | Consent management, suppression lists, preference center |

### PA-C4 — Website, Cookies & Analytics
| Attribute | Detail |
|---|---|
| Purpose | Site operation, security, analytics, preference handling |
| PII principals | Website visitors |
| PII categories | Online identifiers, device/usage data, cookie IDs |
| Lawful basis | Consent (non-essential cookies); legitimate interests (security/essential) |
| Recipients | Analytics provider, CDN/security provider |
| Retention | Per cookie lifetime and analytics configuration |
| Transfers | Per provider hosting; transfer mechanism where required |
| Safeguards | Consent banner, essential/non-essential split, IP handling controls |

---

## 3. Rights Enablement Summary

| Right (GDPR Art. 12–22) | How supported |
|---|---|
| Access / portability | DSR procedure with identity verification |
| Rectification | Self-service + Privacy Ops workflow |
| Erasure / objection | Honored subject to legal-retention exceptions |
| Consent withdrawal | Preference center + suppression sync |

Cross-reference: `06-data-subject-rights/dsr-procedure.md`

---

## 4. Change Log

| Version | Date | Change |
|---|---|---|
| 1.0 | *[date]* | Initial controller RoPA established |

> *Fictional reference document — no real personal data is represented.*
