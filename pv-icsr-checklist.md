# Pharmacovigilance ICSR Processing Checklist

> **Template version:** 1.0  
> **Scope:** Individual Case Safety Report (ICSR) intake, triage, processing, and narrative authorship  
> **Applicable regulations:** ICH E2B(R3), EU GVP Module VI, MHRA Yellow Card guidance

---

## Table of Contents

1. [Minimum Criteria for Validity](#1-minimum-criteria-for-validity)
2. [Case Receipt & Initial Triage](#2-case-receipt--initial-triage)
3. [Case Classification](#3-case-classification)
4. [Data Entry Checklist](#4-data-entry-checklist)
5. [Seriousness Assessment](#5-seriousness-assessment)
6. [Causality Assessment](#6-causality-assessment)
7. [Narrative Authorship Checklist](#7-narrative-authorship-checklist)
8. [Reporting Timelines](#8-reporting-timelines)
9. [Follow-up Management](#9-follow-up-management)
10. [Quality Control Before Submission](#10-quality-control-before-submission)

---

## 1. Minimum Criteria for Validity

An ICSR is valid and must be processed if **all four** of the following are present:

| Criterion | Present? | Notes |
|---|---|---|
| **1. Identifiable reporter** | ☐ Yes / ☐ No | Name, initials, or contact detail sufficient |
| **2. Identifiable patient** | ☐ Yes / ☐ No | Initials, age, sex, case reference — any identifier |
| **3. Suspect medicinal product** | ☐ Yes / ☐ No | Product name or description |
| **4. Adverse event / outcome** | ☐ Yes / ☐ No | Any undesirable medical occurrence described |

> ⚠️ If any of the four criteria is absent, attempt follow-up **before** determining the case is invalid. Document all follow-up attempts in the safety database.

---

## 2. Case Receipt & Initial Triage

### Source Identification

- [ ] Identify source type:
  - ☐ Spontaneous (HCP, patient, consumer, pharmacist)
  - ☐ Literature (published case report / observational study)
  - ☐ Clinical trial (refer to trial-specific SAE SOP)
  - ☐ Regulatory authority (forwarded report)
  - ☐ Business partner / licence partner
  - ☐ Digital / social media

- [ ] Record **date of receipt** (Day 0 for reporting clock)
- [ ] Assign unique case reference number in safety database
- [ ] Determine initial/follow-up status:
  - ☐ **Initial report** — first notification of this event for this patient
  - ☐ **Follow-up** — additional information to an existing case (link to parent case)
  - ☐ **Duplicate** — same event from same source (do not create new case; document and close)

### Duplicate Check

Before creating a new case, search the database for:
- Same reporter + same patient + same suspect product + same event
- Same case reference from a licence partner or regulatory authority

---

## 3. Case Classification

### Seriousness (see [Section 5](#5-seriousness-assessment) for criteria)

- [ ] Serious
- [ ] Non-serious

### Expectedness

| Assessment | Basis |
|---|---|
| **Expected (labelled)** | Event is listed in the current Company Core Safety Information (CCSI) / SmPC Section 4.8 |
| **Unexpected (unlabelled)** | Event is **not** listed, or listed at a less specific level, or listed with less severity |

- [ ] Expected
- [ ] Unexpected — note: unexpected serious ADRs have expedited reporting requirements

### Listedness Reference Document

> Document which version of the CCSI / SmPC / RSI was used for expectedness determination:

| Field | Entry |
|---|---|
| Document name | |
| Version / date | |
| Section reviewed | 4.8 / CCSI equivalent |

---

## 4. Data Entry Checklist

### Reporter Information

- [ ] Reporter type (physician, pharmacist, nurse, patient, other)
- [ ] Reporter name or identifier
- [ ] Institution / country
- [ ] Contact details (for follow-up if needed)
- [ ] Reporter's own causality assessment (if provided)

### Patient Information

- [ ] Patient identifier (initials and/or patient number)
- [ ] Age or date of birth
- [ ] Sex
- [ ] Weight / height (if provided and relevant)
- [ ] Relevant medical history and concomitant conditions
- [ ] Concomitant medications (with dose, route, dates)

### Suspect Product(s)

- [ ] Product name (brand and/or INN)
- [ ] Indication for use
- [ ] Dose, route, frequency
- [ ] Start date / stop date
- [ ] Batch number (if available — especially relevant for PQCs and biologics)
- [ ] Action taken (none / dose reduced / drug withdrawn / dose increased / unknown)
- [ ] Re-challenge information (if applicable)

### Adverse Event(s)

- [ ] Event description in verbatim (as reported by the reporter — do not recode at intake)
- [ ] MedDRA PT coding (LLT → PT → HLT → HLGT → SOC)
- [ ] Event onset date
- [ ] Event end date / duration
- [ ] Outcome at time of report:
  - ☐ Recovered / resolved
  - ☐ Recovering / resolving
  - ☐ Not recovered / not resolved
  - ☐ Recovered with sequelae
  - ☐ Fatal
  - ☐ Unknown
- [ ] If fatal: date of death; autopsy performed (yes / no / unknown); cause of death

### Relevant Tests & Lab Values

- [ ] Relevant lab results with dates and normal ranges
- [ ] Relevant diagnostic procedures / imaging
- [ ] Any other clinically relevant information provided

---

## 5. Seriousness Assessment

An adverse event is **serious** if it meets **one or more** of the following ICH E2A criteria:

| Criterion | Met? |
|---|---|
| Results in **death** | ☐ Yes / ☐ No |
| Is **life-threatening** (patient at immediate risk of death at time of event) | ☐ Yes / ☐ No |
| Requires **inpatient hospitalisation** or **prolongation** of existing hospitalisation | ☐ Yes / ☐ No |
| Results in **persistent or significant disability / incapacity** | ☐ Yes / ☐ No |
| Is a **congenital anomaly / birth defect** | ☐ Yes / ☐ No |
| Is an **important medical event** (may jeopardise patient; may require intervention to prevent above outcomes) | ☐ Yes / ☐ No |

> **Important:** "Important medical event" requires medical judgement. If unsure, escalate to the medical assessor.

---

## 6. Causality Assessment

### Assessment Scales

Causality is typically assessed using the **WHO-UMC scale** or the company's own methodology. Document which scale was used.

| WHO-UMC Term | Criteria Summary |
|---|---|
| **Certain** | Plausible time relationship; confirmed on dechallenge; no alternative explanation |
| **Probable / Likely** | Plausible time relationship; confirmed on dechallenge; alternative explanation unlikely |
| **Possible** | Plausible time relationship; but could also be explained by disease or other drugs |
| **Unlikely** | Plausible time relationship improbable; other explanation more convincing |
| **Conditional / Unclassified** | More data needed |
| **Unassessable / Unclassifiable** | Insufficient or contradictory information; cannot be assessed |

### Causality Entry

- [ ] Company causality assessment recorded
- [ ] Reporter's causality assessment recorded (if provided — must not be altered)
- [ ] Basis for company assessment documented in case notes

---

## 7. Narrative Authorship Checklist

The case narrative must be a **coherent, factual, chronological summary** of the case. It is not an interpretation — it is a structured retelling of what was reported.

### Narrative Structure

```
PATIENT BACKGROUND → RELEVANT HISTORY → SUSPECT PRODUCT(S) 
→ EVENT ONSET & DESCRIPTION → MANAGEMENT & TREATMENT 
→ OUTCOME → FOLLOW-UP INFORMATION (if applicable)
```

### Pre-writing Checklist

- [ ] All four minimum criteria confirmed
- [ ] MedDRA coding completed and reviewed
- [ ] Seriousness and expectedness assessed
- [ ] All data entry fields complete (see Section 4)

### Narrative Content Checklist

- [ ] Case reference number and report date included
- [ ] Reporter type and country identified (do not include identifying details if anonymisation required)
- [ ] Patient demographics (age, sex, weight if relevant) included
- [ ] Relevant medical history included
- [ ] All suspect and concomitant medications listed with dose, route, dates
- [ ] Indication for suspect product stated
- [ ] Event onset date (or time to onset from drug start) included
- [ ] Event described in clinical terms — verbatim retained in separate field; MedDRA PT in narrative
- [ ] Treatment / management of the event described
- [ ] Outcome stated clearly
- [ ] Lab / test values included with units and normal ranges
- [ ] Dechallenge / rechallenge information included if applicable
- [ ] Cause of death (if fatal) included
- [ ] Reporter's causality included
- [ ] Missing information clearly flagged (e.g. "batch number not provided"; "outcome unknown at time of report")

### Narrative Quality Standards

- [ ] Written in past tense, third person
- [ ] No speculation or interpretation — only what was reported
- [ ] No copy-paste of verbatim text from reporter without medical review
- [ ] Abbreviations defined on first use
- [ ] Dates in consistent format (DD-MMM-YYYY recommended)
- [ ] No promotional language
- [ ] Narrative is self-contained — a reader should be able to understand the case without reference to individual data fields

---

## 8. Reporting Timelines

> Timelines below are indicative under EU GVP / MHRA guidance. Always verify against your company SOP and applicable regulatory agency requirements.

| Case Type | Regulatory Reporting Timeline |
|---|---|
| **Serious, unexpected, suspected ADR** (SUSAR) | **7 calendar days** (life-threatening / fatal); **15 calendar days** (other serious unexpected) |
| **Serious, expected ADR** | **15 calendar days** |
| **Non-serious ADR** | Periodic (PSUR / PBRER) |
| **Serious ADR from literature** | **15 calendar days** from date of awareness |
| **Pregnancy exposure** | Per company SOP; expedited if serious outcome |

### Internal Escalation Timelines (indicative)

| Milestone | Target |
|---|---|
| Initial data entry complete | Day 0 + 2 |
| Medical assessment complete | Day 0 + 5 |
| QC review complete | Day 0 + 7 |
| Submission to regulatory authority | Per table above |

---

## 9. Follow-up Management

### When to Request Follow-up

- [ ] Minimum validity criteria partially met (missing patient or reporter identifier)
- [ ] Key clinical details absent (onset date, outcome, dose)
- [ ] Batch number missing for a biologic or quality complaint case
- [ ] Pregnancy outcome unknown
- [ ] Outcome listed as "unknown" or "ongoing" at time of initial report

### Follow-up Documentation

- [ ] Date of follow-up attempt recorded in database
- [ ] Method of follow-up (phone / email / letter) recorded
- [ ] Response received — update case and re-assess
- [ ] No response after [X] attempts — document and close follow-up per SOP

---

## 10. Quality Control Before Submission

### Final QC Checklist

- [ ] All four minimum validity criteria confirmed
- [ ] Case classification (serious / non-serious; expected / unexpected) confirmed and documented
- [ ] MedDRA coding reviewed — PT selected reflects event as described
- [ ] Narrative reviewed by a second reviewer (mandatory for serious cases)
- [ ] Reporter and company causality assessments both recorded
- [ ] Reporting timeline met or escalated if at risk
- [ ] No patient-identifiable data in fields that will be transmitted unmasked
- [ ] Relevant attachments (source documents, medical records if provided) linked to case
- [ ] Submission-ready status confirmed in database
- [ ] Case locked / frozen per database SOP before submission

---

## Reference Documents

| Document | Source |
|---|---|
| ICH E2A: Clinical Safety Data Management | [ICH website](https://www.ich.org) |
| ICH E2B(R3): Electronic Transmission of ICSRs | [ICH website](https://www.ich.org) |
| EU GVP Module VI: Management and Reporting of Adverse Reactions | [EMA website](https://www.ema.europa.eu) |
| MedDRA Browser | [MedDRA MSSO](https://www.meddra.org) |
| WHO-UMC Causality Assessment | [WHO-UMC website](https://www.who-umc.org) |
| MHRA Yellow Card guidance (UK) | [MHRA website](https://yellowcard.mhra.gov.uk) |

---

*Template for educational and workflow reference purposes. Always follow your organisation's validated SOPs and local regulatory requirements for live case processing.*
