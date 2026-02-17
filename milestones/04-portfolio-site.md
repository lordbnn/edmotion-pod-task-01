# Milestone 4: Portfolio Site

**Goal:** Build and deploy a live portfolio website that showcases your data analysis work using GitHub Pages.

**Estimated time:** 90–120 minutes

---

## What Is GitHub Pages?

GitHub Pages turns a repo into a free, live website. Your portfolio will be accessible at:

```
https://YOUR-USERNAME.github.io
```

For data analysts, your portfolio is where you prove that you can take messy data, ask the right questions, and communicate clear answers. The site doesn't need to be flashy — it needs to be clear.

---

## Step 1: Create the Portfolio Repo

1. Go to [github.com/new](https://github.com/new)
2. Name it **exactly**: `YOUR-USERNAME.github.io` (replace with your actual username)
   - Example: if your username is `jane-analytics`, name it `jane-analytics.github.io`
3. Set to **Public**
4. Check **Add a README file**
5. Click **Create repository**

Clone it to your computer:

```bash
git clone https://github.com/YOUR-USERNAME/YOUR-USERNAME.github.io.git
cd YOUR-USERNAME.github.io
```

---

## Step 2: Choose Your Template

We provide two portfolio templates. Pick the one that matches your comfort level:

### Option A: Starter Template
📁 [templates/portfolio-site-starter/index.html](../templates/portfolio-site-starter/index.html)

- Clean, light design on a white background
- Simple HTML and CSS — easy to read and customize
- No JavaScript (except the year in the footer)
- Great if you want to understand every line of code
- **Best for:** Complete beginners or anyone who prefers simplicity

### Option B: Premium Template
📁 [templates/portfolio-site-premium/index.html](../templates/portfolio-site-premium/index.html)

- Dark editorial design with gold accents and custom fonts
- Scroll-triggered animations that reveal sections as you scroll down
- Animated metric counters (projects completed, rows analyzed, etc.)
- Toolkit proficiency bars that fill on scroll
- Alternating project card layouts for visual variety
- Frosted glass navigation bar
- **Best for:** Anyone who wants a portfolio that stands out immediately

> **Which should you pick?** If you're brand new to HTML, start with **Option A** — you can always upgrade to Option B later. If you're comfortable editing HTML or just want the most impressive result, go straight to **Option B**. Both are fully customizable and marked with ✏️ comments showing you what to change.

Copy your chosen template's `index.html` into your portfolio repo and start customizing.

### What to Include on a Data Analyst Portfolio

**Hero Section** — Your name, a one-liner that positions you as an analyst, and a photo or avatar.

> Example: "Data Analyst exploring patterns in business operations and public data using SQL, Python, and Tableau."

**About** — 2-3 sentences about your analytical background, what kinds of problems interest you, and where you're headed. Be specific.

**Projects Section** — This is the centerpiece. For each project, include:
- **Project title** — clear and descriptive
- **One-sentence summary** — what you analyzed and what you found
- **Tools used** — e.g., "Python · pandas · Matplotlib"
- **Link to the repo** — so visitors can see your code and methodology
- **A key visual** — one chart or finding that hooks the reader (save chart images to your portfolio repo)

**Skills / Toolkit** — List your actual tools, grouped by category:
- **Languages:** SQL, Python
- **Visualization:** Tableau, Matplotlib, Seaborn
- **Data Tools:** pandas, Excel, Google Sheets, Jupyter
- **Databases:** PostgreSQL, MySQL, SQLite
- **Other:** Git, Google Colab, Kaggle

**Contact** — Email, LinkedIn, GitHub profile

### What Makes an Analyst Portfolio Stand Out

- **Show the insight, not just the project** — "I found that 60% of returns come from 3 product subcategories" is more compelling than "I analyzed return data"
- **Lead with visuals** — Embed a chart from each project. People skim, and a clean chart stops the scroll.
- **Quality over quantity** — One well-documented analysis beats five sloppy notebooks
- **Clarity is the skill** — An analyst's job is communication. Your portfolio should prove you can explain complex findings simply.

---

## Step 3: Add Project Visuals

For each project you want to showcase:

1. Export your best chart as a PNG from your notebook or tool
2. Save it in your portfolio repo (e.g., create an `images/` folder)
3. Reference it in your HTML:

```html
<img src="images/sales-by-region.png" alt="Sales by Region bar chart">
```

If you used Google Sheets or Tableau, take a clean screenshot of the visualization.

---

## Step 4: Test Locally

Before pushing to GitHub, check your site in a browser:

1. Open the `index.html` file directly in your browser (double-click it or drag into a browser window)
2. Check that everything looks right — text is readable, charts display, links work
3. Test on different screen sizes if you can (press `F12` in your browser → toggle device toolbar)

---

## Step 5: Deploy to GitHub Pages

1. Add, commit, and push your files:

```bash
git add .
git commit -m "Add analyst portfolio site"
git push
```

2. Go to your repo on GitHub
3. Navigate to **Settings → Pages**
4. Under **Source**, select **Deploy from a branch**
5. Choose `main` branch and `/ (root)` folder
6. Click **Save**
7. Wait 1–2 minutes, then visit `https://YOUR-USERNAME.github.io`

Your site is live! 🎉

---

## Step 6: Iterate and Improve

Your first version doesn't need to be perfect. Ship it, then improve.

Ideas for future updates:
- Add a "Currently Learning" or "Currently Exploring" section
- Embed Tableau Public dashboards using iframes
- Add a blog section where you write about your analysis process
- Include a downloadable resume/CV link
- As you complete more projects, add them to the Projects section

---

## Step 7: Connect Everything

Tie your entire GitHub presence together so everything links to everything:

1. **Profile README** → Link to your portfolio site
2. **Portfolio site** → Link to your GitHub profile and each project repo
3. **Project repos** → Reference your portfolio in their READMEs
4. **Pod shared repo** → Share your live site URL
5. **LinkedIn** → Add your portfolio URL to your profile

A hiring manager should be able to start anywhere and find everything.

---

## Step 8: Final Pod Review

This is the big one. Review each pod member's full setup:

1. **Profile** → Does it clearly say "data analyst"? Are tools specific?
2. **Data project** → Is the analysis question clear? Are findings specific with numbers? Could you reproduce it?
3. **Portfolio site** → Does it load? Does it showcase analysis work with visuals? Is it easy to navigate?
4. Open an Issue on their fork of this task repo:
   - Title: `EdMotion Final Pod Review - [Your Name]`
   - Cover all four milestones
   - Highlight strengths and areas for growth

---

## ✅ Milestone 4 Checklist

- [ ] Portfolio repo created as `YOUR-USERNAME.github.io`
- [ ] Site includes: hero, about, projects (with visuals), skills/toolkit, and contact
- [ ] Projects section highlights findings and links to repos
- [ ] At least one chart or visualization embedded on the site
- [ ] Skills section lists specific tools grouped by category
- [ ] Site tested locally before deployment
- [ ] GitHub Pages enabled and site is live
- [ ] Profile README links to portfolio site
- [ ] Portfolio site links back to GitHub profile and project repos
- [ ] Shared live URL with the pod
- [ ] Completed final pod review for at least 2 members

---

## 🏆 Task Complete!

If you've checked everything off across all four milestones, you've successfully:

- Set up a professional GitHub presence positioned for data analytics
- Learned Git basics (clone, commit, push, fork)
- Published a complete data exploration with proper structure
- Built and deployed a live analyst portfolio
- Practiced peer review and collaboration with your pod

**You shipped real analysis to a live site. That's more than most aspiring analysts ever do. Keep building.**
