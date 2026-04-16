# Medical Information Workflow Guide

> **Template version:** 1.0  
> **Scope:** Standard MI inquiry handling — HCP and patient/consumer channels  
> **Applicable markets:** [UK / Ireland / Nordic — adapt per local regulatory requirements]

---

## Table of Contents

1. [Inquiry Receipt & Triage](#1-inquiry-receipt--triage)
2. [Inquiry Classification](#2-inquiry-classification)
3. [Response Preparation](#3-response-preparation)
4. [Quality Review](#4-quality-review)
5. [Dispatch & Closure](#5-dispatch--closure)
6. [Escalation Pathways](#6-escalation-pathways)
7. [Adverse Event & PQC Identification](#7-adverse-event--pqc-identification)
8. [Documentation Standards](#8-documentation-standards)

---

## 1. Inquiry Receipt & Triage

### Intake Channels

| Channel | System | SLA (Business Hours) |
|---|---|---|
| Phone | IVR / Telephony platform (e.g. Genesys) | Same day |
| Email | CRM (e.g. Salesforce, IRMS) | 24–48 hours |
| Web form | CRM portal | 24–48 hours |
| Written (post/fax) | Manual logging into CRM | 48–72 hours |

### Triage Checklist

- [ ] Confirm caller/sender identity (HCP, patient, caregiver, other)
- [ ] Confirm product name and indication referenced
- [ ] Identify if an **Adverse Event (AE)** or **Product Quality Complaint (PQC)** is present — see [Section 7](#7-adverse-event--pqc-identification)
- [ ] Assign inquiry type (see [Section 2](#2-inquiry-classification))
- [ ] Log all mandatory fields in CRM before proceeding

> ⚠️ **If an AE or PQC is identified at any point in the process, it must be documented and forwarded to Pharmacovigilance / Quality immediately, regardless of whether the MI inquiry is answered.**

---

## 2. Inquiry Classification

### Inquiry Types

| Code | Type | Description | Route |
|---|---|---|---|
| `MI-STD` | Standard MI | Answered by approved SRD or FAQ | 1st line |
| `MI-2L` | 2nd-line / Complex | Requires literature search or clinical interpretation | 2nd line SME |
| `MI-OFF` | Off-label | Query relates to unapproved use | Escalate per SOP |
| `MI-COMP` | Compassionate Use | Patient access / named patient programme | Specialist team |
| `MI-MED` | Medical Emergency | Urgent safety or treatment query | Escalate immediately |

### Line Routing Decision

```
Incoming inquiry
    │
    ├── Is an SRD/FAQ available that fully addresses the query?
    │       └── YES → 1st line response using approved content
    │
    ├── Does the query require clinical interpretation or unapproved use discussion?
    │       └── YES → Route to 2nd line SME
    │
    ├── Is it a named patient / compassionate use request?
    │       └── YES → Route to Compassionate Use team
    │
    └── Is there an immediate patient safety concern?
            └── YES → Escalate as Medical Emergency — notify Medical Affairs
```

---

## 3. Response Preparation

### Using Standard Response Documents (SRDs)

1. Search CRM / content library for applicable SRD using product name + query keyword
2. Confirm SRD is **current** (within validity period) and approved for the requester's market
3. Tailor cover letter to match requester type (HCP vs patient language level)
4. Do **not** modify SRD body content — route to content team if amendment is required
5. Attach relevant prescribing information (SmPC / PIL) where applicable

### 2nd-Line Response Preparation

1. Conduct literature search (PubMed, Embase) using structured search strategy
2. Document search terms and results in CRM
3. Draft response using internal clinical data + published literature
4. Ensure response is factual, balanced, and does not constitute promotional messaging
5. Route for QC review before dispatch (see [Section 4](#4-quality-review))

### Language & Tone Guidelines

| Audience | Guidance |
|---|---|
| HCP | Scientific terminology acceptable; reference data sources; include clinical context |
| Patient / Caregiver | Plain language; avoid jargon; signpost to HCP for clinical decisions |
| All | Non-promotional; balanced; evidence-based; compliant with applicable code (e.g. ABPI, EFPIA) |

---

## 4. Quality Review

### QC Checklist — Before Dispatch

- [ ] Response addresses the specific question asked
- [ ] All factual statements are referenced to approved sources
- [ ] No promotional language or unapproved comparative claims
- [ ] AE/PQC check completed and documented
- [ ] Cover letter matches requester type and market
- [ ] Approved SRD version used (not expired)
- [ ] Response logged in CRM with all mandatory fields completed
- [ ] Local regulatory requirements met (e.g. market-specific disclaimers)

### Quality Escalation

If a quality issue is identified during review:

- Minor (formatting, typo): correct and document in CRM notes
- Significant (factual error, compliance risk): place on hold; notify line manager; do not dispatch
- Systemic (recurring issue with SRD): raise as content update request via content team SOP

---

## 5. Dispatch & Closure

### Dispatch Steps

1. Final check — verify recipient contact details against CRM record
2. Send via appropriate channel (phone callback / email / written)
3. Record dispatch date/time and method in CRM
4. Attach copy of response document to case record
5. Close case in CRM with appropriate closure code

### Case Closure Codes

| Code | Meaning |
|---|---|
| `CLOSED-ANSWERED` | Full response provided |
| `CLOSED-REFERRED` | Directed to HCP / other resource; no clinical response given |
| `CLOSED-AE` | AE/PQC identified; forwarded to PV/Quality; MI response secondary |
| `CLOSED-ESCALATED` | Escalated to 2nd line or Medical Affairs; awaiting follow-up |
| `CLOSED-WITHDRAWN` | Caller withdrew inquiry before response |

---

## 6. Escalation Pathways

```
Standard MI (1st line)
    └── Cannot answer with SRD → 2nd line SME
            └── Requires clinical/regulatory input → Medical Affairs
                    └── Urgent patient safety → CMO / Medical Emergency Protocol

Off-label inquiry
    └── Assess under fair balance / unsolicited request SOP
            └── Escalate to Medical Affairs if any uncertainty

Compassionate Use / Named Patient
    └── Route to specialist access team from point of identification
```

---

## 7. Adverse Event & PQC Identification

> This section applies at every stage of inquiry handling. AE/PQC identification is **mandatory** and cannot be deferred.

### Minimum AE Data Set (to capture and forward to PV)

| Field | Required? |
|---|---|
| Reporter (name, profession, contact) | Yes |
| Patient identifiers (initials, age/DOB, sex) | Yes |
| Suspect product (name, dose, route, batch if available) | Yes |
| Adverse event description | Yes |
| Outcome (ongoing, resolved, unknown) | Yes |

### PQC Indicators

- Complaint about product appearance, odour, colour, packaging
- Suspected counterfeit or tampered product
- Device malfunction (for combination products)

### Reporting Timeline (indicative — verify per local SOP)

| Event Type | Report To | Indicative Timeline |
|---|---|---|
| Serious AE | PV team | As soon as possible, within 24 hours |
| Non-serious AE | PV team | Within 72 hours |
| PQC | Quality / Batch release | Per local quality SOP |

---

## 8. Documentation Standards

### Mandatory CRM Fields

| Field | Notes |
|---|---|
| Date / time of inquiry receipt | In local market time |
| Requester type | HCP, patient, caregiver, other HCP (specify profession) |
| Product name | As per approved label |
| Inquiry verbatim | Record exactly as received — do not paraphrase at intake |
| Inquiry category | See Section 2 |
| AE / PQC flag | Yes / No — mandatory on every record |
| Response method | Phone, email, written |
| SRD reference | Document number and version |
| Case owner | Initials or user ID |
| Closure code | See Section 5 |

### Record Retention

Records must be retained in accordance with local regulatory requirements and company policy. Typically a minimum of **5 years** post product withdrawal from market. Do not delete or archive cases without authorisation from the MI Manager.

---

*Template maintained by MI Operations. For SRD-related queries contact the Medical Content team. For PV reporting queries contact Pharmacovigilance.*
