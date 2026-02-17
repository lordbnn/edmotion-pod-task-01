# Milestone 1: GitHub Setup

**Goal:** Create your GitHub account, install Git, and make your first fork.

**Estimated time:** 30–45 minutes

---

## Why GitHub Matters for Data Analysts

You might be thinking "I'm an analyst, not a developer — why do I need GitHub?" Here's why:

- **Reproducibility** — GitHub lets others (and future you) re-run your analyses
- **Portfolio proof** — Saying "I know SQL and Python" means nothing without evidence. GitHub is that evidence.
- **Collaboration** — Real data teams use version control. This is how analysts work with engineers, other analysts, and stakeholders.
- **Career leverage** — Hiring managers increasingly check GitHub profiles when evaluating analysts

---

## Step 1: Create a GitHub Account

1. Go to [github.com](https://github.com)
2. Click **Sign Up**
3. Choose a professional username — this becomes part of your public identity
   - ✅ Good: `jane-analytics`, `marcus-data`, `aisha-analyst`
   - ❌ Avoid: `xXx_gangsta_xXx`, `throwaway123`
4. Use a real email you check regularly
5. Complete the setup and verify your email

### Quick Wins After Signup
- [ ] Add a profile photo (a real photo or clean avatar)
- [ ] Add your name
- [ ] Add a short bio (e.g., "Data Analyst | SQL · Python · Tableau")
- [ ] Set your location (optional but adds credibility)

---

## Step 2: Install Git on Your Computer

Git is the tool that connects your computer to GitHub.

### Windows
1. Download Git from [git-scm.com/download/win](https://git-scm.com/download/win)
2. Run the installer — accept all default settings
3. Open **Git Bash** (it installs with Git)
4. Type `git --version` and press Enter. You should see a version number.

### Mac
1. Open **Terminal** (search for it in Spotlight)
2. Type `git --version` and press Enter
3. If it's not installed, you'll be prompted to install Xcode Command Line Tools — say yes
4. Run `git --version` again to confirm

### Chromebook / Linux
1. Open **Terminal**
2. Run: `sudo apt-get install git`
3. Confirm with `git --version`

### Configure Git
Run these two commands in your terminal (replace with your info):

```bash
git config --global user.name "Your Name"
git config --global user.email "your-email@example.com"
```

Use the **same email** you signed up to GitHub with.

---

## Step 3: Fork This Repo

"Forking" makes a personal copy of this repo under your GitHub account.

1. Go to this repo's page on GitHub
2. Click the **Fork** button (top right)
3. Select your account as the destination
4. You now have your own copy at `github.com/YOUR-USERNAME/edmotion-pod-task-01`

---

## Step 4: Clone Your Fork to Your Computer

"Cloning" downloads your fork so you can work on it locally.

1. On your forked repo page, click the green **Code** button
2. Copy the HTTPS URL
3. Open your terminal and navigate to where you want the project:

```bash
cd Desktop
```

4. Clone it:

```bash
git clone https://github.com/YOUR-USERNAME/edmotion-pod-task-01.git
```

5. Move into the folder:

```bash
cd edmotion-pod-task-01
```

You're in! 🎉

---

## Step 5: Set Up Your Pod's Shared Repo

One person in the pod should do this:

1. Go to [github.com/new](https://github.com/new)
2. Name it something like `edmotion-pod-alpha` or `edmotion-pod-01` (your pod decides)
3. Check **Add a README file**
4. Click **Create repository**
5. Go to **Settings → Collaborators → Add people**
6. Invite every pod member by their GitHub username

Everyone else:
1. Accept the invitation (check your email or GitHub notifications)
2. Clone the shared repo to your computer too

---

## ✅ Milestone 1 Checklist

- [ ] GitHub account created with professional username
- [ ] Profile photo and bio added (mention data/analytics in bio)
- [ ] Git installed and configured on my computer
- [ ] This repo forked to my account
- [ ] Fork cloned to my computer
- [ ] Pod shared repo created (or invitation accepted)
- [ ] Shared repo cloned to my computer

---

**Up next:** [Milestone 2: Profile README →](02-profile-readme.md)
