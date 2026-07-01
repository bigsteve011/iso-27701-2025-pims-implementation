# Statement of Applicability (SoA)
### Meridian HR Cloud — PIMS · ISO/IEC 27701:2025

| Field | Value |
|---|---|
| Document ID | PIMS-SOA-001 |
| Version | 1.0 |
| Owner | Privacy Lead / DPO |
| Approved by | PIMS Steering Committee |
| Review cycle | Annual, or on material change to processing |
| Classification | Internal |

---

## 1. Purpose

This Statement of Applicability records which ISO/IEC 27701:2025 Annex A controls apply to Meridian HR Cloud's Privacy Information Management System (PIMS), the justification for inclusion or exclusion, and the current implementation status. It is the primary index an auditor uses to navigate the PIMS evidence base.

Because Meridian operates as **both a PII Controller and a PII Processor**, controls are assessed across all three Annex A groupings:

- **A.1 — General PIMS controls** (apply to all organizations)
- **A.2 — PII Controller controls**
- **A.3 — PII Processor controls** (including the information-security controls surfaced in the 2025 edition)

> The control-area descriptions below are paraphrased in the implementer's own words for mapping purposes. Official Annex A control titles and text are reproduced from the purchased ISO/IEC 27701:2025 standard in the controlled master copy of this SoA and are not included here.

**Status legend:** ✅ Implemented · 🟡 Partial / In progress · ⬜ Planned · ➖ Not applicable

---

## 2. A.1 — General PIMS Controls

| Ref | Control area (paraphrased) | Applicable | Justification | Status | Evidence |
|---|---|---|---|---|---|
| A.1.a | Identify and document the organization's role(s) as controller and/or processor for each processing activity | Yes | Meridian holds both roles; role clarity drives all downstream obligations | ✅ | `04-controller-processor-roles/role-determination-matrix.md` |
| A.1.b | Maintain records of processing activities (RoPA) | Yes | Required for both roles; core accountability evidence | ✅ | `02-ropa/` |
| A.1.c | Conduct privacy risk assessments and maintain treatment decisions | Yes | Clause 6 risk-based planning | ✅ | `03-privacy-risk/privacy-risk-register.md` |
| A.1.d | Trigger and perform DPIAs for high-risk processing | Yes | Payroll/benefits processing meets high-risk thresholds | 🟡 | `03-privacy-risk/dpia/` |
| A.1.e | Provide privacy notices / transparency information to PII principals | Yes | Controller obligation to staff, prospects, visitors | ✅ | `06-data-subject-rights/` |
| A.1.f | Establish and operate a process for handling PII principal requests | Yes | DSR handling across both roles | ✅ | `06-data-subject-rights/dsr-procedure.md` |
| A.1.g | Define retention and secure disposal rules per processing purpose | Yes | Lifecycle governance | 🟡 | `01-context-and-scope/pii-processing-context.md` |
| A.1.h | Manage privacy obligations in supplier and sub-processor relationships | Yes | Cloud/sub-processor chain | ✅ | `07-contracts-and-subprocessors/` |
| A.1.i | Awareness and competence for personnel handling PII | Yes | Clause 7 support | 🟡 | `09-performance-and-improvement/` |
| A.1.j | Privacy incident and breach handling procedure | Yes | Regulatory notification exposure (GDPR 33/34) | ✅ | linked to ISMS incident process |

---

## 3. A.2 — PII Controller Controls

Applied to processing where **Meridian determines purposes and means** (own staff, sales/marketing prospects, website visitors).

| Ref | Control area (paraphrased) | Applicable | Justification | Status | Evidence |
|---|---|---|---|---|---|
| A.2.a | Determine and document the lawful basis for each purpose | Yes | GDPR Art. 6 alignment | ✅ | `08-regulatory-crosswalk/27701-to-gdpr.md` |
| A.2.b | Obtain, record, and enable withdrawal of consent where relied upon | Yes | Marketing / non-essential cookies | 🟡 | `02-ropa/ropa-controller.md` |
| A.2.c | Provide transparency / privacy notice at or before collection | Yes | Staff and prospect notices | ✅ | `06-data-subject-rights/` |
| A.2.d | Uphold PII principal rights (access, rectification, erasure, objection, portability) | Yes | GDPR Art. 12–22 | ✅ | `06-data-subject-rights/dsr-procedure.md` |
| A.2.e | Privacy by design and by default in new systems/features | Yes | Product & internal tooling changes | 🟡 | `03-privacy-risk/dpia/dpia-methodology.md` |
| A.2.f | Governance of automated decision-making / profiling | Yes | Marketing segmentation review | ⬜ | planned Q-next |
| A.2.g | Manage joint-controller arrangements where applicable | ➖ | No current joint-controller relationships identified | ➖ | role matrix |
| A.2.h | Govern international transfers of PII (controller-initiated) | Yes | Marketing tooling hosted cross-border | 🟡 | `07-contracts-and-subprocessors/` |

---

## 4. A.3 — PII Processor Controls

Applied to **customer-directed processing** (business customers' employee payroll, benefits, and performance data).

| Ref | Control area (paraphrased) | Applicable | Justification | Status | Evidence |
|---|---|---|---|---|---|
| A.3.a | Process PII only on the documented instructions of the customer (controller) | Yes | Core processor obligation (GDPR Art. 28) | ✅ | `07-contracts-and-subprocessors/dpa-clause-checklist.md` |
| A.3.b | Support the controller in meeting PII principal rights requests | Yes | DSR assist SLAs to customers | ✅ | `06-data-subject-rights/dsr-response-sla.md` |
| A.3.c | Assist the controller with breach notification obligations | Yes | Contractual notification timelines | ✅ | incident process + DPA |
| A.3.d | Govern engagement and flow-down to sub-processors, with customer authorization | Yes | Hosting, email, analytics sub-processors | ✅ | `07-contracts-and-subprocessors/subprocessor-register.md` |
| A.3.e | Return or securely delete PII at end of service | Yes | Contract exit obligation | 🟡 | `07-contracts-and-subprocessors/flow-down-obligations.md` |
| A.3.f | Make available information necessary to demonstrate compliance / support audits | Yes | Customer audit rights | ✅ | this SoA + evidence base |
| A.3.g | Govern international transfers on behalf of the controller | Yes | Multi-region customer base | 🟡 | crosswalk + DPA |
| A.3.h | Apply information-security controls protecting processed PII (A.3 security set) | Yes | Confidentiality/integrity/availability of customer PII | 🟡 | mapped to ISO/IEC 27001 ISMS controls |

---

## 5. Exclusions Summary

| Ref | Control area | Reason for exclusion |
|---|---|---|
| A.2.g | Joint-controller arrangements | No joint-controller processing currently exists; to be reassessed on new partnerships |

All other controls are applicable. Exclusions are reviewed at each management review (Clause 9) and upon material change to processing.

---

## 6. Approval

| Role | Name | Date |
|---|---|---|
| Privacy Lead / DPO | *[signature]* | *[date]* |
| PIMS Steering Committee Chair | *[signature]* | *[date]* |

> *Fictional reference document — Meridian HR Cloud does not exist and no real PII is represented.*
