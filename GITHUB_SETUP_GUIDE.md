# GitHub Setup and Upload Guide

## Prerequisites
- GitHub account (create at https://github.com if you don't have one)
- Git installed on your computer (download from https://git-scm.com)

## Option 1: Upload via GitHub Website (Easiest)

### Step 1: Create a New Repository on GitHub
1. Go to https://github.com
2. Click the **+** icon in the top right
3. Select **"New repository"**
4. Fill in the details:
   - **Repository name:** `uk-household-expenditure-analysis-2019-2024`
   - **Description:** "Time series analysis of UK household spending patterns before, during, and after COVID-19 pandemic"
   - **Visibility:** Choose Public or Private
   - **DO NOT** initialize with README (we already have one)
5. Click **"Create repository"**

### Step 2: Upload Files
1. On the repository page, click **"uploading an existing file"**
2. Drag and drop all folders from this project:
   - data/
   - raw_data/
   - powerbi/
   - reports/
   - documentation/
   - README.md
   - .gitignore

3. Add a commit message: "Initial commit - UK household expenditure analysis project"
4. Click **"Commit changes"**

## Option 2: Using Git Command Line (Recommended for Developers)

### Step 1: Initialize Git Repository
Open terminal/command prompt and navigate to your project folder:

```bash
cd /path/to/household-expenditure-analysis
git init
git add .
git commit -m "Initial commit - UK household expenditure analysis project"
```

### Step 2: Connect to GitHub
Create a new repository on GitHub (as in Option 1, Step 1), then:

```bash
git remote add origin https://github.com/YOUR_USERNAME/uk-household-expenditure-analysis-2019-2024.git
git branch -M main
git push -u origin main
```

Replace `YOUR_USERNAME` with your GitHub username.

## Option 3: Using GitHub Desktop (User-Friendly GUI)

### Step 1: Install GitHub Desktop
1. Download from https://desktop.github.com
2. Install and sign in with your GitHub account

### Step 2: Publish Repository
1. Open GitHub Desktop
2. Click **File → Add Local Repository**
3. Browse to your project folder
4. Click **"Create a repository instead"**
5. Fill in:
   - **Name:** uk-household-expenditure-analysis-2019-2024
   - **Description:** Time series analysis of UK household spending patterns
   - Check "Initialize with README" = NO (we already have one)
6. Click **"Publish repository"**
7. Choose visibility (Public/Private)
8. Click **"Publish repository"**

## Important Notes

### File Size Considerations
⚠️ GitHub has a 100MB file size limit per file. If any of your files exceed this:
- Use Git Large File Storage (Git LFS) - see instructions below
- Or store large files elsewhere (OneDrive, Google Drive) and link in README

### Git LFS Setup (if needed for large files)
```bash
git lfs install
git lfs track "*.pbix"
git lfs track "*.xlsx"
git add .gitattributes
git commit -m "Add Git LFS tracking"
git push
```

### Recommended Repository Structure
Your repository will look like this on GitHub:
```
uk-household-expenditure-analysis-2019-2024/
├── README.md                    ← Main documentation
├── .gitignore                   ← Files to exclude from Git
├── data/                        ← Processed data
├── raw_data/                    ← Original ONS data
├── powerbi/                     ← Dashboard files
├── reports/                     ← Academic papers/reports
└── documentation/               ← Additional docs
```

## After Upload: Enhance Your Repository

### Add Topics/Tags
On your GitHub repository page:
1. Click the gear icon next to "About"
2. Add topics: `data-analysis`, `time-series`, `covid-19`, `household-expenditure`, `power-bi`, `uk-data`, `ons-data`

### Create Releases (Optional)
Mark significant versions:
1. Go to "Releases" tab
2. Click "Create a new release"
3. Tag: `v1.0` - Description: "Initial analysis submission"

### Enable GitHub Pages (Optional)
If you want to host documentation online:
1. Go to Settings → Pages
2. Select branch: `main`, folder: `/docs`
3. Your README will be visible at: `https://YOUR_USERNAME.github.io/uk-household-expenditure-analysis-2019-2024/`

## Troubleshooting

### "File too large" error
- Use Git LFS (see above)
- Or exclude large files in .gitignore and store elsewhere

### "Repository already exists" error
- Use a different repository name
- Or delete the existing repository and try again

### Authentication issues
- Use Personal Access Token instead of password
- Generate at: Settings → Developer settings → Personal access tokens

## Need Help?
- GitHub documentation: https://docs.github.com
- Git handbook: https://guides.github.com/introduction/git-handbook/

---

**Recommended Repository Name:**
`uk-household-expenditure-analysis-2019-2024`

**Recommended Repository Description:**
"Time series analysis of UK household spending patterns (2019-2024) examining COVID-19 pandemic impact using ONS data and Power BI visualization"

**Recommended Topics:**
`data-analysis`, `time-series`, `covid-19`, `household-expenditure`, `power-bi`, `data-visualization`, `uk-statistics`, `ons-data`, `academic-research`
