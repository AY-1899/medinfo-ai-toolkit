# Automation Scripts

Simple Python utilities for Medical Information workflows.
Each script is heavily commented and written to be readable by non-developers.

---

## Scripts

### 1. `pubmed_search.py` — PubMed Literature Search

Search PubMed for clinical papers and save results to a CSV file.

**What it does:**
- Takes a search term (e.g. `osimertinib renal impairment`)
- Queries the NCBI PubMed API (free, no account needed)
- Returns title, authors, journal, year, abstract, and direct link for each result
- Saves results to a CSV you can open in Excel

**Setup (one-time):**
```bash
pip install requests
```

**Run:**
```bash
python pubmed_search.py
```

---

### 2. `case_tracker.py` — MI Case Log

A command-line tool for logging and tracking Medical Information inquiry cases. Cases are stored in a local CSV file (`mi_cases.csv`) that can also be opened in Excel.

**What it does:**
- Log new cases with product, query topic, reporter type, AE flag, and status
- View open cases and all cases
- Update case status and notes
- Generate a summary report (case counts by category and product)
- Auto-flags AE cases with a reminder to notify Pharmacovigilance

**Setup:**
No installation needed — uses Python's built-in libraries only.

**Run:**
```bash
python case_tracker.py
```

---

### 3. `response_checker.py` — MI Response Quality Checker

A pre-review screening tool that scans a draft MI response for common compliance and quality issues.

**What it checks:**
| Check | Type |
|---|---|
| AE reporting reminder present | ❌ Missing (blocks dispatch) |
| Promotional language | ⚠️ Warning |
| Source references present | ⚠️ Warning |
| Off-label content signals | ⚠️ Warning |
| Comparative claims | ⚠️ Warning |
| Absolute / overconfident language | ℹ️ Note |
| Word count (too short / too long) | ℹ️ Note |
| SmPC / prescribing information referenced | ℹ️ Note |
| Standard MI closing line present | ℹ️ Note |

**Setup:**
No installation needed.

**Run (interactive — paste text when prompted):**
```bash
python response_checker.py
```

**Run (pass a text file directly):**
```bash
python response_checker.py my_response.txt
```

---

## Requirements

| Script | External libraries needed | Install command |
|---|---|---|
| `pubmed_search.py` | `requests` | `pip install requests` |
| `case_tracker.py` | None | — |
| `response_checker.py` | None | — |

Python 3.7 or higher required for all scripts.

---

## Disclaimer

These scripts are tools to support MI workflows — they do not replace qualified human review. `response_checker.py` flags potential issues; it cannot assess clinical accuracy. `pubmed_search.py` returns publicly available literature; relevance and quality assessment must be performed by a Medical Information professional.
