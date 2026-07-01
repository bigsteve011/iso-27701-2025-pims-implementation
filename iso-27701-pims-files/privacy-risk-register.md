# Privacy Risk Register
### Meridian HR Cloud — PIMS · ISO/IEC 27701:2025 (Clause 6)

| Field | Value |
|---|---|
| Document ID | PIMS-RISK-001 |
| Version | 1.0 |
| Owner | Privacy Lead / DPO |
| Methodology | `03-privacy-risk/privacy-risk-methodology.md` |
| Review cycle | Quarterly, or on trigger event (new processing, incident, regulatory change) |
| Classification | Internal |

---

## 1. Scoring Model

Privacy risk is scored on **Likelihood (1–5) × Impact (1–5)**, where Impact weighs harm **to PII principals** first (not just to the organization) — a deliberate 27701 emphasis. Residual risk reflects the score after treatment controls are applied.

| Band | Score | Action |
|---|---|---|
| 🟥 Critical | 20–25 | Immediate treatment; executive visibility |
| 🟧 High | 12–19 | Treatment plan with owner + due date |
| 🟨 Medium | 6–11 | Treat or monitor with justification |
| 🟩 Low | 1–5 | Accept / monitor |

Where a quantitative view aids prioritization, **ALE = SLE × ARO** is noted (Single Loss Expectancy × Annual Rate of Occurrence). Figures are illustrative.

---

## 2. Risk Register

| ID | Risk description | Role | Affected principals | L | I | Inherent | Treatment / controls | Residual | Owner | Status |
|---|---|---|---|---|---|---|---|---|---|---|
| PR-01 | Excessive PII collected in HRIS beyond stated purpose (data minimization failure) | Controller | Staff | 3 | 4 | 🟧 12 | Field-level purpose mapping; collection review at design; RoPA enforcement | 🟨 6 | Product Privacy Lead | 🟡 In progress |
| PR-02 | Customer employee PII processed outside documented instructions | Processor | Customer staff | 2 | 5 | 🟨 10 | Instruction logging; contractual scope controls; change-control gate | 🟩 4 | Service Delivery | ✅ Treated |
| PR-03 | Sub-processor added without customer authorization / flow-down gap | Processor | Customer staff | 3 | 4 | 🟧 12 | Sub-processor register + authorization workflow; DPA flow-down clauses | 🟨 6 | Vendor Risk | 🟡 In progress |
| PR-04 | Data subject request (DSR) missed within regulatory deadline | Both | All | 3 | 3 | 🟨 9 | DSR ticketing with SLA timers; escalation; monthly KPI | 🟩 4 | Privacy Ops | ✅ Treated |
| PR-05 | Unlawful international transfer of PII (no valid transfer mechanism) | Both | Staff + customer staff | 3 | 4 | 🟧 12 | Transfer mapping; SCCs/transfer tooling; sub-processor location register | 🟨 8 | DPO | 🟡 In progress |
| PR-06 | Retention beyond necessity (terminated-employee records not purged) | Both | Staff + customer staff | 4 | 3 | 🟧 12 | Retention schedule; automated purge jobs; disposal evidence | 🟨 6 | Data Engineering | 🟡 In progress |
| PR-07 | Marketing consent not captured or withdrawal not honored | Controller | Prospects | 3 | 3 | 🟨 9 | Consent management platform; suppression list sync | 🟩 4 | Marketing Ops | ✅ Treated |
| PR-08 | Personal data breach with delayed detection/notification | Both | All | 2 | 5 | 🟨 10 | Incident process aligned to GDPR 33/34; 72-hour clock; customer notify SLA | 🟨 6 | Security/DPO | 🟡 In progress |
| PR-09 | Inadequate transparency (privacy notice stale vs actual processing) | Controller | Staff + prospects | 3 | 2 | 🟨 6 | Notice-to-RoPA reconciliation at each review | 🟩 3 | Privacy Ops | ✅ Treated |
| PR-10 | Insufficient staff awareness leads to mishandling of PII | Both | All | 3 | 3 | 🟨 9 | Role-based privacy training; phishing/handling drills; completion KPI | 🟨 6 | People Ops | 🟡 In progress |

---

## 3. Illustrative Quantification (selected risks)

| ID | SLE (illustrative) | ARO | ALE | Note |
|---|---|---|---|---|
| PR-08 | $180,000 | 0.3 | $54,000 | Breach handling, notification, remediation, customer churn |
| PR-05 | $90,000 | 0.4 | $36,000 | Regulatory exposure + remediation on transfer finding |
| PR-06 | $40,000 | 0.6 | $24,000 | Over-retention finding + purge remediation effort |

> ALE is directional and used to sequence treatment investment, not as a precise loss forecast.

---

## 4. Treatment Summary

| Treatment strategy | Count | Example |
|---|---|---|
| Mitigate | 8 | PR-01, PR-03, PR-05, PR-06, PR-08, PR-10 |
| Mitigate + Transfer (contractual) | 1 | PR-02 (contractual liability + controls) |
| Accept (monitored) | 1 | Low-residual items reviewed quarterly |

Open high-residual items (🟧 at inherent, still 🟨 at residual) carry a named owner and due date and are standing inputs to the **management review** (Clause 9) and **continual improvement** (Clause 10).

> *Fictional reference document — all entities, figures, and scores are illustrative.*
