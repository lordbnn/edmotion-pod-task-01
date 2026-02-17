# Data Dictionary Template

Copy this into your data project's `docs/` folder and fill it in. A data dictionary documents every column in your dataset so anyone (including future you) can understand the data without guessing.

---

## Dataset: [Dataset Name]

**Source:** [Where you got the data — link to original source]
**Downloaded:** [Date you downloaded it]
**File:** `data/raw/[filename.csv]`
**Rows:** [Number of rows]
**Columns:** [Number of columns]

---

## Column Definitions

| Column Name | Data Type | Description | Example Value | Notes |
|-------------|-----------|-------------|---------------|-------|
| `column_1` | string | [What this column represents] | "Example" | |
| `column_2` | integer | [What this column represents] | 42 | |
| `column_3` | float | [What this column represents] | 19.99 | Currency in USD |
| `column_4` | date | [What this column represents] | 2024-01-15 | Format: YYYY-MM-DD |
| `column_5` | string | [What this column represents] | "Category A" | Possible values: A, B, C |

---

## Data Quality Notes

- **Missing values:** [Which columns have missing data? How many? How did you handle them?]
- **Duplicates:** [Did you find any duplicate rows? What did you do?]
- **Assumptions:** [Any assumptions you made about the data?]
- **Limitations:** [What's NOT in this data that would be useful?]

---

## Changes Made During Cleaning

1. [What you changed and why — e.g., "Removed 12 rows with null values in the revenue column"]
2. [Another change]
3. [Another change]

Cleaned file saved to: `data/cleaned/[filename_clean.csv]`
