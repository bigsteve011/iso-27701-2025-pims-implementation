# Privacy Information Management System (PIMS) Implementation Blueprint
### Aligned to ISO/IEC 27701:2025 (2nd Edition — Stand-Alone PIMS)

![Standard](https://img.shields.io/badge/ISO%2FIEC-27701%3A2025-1f3a5f)
![Type](https://img.shields.io/badge/PIMS-Stand--Alone-0d7377)
![Discipline](https://img.shields.io/badge/Domain-Privacy%20%7C%20GRC-1f3a5f)
![Regulations](https://img.shields.io/badge/Mapped-GDPR%20%7C%20CCPA%2FCPRA-0d7377)
![Roles](https://img.shields.io/badge/Roles-PII%20Controller%20%2B%20Processor-e8a33d)
![Status](https://img.shields.io/badge/Blueprint-Reference%20Implementation-1f3a5f)

> An end-to-end reference implementation of a **Privacy Information Management System (PIMS)** built to the **October 2025 revision of ISO/IEC 27701**, demonstrating the full lifecycle of privacy governance design, documentation, control implementation, risk treatment, and audit readiness for an organization operating as **both a PII Controller and a PII Processor**.

---

## 📌 Overview

ISO/IEC 27701:2025 is the most significant revision of the privacy standard since its original 2019 release. It is **no longer an extension of ISO/IEC 27001** — it is now a **stand-alone management system standard** with its own full clause structure (Clauses 4–10) built on the ISO Harmonized Structure (Annex SL), the same backbone used by ISO/IEC 27001:2022 and ISO/IEC 42001:2023.

This repository is a **practitioner-grade blueprint** showing how a privacy program is scoped, documented, implemented, and made audit-ready against the current standard. It reflects the perspective of a certified **ISO/IEC 27701 PIMS Lead Auditor** — every artifact is structured the way an auditor expects to receive evidence.

> ⚠️ **Note:** All organizational data in this repository is **fictional**. "Meridian HR Cloud" and all associated records, names, and figures are illustrative and created solely to demonstrate implementation methodology. No real personal data is present.

---

## 🎯 What This Project Demonstrates

| Capability | Where It's Evidenced |
|---|---|
| PIMS scoping & context definition (stand-alone, not tied to an ISMS) | `01-context-and-scope/` |
| Controller **and** Processor dual-role governance | `04-controller-processor-roles/` |
| Records of Processing Activities (RoPA) | `02-ropa/` |
| Privacy risk assessment & treatment (risk-based Clause 6) | `03-privacy-risk/` |
| Data Protection Impact Assessment (DPIA/PIA) methodology | `03-privacy-risk/dpia/` |
| Annex A control implementation (A.1 / A.2 / A.3) | `05-annex-a-controls/` |
| Statement of Applicability (SoA) mapped to 2025 clause references | `05-annex-a-controls/SoA.md` |
| Data Subject Rights (DSR) operational procedures | `06-data-subject-rights/` |
| Contractual privacy governance (DPA / sub-processor flow-down) | `07-contracts-and-subprocessors/` |
| Regulatory crosswalk (GDPR, CCPA/CPRA) | `08-regulatory-crosswalk/` |
| Privacy KPIs / KRIs & management review | `09-performance-and-improvement/` |
| 2019 → 2025 transition gap analysis | `10-transition-2019-to-2025/` |

---

## 🏢 The Scenario — "Meridian HR Cloud"

A fictional SaaS provider of cloud HRIS and payroll software, chosen deliberately because it forces the PIMS to address **both** privacy roles:

- **As a PII Controller** — Meridian determines the purposes and means of processing for its *own* staff data, sales/marketing prospects, and website visitors.
- **As a PII Processor** — Meridian processes the *employee* personal data of its business customers (payroll, benefits, performance records) strictly on documented instructions.

This dual posture is the ideal teaching context for ISO/IEC 27701:2025, which sharpened the distinction between controller and processor responsibilities and clarified decision-making authority, purpose determination, and processing obligations.

**Illustrative scope statement:**
> *The PIMS covers the processing of personally identifiable information (PII) by Meridian HR Cloud in its delivery of SaaS HRIS and payroll services — spanning the roles of PII Controller (corporate, HR, and marketing processing) and PII Processor (customer-directed processing) — across its production cloud environment, supporting business functions, and engaged sub-processors.*

---

## 🧭 ISO/IEC 27701:2025 Clause Structure & Coverage

The 2025 edition adopts the full management-system clause set (4–10). Each clause below maps to the artifacts that provide conformity evidence.

| Clause | Title | Evidence in This Repo |
|---|---|---|
| **4** | Context of the organization | Scope, interested parties, PII processing context, boundaries |
| **5** | Leadership | Privacy policy, roles & accountability (incl. DPO/privacy lead), management commitment |
| **6** | Planning | Privacy risk assessment methodology, risk treatment plan, privacy objectives |
| **7** | Support | Competence & awareness program, documented information control, resourcing |
| **8** | Operation | PII lifecycle processes, DPIA triggers, operational controls referencing Annex A |
| **9** | Performance evaluation | KPIs/KRIs, internal audit programme, management review inputs/outputs |
| **10** | Improvement | Nonconformity & corrective action, continual improvement register |

> In the 2025 edition, planning (Clause 6) must explicitly address **privacy risks** in the organization's legal, regulatory, and operational context, and Clause 8 refers operational control down to the **Annex A** control set.

---

## 🗂️ Annex A — Consolidated Control Model

The 2025 revision **consolidated** the previously separate controller/processor annexes into a single Annex A, restructured to align with the ISO/IEC 27002:2022 control themes, and surfaced a set of information-security controls directly within the annex:

- **A.1** — General PIMS controls applicable to all organizations
- **A.2** — Controls specific to organizations acting as **PII Controllers**
- **A.3** — Controls specific to organizations acting as **PII Processors** (and the added information-security controls)

Because Meridian occupies both roles, the **Statement of Applicability** in this repo documents applicability, justification, and implementation status across **A.1, A.2, and A.3** — the exact evidence structure an auditor reviews first.

---

## 📁 Repository Structure

```
iso-27701-2025-pims-implementation/
│
├── README.md                          ← you are here
│
├── 01-context-and-scope/
│   ├── pims-scope-statement.md
│   ├── interested-parties-register.md
│   └── pii-processing-context.md
│
├── 02-ropa/
│   ├── ropa-controller.md             ← Records of Processing (controller role)
│   └── ropa-processor.md              ← Records of Processing (processor role)
│
├── 03-privacy-risk/
│   ├── privacy-risk-methodology.md
│   ├── privacy-risk-register.md       ← inherent/residual scoring + treatment
│   └── dpia/
│       ├── dpia-methodology.md
│       └── dpia-example-payroll.md
│
├── 04-controller-processor-roles/
│   ├── role-determination-matrix.md
│   └── responsibility-raci.md
│
├── 05-annex-a-controls/
│   ├── SoA.md                         ← Statement of Applicability (A.1/A.2/A.3)
│   ├── annexA1-general-controls.md
│   ├── annexA2-controller-controls.md
│   └── annexA3-processor-controls.md
│
├── 06-data-subject-rights/
│   ├── dsr-procedure.md
│   └── dsr-response-sla.md
│
├── 07-contracts-and-subprocessors/
│   ├── dpa-clause-checklist.md
│   ├── subprocessor-register.md
│   └── flow-down-obligations.md
│
├── 08-regulatory-crosswalk/
│   ├── 27701-to-gdpr.md
│   └── 27701-to-ccpa-cpra.md
│
├── 09-performance-and-improvement/
│   ├── privacy-kpi-kri-dashboard.md
│   ├── internal-audit-programme.md
│   └── management-review-template.md
│
└── 10-transition-2019-to-2025/
    └── gap-analysis-2019-to-2025.md
```

---

## 🔄 2019 → 2025 Transition Awareness

A dedicated gap analysis demonstrates fluency with the migration path, which is a live concern for every currently certified organization:

- **Structure:** clauses 5–8 → full management-system clauses **4–10**
- **Independence:** PIMS scope now defined on its own PII-processing basis, **decoupled** from ISMS scope
- **Annex:** two separate controller/processor annexes → **single consolidated Annex A** aligned to ISO/IEC 27002:2022
- **Control references:** all references renumbered; SoA must be updated from 2019 to 2025 clause/control references
- **Transition deadline:** organizations certified to the 2019 edition transition by **October 2028**

---

## 📊 Sample Regulatory Crosswalk (excerpt)

| ISO/IEC 27701:2025 Theme | GDPR Article(s) | CCPA/CPRA |
|---|---|---|
| Lawful basis & purpose specification | Art. 5, 6 | §1798.100 (notice at collection) |
| Data subject / consumer rights | Art. 12–22 | §1798.105–.130 |
| Records of processing | Art. 30 | §1798.130 (record-keeping) |
| Controller–processor obligations | Art. 28 | Service-provider contract terms |
| Breach handling | Art. 33–34 | §1798.150 (breach exposure) |
| Privacy by design & DPIA | Art. 25, 35 | Risk-assessment expectations |

---

## 👤 About

Built by a **certified ISO/IEC 27701 PIMS Lead Auditor** (Mastermind — training, examination, and certification) as a demonstration of practical PIMS implementation and audit-readiness capability across privacy governance, risk, and compliance.

**Core focus:** Governance, Risk & Compliance (GRC) · Privacy Information Management · ISO/IEC 27001 & 27701 · Third-Party Risk · Audit & Assurance.

---

## ⚖️ Disclaimer

This repository is an educational reference implementation. "Meridian HR Cloud" is fictional, and all data is illustrative. It does not reproduce copyrighted text of the ISO/IEC 27701:2025 standard; the standard must be purchased from ISO or an authorized reseller. Clause and control references are used for mapping and educational purposes only.
