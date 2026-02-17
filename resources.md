# Resources

A curated list of datasets, tools, tutorials, and troubleshooting tips for data analysts.

---

## Datasets to Explore

### Beginner-Friendly
- [Kaggle Datasets](https://www.kaggle.com/datasets) — Thousands of free datasets with community notebooks for inspiration
- [Superstore Dataset](https://www.kaggle.com/datasets/vivek468/superstore-dataset-final) — Classic business analytics dataset
- [World Happiness Report](https://www.kaggle.com/datasets/unsdsn/world-happiness) — Country-level data, great for comparisons
- [Google Dataset Search](https://datasetsearch.research.google.com/) — Search engine for datasets

### Nigeria / Africa Focused
- [Nigeria Data Portal](https://nigeria.opendataforafrica.org/) — Economic, demographic, and social data
- [Lagos State Open Data](https://data.lagosstate.gov.ng/) — Local government data
- [Africa Open Data](https://africaopendata.org/) — Pan-African datasets
- [World Bank Open Data — Nigeria](https://data.worldbank.org/country/nigeria) — Development indicators

### Real-World Practice
- [FiveThirtyEight Data](https://github.com/fivethirtyeight/data) — The data behind their articles
- [Our World in Data](https://github.com/owid/owid-datasets) — Global development datasets
- [UCI Machine Learning Repository](https://archive.ics.uci.edu/) — Classic datasets used in research

---

## Tools Setup Guides

### Python & Jupyter
- [Install Anaconda](https://docs.anaconda.com/anaconda/install/) — Installs Python, Jupyter, pandas, and more in one go (recommended for beginners)
- [Google Colab](https://colab.research.google.com/) — Free Jupyter notebooks in your browser, no install needed
- [Jupyter Notebook Beginner Guide](https://realpython.com/jupyter-notebook-introduction/) — How to use notebooks effectively

### SQL Practice
- [SQLite Online](https://sqliteonline.com/) — Run SQL queries in your browser
- [Mode Analytics SQL Tutorial](https://mode.com/sql-tutorial/) — Learn SQL with real data
- [LeetCode SQL](https://leetcode.com/problemset/database/) — Practice SQL problems

### Visualization
- [Tableau Public](https://public.tableau.com/) — Free version of Tableau, publish dashboards online
- [Matplotlib Cheatsheet](https://matplotlib.org/cheatsheets/) — Quick reference for Python plotting
- [Seaborn Gallery](https://seaborn.pydata.org/examples/index.html) — Visual examples of every chart type

---

## Git & GitHub

- [GitHub Docs: Hello World](https://docs.github.com/en/get-started/start-your-journey/hello-world) — Official beginner guide
- [Git Cheat Sheet (PDF)](https://education.github.com/git-cheat-sheet-education.pdf) — Print this out
- [GitHub Skills](https://skills.github.com/) — Free interactive courses

### Common Git Commands

```bash
git clone <url>          # Download a repo to your computer
git status               # See what's changed
git add .                # Stage all changes
git commit -m "message"  # Save changes with a description
git push                 # Upload changes to GitHub
git pull                 # Download latest changes from GitHub
git log --oneline        # See your commit history
```

---

## Markdown

- [Markdown Guide — Basic Syntax](https://www.markdownguide.org/basic-syntax/) — Everything you need
- [GitHub Flavored Markdown Spec](https://github.github.com/gfm/) — GitHub's specific flavor

---

## HTML & CSS (for Portfolio Site)

- [MDN Web Docs: HTML Basics](https://developer.mozilla.org/en-US/docs/Learn/Getting_started_with_the_web/HTML_basics)
- [MDN Web Docs: CSS First Steps](https://developer.mozilla.org/en-US/docs/Learn/CSS/First_steps)
- [GitHub Pages Quickstart](https://docs.github.com/en/pages/quickstart)

---

## Analyst Portfolio Inspiration

- Search GitHub for `data-analyst-portfolio` to see how others structure theirs
- Browse [Kaggle Notebooks](https://www.kaggle.com/code) to see how analysts present analysis
- Look at [Tableau Public Gallery](https://public.tableau.com/app/discover) for dashboard inspiration

---

## Troubleshooting

### "Permission denied" when pushing
You likely need to set up authentication. GitHub no longer accepts passwords.
1. **HTTPS with Personal Access Token:** GitHub → Settings → Developer Settings → Personal Access Tokens → Generate new token. Use this as your password when pushing.
2. **SSH Key:** Follow [GitHub's SSH setup guide](https://docs.github.com/en/authentication/connecting-to-github-with-ssh).

### My GitHub Pages site isn't showing up
- Make sure the repo name is exactly `YOUR-USERNAME.github.io`
- Check that you have an `index.html` file in the root of the repo
- Go to repo Settings → Pages and confirm the source is set to `main` branch
- Wait 2-5 minutes — it can take a moment to deploy
- Hard refresh your browser (Ctrl+Shift+R or Cmd+Shift+R)

### Jupyter notebook won't render on GitHub
- Large notebooks sometimes fail to render. Keep notebooks under 10MB.
- Use `nbconvert` to export to HTML as a backup: `jupyter nbconvert --to html notebook.ipynb`
- Consider using [nbviewer.org](https://nbviewer.org/) — paste your notebook URL and it renders reliably.

### My CSV file is too big for GitHub
- GitHub warns on files over 50MB and blocks files over 100MB
- For large datasets, add the file to `.gitignore` and include download instructions in your README instead
- Or use a sample/subset of the data and note this in your documentation

### "Fatal: not a git repository"
You're in the wrong folder. Navigate to your project:
```bash
cd my-data-project
```

### I made a mistake in my last commit message
```bash
git commit --amend -m "New corrected message"
git push --force
```
⚠️ Only use `--force` on your own repos, never on shared repos.

---

## Need Help?

1. **Ask your pod first** — someone might have hit the same issue
2. **Search the error message** — paste it into Google exactly as it appears
3. **Stack Overflow** — Search for your specific error
4. **Kaggle Forums** — Great for data-specific questions
5. **GitHub Community Forum** — [github.community](https://github.community)
