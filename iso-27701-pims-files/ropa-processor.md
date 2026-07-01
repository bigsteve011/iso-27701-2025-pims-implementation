# Records of Processing Activities (RoPA) — Processor Role
### Meridian HR Cloud — PIMS · ISO/IEC 27701:2025

| Field | Value |
|---|---|
| Document ID | PIMS-ROPA-P-001 |
| Version | 1.0 |
| Role | **PII Processor** (processing on customer's documented instructions) |
| Owner | Privacy Lead / DPO |
| Legal anchor | GDPR Art. 30(2); ISO/IEC 27701:2025 A.1.b, A.3.a |
| Review cycle | Semi-annual, or on new customer/sub-processor |
| Classification | Internal |

---

## 1. Scope of This Record

This RoPA covers processing carried out **on behalf of customers (controllers)**. Meridian does **not** determine the purposes of this processing; it acts strictly on each customer's documented instructions per the executed Data Processing Agreement (DPA).

**Key principle:** every activity here is bounded by a customer instruction. Any processing outside instruction is a nonconformity (see risk PR-02).

---

## 2. Processing Activities (on behalf of controllers)

### PA-P1 — Payroll Processing (SaaS)
| Attribute | Detail |
|---|---|
| Controller | Business customer |
| Purpose (as instructed) | Calculate and administer customer payroll |
| PII principals | Customer's employees |
| PII categories | Identity, salary/financial, tax IDs, bank details |
| Nature of processing | Storage, computation, reporting, transmission to banks/authorities as directed |
| Sub-processors | Cloud hosting; payment file transmission (see register) |
| Retention | Per customer instruction / contract; return or delete on exit |
| Transfers | Per customer's authorized regions + mechanisms |
| Security | Encryption, segregation of tenant data, access logging |

### PA-P2 — Benefits Administration (SaaS)
| Attribute | Detail |
|---|---|
| Controller | Business customer |
| Purpose (as instructed) | Administer employee benefits enrollment & records |
| PII principals | Customer's employees (and dependents where provided) |
| PII categories | Identity, benefits elections, possibly health-related data |
| Special-category note | Elevated safeguards where health data is present |
| Sub-processors | Cloud hosting; benefits-carrier integrations as authorized |
| Retention | Per customer instruction; secure disposal on exit |
| Security | Field-level protection, least-privilege access |

### PA-P3 — Performance & Talent Records (SaaS)
| Attribute | Detail |
|---|---|
| Controller | Business customer |
| Purpose (as instructed) | Host performance reviews and talent records |
| PII principals | Customer's employees |
| PII categories | Identity, performance evaluations, development notes |
| Sub-processors | Cloud hosting |
| Retention | Per customer instruction |
| Security | Tenant isolation, access control, audit trail |

---

## 3. Processor Obligations Matrix

| Obligation (GDPR Art. 28 / 27701 A.3) | Meridian's implementation |
|---|---|
| Process only on documented instructions | DPA + instruction logging; change-control gate |
| Confidentiality of authorized personnel | Contractual + role-based access |
| Assist with data subject requests | DSR-assist workflow + SLA to customer |
| Assist with breach notification | Notification within contractual timeline; supports 72-hour clock |
| Sub-processor authorization & flow-down | Register + prior authorization + equivalent terms |
| Return/delete PII at end of service | Exit procedure with disposal evidence |
| Support audits / demonstrate compliance | Evidence base, SoA, and customer audit support |

Cross-reference: `07-contracts-and-subprocessors/` and `06-data-subject-rights/dsr-response-sla.md`

---

## 4. Sub-processor Summary

| Sub-processor (illustrative) | Function | Location | Customer authorization |
|---|---|---|---|
| Cloud Hosting Provider | Infrastructure | Region-configurable | General authorization + register |
| Payment File Gateway | Payroll transmission | In-region | Activity-specific |
| Email/Notification Service | Transactional messaging | Region-configurable | General authorization |

Full detail: `07-contracts-and-subprocessors/subprocessor-register.md`

---

## 5. Change Log

| Version | Date | Change |
|---|---|---|
| 1.0 | *[date]* | Initial processor RoPA established |

> *Fictional reference document — no real personal data is represented.*
