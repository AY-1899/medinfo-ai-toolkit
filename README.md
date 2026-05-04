# medinfo-ai-toolkit

An open-source toolkit for AI-assisted Medical Information, Pharmacovigilance, and pharmaceutical Quality operations.

Designed to be:
- **Regulatory-aware** — aligned with ICH, EU GVP, ABPI/EFPIA, and GxP frameworks
- **System-agnostic** — adaptable to Salesforce, IRMS, Veeva, and other MI/QMS platforms

---

## MI Workflows

Step-by-step process guides for Medical Information operations.

| File | Description |
|---|---|
| [`workflows/mi-workflow-guide.md`](./workflows/mi-workflow-guide.md) | End-to-end MI inquiry handling — triage, classification, response prep, QC, dispatch |

---

## MI Templates

Document structures ready to fill in.

| File | Description |
|---|---|
| [`templates/srd-template.md`](./templates/srd-template.md) | Standard Response Document structure with document control, key messages, evidence summary, and approval workflow |
| [`templates/pv-icsr-checklist.md`](./templates/pv-icsr-checklist.md) | ICSR processing checklist — validity, triage, data entry, seriousness, causality, narrative authorship, reporting timelines |

---

## AI Prompt Libraries

Modular prompts for AI-assisted MI, PV, and Quality workflows. All prompts use `[VARIABLE]` placeholders and are compatible with Claude, GPT-4, or any instruction-following LLM. AI outputs require human review before use in live operations.

### Medical Information & Pharmacovigilance

| File | Prompts | Use Case |
|---|---|---|
| [`prompt-libraries/prompt-library-hcp-2nd-line.md`](./prompt-libraries/prompt-library-hcp-2nd-line.md) | 7 prompts | Query intake, 2nd-line response drafting, literature summary, SRD gap check, cover letter, QC review, escalation handoff |
| [`prompt-libraries/prompt-library-ae-triage.md`](./prompt-libraries/prompt-library-ae-triage.md) | 8 prompts | AE signal detection, minimum criteria check, data extraction, seriousness assessment, MedDRA coding, narrative drafting, follow-up letters, PV handoff |
| [`prompt-libraries/prompt-library-srd-drafting.md`](./prompt-libraries/prompt-library-srd-drafting.md) | 8 prompts | SRD scoping, evidence synthesis, key messages, summary response, FAQ generation, SRD review, gap analysis, market localisation |

### Quality (GxP)

| File | Prompts | Use Case |
|---|---|---|
| [`quality/prompt-library-capa.md`](./quality/prompt-library-capa.md) | 8 prompts | Deviation intake, 5-Why RCA, Ishikawa RCA, CAPA planning, effectiveness check, risk classification, closure report, regulatory impact assessment |

---

## AI-Powered Tools

Single-file web applications powered by the Claude API. Open in any browser — no installation required.

| Tool | Folder | Description |
|---|---|---|
| [MI Response Drafting Tool](./tool/mi-drafting-tool.html) | `tool/` | 4-step workflow: query intake → SRD gap check → response draft → QC review |
| [Deviation & CAPA Tool](./quality/tools/deviation-capa-tool.html) | `quality/tools/` | 4-step workflow: deviation intake → root cause analysis → CAPA plan → closure report |

> Both tools require an [Anthropic API key](https://console.anthropic.com/). See individual tool READMEs for setup instructions.

---

## Scripts

Python utilities for MI workflow automation. See [`scripts/README.md`](./scripts/README.md) for setup and usage.

| File | Description |
|---|---|
| [`scripts/pubmed_search.py`](./scripts/pubmed_search.py) | Search PubMed by keyword and export results to CSV |
| [`scripts/case_tracker.py`](./scripts/case_tracker.py) | Log, track, and report on MI inquiry cases via command line |
| [`scripts/response_checker.py`](./scripts/response_checker.py) | Scan draft MI responses for compliance and quality issues |

---

## How to Use

Clone or fork this repository and adapt to your organisation's SOPs.

```bash
git clone https://github.com/AY-1899/medinfo-ai-toolkit.git
```

All templates use standard markdown and render on GitHub, Notion, and Confluence. HTML tools open directly in any modern browser.

---

## Disclaimer

See [DISCLAIMER.md](./DISCLAIMER.md) for full terms of use, data privacy guidance, and liability information.

These materials are for **reference and educational purposes only**. They do not replace validated company SOPs, regulatory guidance, or qualified professional review.

---

## Contact

[LinkedIn](https://www.linkedin.com/in/ammar-jawad-b2a373114/)
