# Experiment 1: Git & GitHub Pages Setup

## Objective
Set up a GitHub repository for a project, create branches, merge changes, and use GitHub Pages for hosting a simple static site.

---

## Step-by-Step Git Workflow & Commands

### 1. Initialize Local Repository
```bash
git init
git checkout -b main
```

### 2. Stage and Make the Initial Commit
```bash
git add .
git commit -m "feat: initial commit with experiment catalog and root portal"
```

### 3. Link Remote GitHub Repository
```bash
git remote add origin https://github.com/kavya141106/<your-repo-name>.git
```

### 4. Create and Work in a Feature Branch
```bash
# Create and switch to a development branch
git checkout -b feature/experiments-setup

# Add any additional changes
git status
git add .
git commit -m "feat: complete experiments 1 through 8 implementation"
```

### 5. Merge Branch Back into Main
```bash
# Switch back to the main branch
git checkout main

# Merge feature branch
git merge feature/experiments-setup

# Verify clean merge
git log --oneline -n 3
```

### 6. Push Changes to Remote GitHub Repository
```bash
git push -u origin main
```

---

## Hosting via GitHub Pages

1. Open your repository on GitHub: `https://github.com/kavya141106/<your-repo-name>`
2. Click on **Settings** tab (gear icon at top).
3. In the left navigation sidebar under "Code and automation", click **Pages**.
4. Under **Build and deployment**:
   - **Source**: Select `Deploy from a branch`.
   - **Branch**: Select `main` and set folder to `/ (root)`.
   - Click **Save**.
5. Wait 1–2 minutes. Refresh the settings page until you see:
   > *Your site is live at `https://kavya141106.github.io/<your-repo-name>/`*
