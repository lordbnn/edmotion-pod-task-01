# Milestone 3: First Data Project

**Goal:** Publish a complete data exploration project with a clean, professional repo structure that another analyst could follow.

**Estimated time:** 90–120 minutes

---

## Why This Matters

This is the milestone that separates analysts who *talk* about data from analysts who *show* their work. A well-structured data project repo tells a hiring manager three things: you can find a question worth asking, you can work through data methodically, and you can communicate what you found.

---

## Step 1: Choose a Dataset

Pick a dataset that interests you. Keep it manageable — this is about structure and process, not building something massive.

**Option A: Global Superstore Sales** (Business Analytics)
A classic dataset with orders, products, customers, and regions. Great for practicing segmentation, trend analysis, and basic KPIs.
- Available at: [Kaggle — Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final)

**Option B: World Happiness Report** (Public Data)
Country-level data on happiness scores and contributing factors. Great for comparisons, rankings, and correlation analysis.
- Available at: [Kaggle — World Happiness Report](https://www.kaggle.com/datasets/unsdsn/world-happiness)

**Option C: Lagos / Nigeria Open Data** (Local Focus)
Public datasets on population, budgets, infrastructure, or education from Nigerian open data portals.
- Explore: [Nigeria Data Portal](https://nigeria.opendataforafrica.org/) or [Lagos State Government Open Data](https://data.lagosstate.gov.ng/)

**Option D: Your Own Dataset**
Any clean CSV you find interesting. Aim for 500–10,000 rows with at least 6–8 columns.

> **Tip:** Don't spend more than 15 minutes choosing. The dataset doesn't matter nearly as much as what you do with it.

---

## Step 2: Create the Repo

1. Go to [github.com/new](https://github.com/new)
2. Name it clearly (e.g., `superstore-sales-analysis`, `world-happiness-exploration`, `lagos-budget-analysis`)
3. Add a description (e.g., "Exploratory data analysis of global superstore sales data")
4. Set to **Public**
5. Check **Add a README file**
6. Select **Add .gitignore** → choose `Python`
7. Select a **License** → MIT
8. Click **Create repository**

---

## Step 3: Set Up the Data Project Structure

Clone the repo and organize it. This is the standard structure for a data analysis project:

```
my-data-project/
├── README.md              # Project overview, question, findings, how to reproduce
├── LICENSE
├── .gitignore
├── data/
│   ├── raw/               # Original untouched data files
│   │   └── dataset.csv
│   └── cleaned/           # Processed/cleaned versions
│       └── dataset_clean.csv
├── notebooks/             # Jupyter notebooks (your analysis lives here)
│   └── 01-exploration.ipynb
├── output/                # Charts, tables, exports
│   ├── chart-sales-by-region.png
│   └── summary-table.csv
└── docs/                  # Extra notes, data dictionary, methodology
    └── data-dictionary.md
```

Create the folders:

```bash
cd my-data-project
mkdir -p data/raw data/cleaned notebooks output docs
```

### Why This Structure?

- **`data/raw/`** — Never modify raw data. Keep the original untouched so anyone can reproduce your work.
- **`data/cleaned/`** — Your processed version goes here. Separating raw from clean is an industry best practice.
- **`notebooks/`** — Your Jupyter notebooks are numbered to show the order of analysis.
- **`output/`** — Save charts and summary tables here so the README can reference them.
- **`docs/`** — Data dictionaries, notes on methodology, and any context someone would need.

---

## Step 4: Do the Analysis

You have two paths depending on your current tools:

### Path A: Jupyter Notebook (Python)
If you have Python and Jupyter installed (or use [Google Colab](https://colab.research.google.com) for free):

1. Create a notebook in `notebooks/01-exploration.ipynb`
2. Walk through these steps in the notebook:

```
1. LOAD — Import the data and preview it
2. CLEAN — Handle missing values, fix data types, rename columns
3. EXPLORE — Summary statistics, distributions, groupings
4. VISUALIZE — 3-5 charts that reveal patterns
5. FINDINGS — Write 3-5 key takeaways in markdown cells
```

Useful starter code:
```python
import pandas as pd
import matplotlib.pyplot as plt
import seaborn as sns

# Load data
df = pd.read_csv('../data/raw/dataset.csv')

# Preview
print(df.shape)
df.head()
df.info()
df.describe()
```

### Path B: Spreadsheet + Markdown (Excel / Google Sheets)
If you're more comfortable in spreadsheets, that's completely valid:

1. Do your analysis in Excel or Google Sheets
2. Export key charts as images → save to `output/`
3. Write up your findings in a Markdown file in `notebooks/analysis-notes.md`
4. Export your cleaned data as CSV → save to `data/cleaned/`

Either path is fine. What matters is the structure, the documentation, and the thinking.

---

## Step 5: Write a Data Project README

This is what separates good analyst repos from mediocre ones. Your README should walk someone through your entire analysis without them needing to open a single file.

### Required Sections

```markdown
# [Project Title]

[One-sentence summary of what you analyzed and what you found.]

## Question

[What question were you trying to answer? Be specific.]

Example: "Which product categories and regions drive the most profit
for the Superstore, and where are we losing money?"

## Dataset

- **Source:** [Where the data came from, with link]
- **Size:** [X rows × Y columns]
- **Time period:** [If applicable]
- **Key fields:** [List the most important columns and what they mean]

## Tools Used

- Python (pandas, matplotlib, seaborn)
- Jupyter Notebook
- [Or: Google Sheets, Excel, etc.]

## Key Findings

1. [Finding 1 — specific, with numbers]
2. [Finding 2 — specific, with numbers]
3. [Finding 3 — specific, with numbers]

## Visualizations

![Chart Title](output/chart-name.png)

[Brief explanation of what the chart shows and why it matters.]

## How to Reproduce

1. Clone this repo
2. Install requirements: `pip install pandas matplotlib seaborn`
3. Open `notebooks/01-exploration.ipynb`
4. Run all cells

## What I'd Do Next

- [Further analysis you'd do with more time]
- [Questions this analysis raised]
```

### What Makes a Great Data README

- **Lead with the finding, not the process** — "Region X accounts for 40% of losses" is better than "First I loaded the data, then I cleaned it..."
- **Include actual numbers** — Vague findings like "sales vary by region" say nothing
- **Show your charts** — Save visualizations to `output/` and embed them in the README
- **Be transparent about limitations** — What's missing from the data? What assumptions did you make?

---

## Step 6: Make Commits That Tell the Analysis Story

Don't dump everything in one commit. Commit at each stage of your analysis:

### Good Data Project Commits
```
Add raw dataset and data dictionary
Set up project folder structure
Clean data: handle missing values and fix date column
Add exploratory analysis notebook
Create sales by region visualization
Add key findings to README
```

### Bad Commits
```
stuff
update
fixed it
added everything
```

Aim for **at least 6 commits** that mirror your analysis workflow.

---

## Step 7: Pod Collaboration

1. Add a link to your project repo in your pod's shared repo
2. Review a pod member's data project. Open an Issue with:
   - Title: `EdMotion Pod Review: Data Project - [Your Name]`
   - Is the analysis question clear?
   - Can you follow the logic from question → data → findings?
   - Are the findings specific (with numbers) or vague?
   - Could you reproduce the analysis from the README?
   - One strength and one suggestion

---

## ✅ Milestone 3 Checklist

- [ ] Data project repo created with clear name and description
- [ ] Proper data project folder structure (`data/raw`, `data/cleaned`, `notebooks`, `output`, `docs`)
- [ ] Raw data preserved separately from cleaned data
- [ ] Analysis completed (notebook or spreadsheet + writeup)
- [ ] At least 3 visualizations saved to `output/`
- [ ] README includes: question, dataset, tools, findings (with numbers), and reproduction steps
- [ ] At least 6 meaningful commits that mirror the analysis workflow
- [ ] .gitignore and LICENSE files included
- [ ] Shared project link with the pod
- [ ] Reviewed at least one pod member's data project

---

**Up next:** [Milestone 4: Portfolio Site →](04-portfolio-site.md)
