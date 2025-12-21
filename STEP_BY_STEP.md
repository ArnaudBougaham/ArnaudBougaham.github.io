# 🚀 Step-by-Step Guide: Get Your Resume Site Live

Follow these steps in order to test locally first, then deploy online.

---

## 📋 Prerequisites Checklist

Before starting, make sure you have:
- [ ] Git installed ([Download Git](https://git-scm.com/downloads))
- [ ] A GitHub account ([Sign up](https://github.com/signup) if needed)
- [ ] Your profile photo ready (optional for testing, but recommended)

---

## STEP 1: Install Hugo Extended ⚙️

### Windows (Recommended: Chocolatey)
```powershell
# If you have Chocolatey installed:
choco install hugo-extended
```

### Windows (Manual Installation)
1. Go to: https://github.com/gohugoio/hugo/releases
2. Download the latest `hugo_extended_X.X.X_windows-amd64.zip`
3. Extract the ZIP file
4. Add Hugo to your PATH:
   - Copy `hugo.exe` to a folder (e.g., `C:\Hugo\bin`)
   - Add that folder to your Windows PATH environment variable
   - Or just run Hugo from that folder

### Verify Installation
```powershell
hugo version
```
You should see something like: `hugo v0.120.0+extended`

**✅ Checkpoint**: Hugo is installed and working

---

## STEP 2: Add Your Profile Photo 📸

1. **Find your profile photo** (professional headshot recommended)
2. **Copy it** to: `C:\Users\arb\hugo-resume-site\static\images\photos\`
3. **Rename it** to: `profile.jpg` (or `profile.png`)

**Note**: If you don't have a photo yet, you can skip this and add it later. The site will still work.

**✅ Checkpoint**: Photo is in place (or you'll add it later)

---

## STEP 3: Choose and Add a Hugo Theme 🎨

You need to add a Hugo theme. Here are 3 great options:

### Option A: hugo-resume (Best for Resumes) ⭐ RECOMMENDED
```powershell
cd C:\Users\arb\hugo-resume-site
git init
git submodule add -b main https://github.com/eddiewebb/hugo-resume.git themes/hugo-resume
```

### Option B: hugo-theme-codex (Minimalist & Clean)
```powershell
cd C:\Users\arb\hugo-resume-site
git init
git submodule add -b main https://github.com/jakewies/hugo-theme-codex.git themes/hugo-resume
```

### Option C: hugo-resume-theme (Modern Design)
```powershell
cd C:\Users\arb\hugo-resume-site
git init
git submodule add -b main https://github.com/ojroques/hugo-resume-theme.git themes/hugo-resume
```

**Important**: 
- The theme name in `config.toml` is set to `hugo-resume`
- Make sure your submodule uses that directory name, OR update `config.toml` line 4 to match your theme name

**✅ Checkpoint**: Theme is added as a submodule

---

## STEP 4: Test Locally (View Before Going Online) 🖥️

### Start the Hugo Server
```powershell
cd C:\Users\arb\hugo-resume-site
hugo server -D
```

You should see:
```
Web Server is available at http://localhost:1313/
```

### View Your Site
1. Open your web browser
2. Go to: **http://localhost:1313/**
3. You should see your resume site!

### What to Check:
- [ ] Site loads without errors
- [ ] Your profile photo appears (if you added one)
- [ ] All sections are visible (About, Experience, Education, etc.)
- [ ] Navigation menu works
- [ ] Content looks good

### Make Adjustments
- Edit files in `content/` folder
- Changes appear automatically (Hugo auto-reloads)
- Refresh browser to see updates

### Stop the Server
Press `Ctrl + C` in the terminal when done testing.

**✅ Checkpoint**: Site looks good locally, ready to deploy!

---

## STEP 5: Create GitHub Repository 📦

### 5.1 Create the Repository
1. Go to: https://github.com/new
2. **Repository name**: `ArnaudBougaham.github.io` (must match exactly!)
3. **Visibility**: Select **Public** (required for free GitHub Pages)
4. **DO NOT** check:
   - ❌ Add a README file
   - ❌ Add .gitignore
   - ❌ Choose a license
5. Click **"Create repository"**

### 5.2 Push Your Code to GitHub
```powershell
cd C:\Users\arb\hugo-resume-site

# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Hugo resume site"

# Add remote (replace with your GitHub username if different)
git remote add origin https://github.com/ArnaudBougaham/ArnaudBougaham.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Note**: You'll be asked for your GitHub username and password (or use a Personal Access Token)

**✅ Checkpoint**: Code is on GitHub

---

## STEP 6: Enable GitHub Pages (Make It Live Online) 🌐

### 6.1 Enable GitHub Pages
1. Go to your repository: https://github.com/ArnaudBougaham/ArnaudBougaham.github.io
2. Click **Settings** (top menu)
3. Click **Pages** (left sidebar)
4. Under **"Source"**, select: **"GitHub Actions"**
5. Click **Save**

### 6.2 Wait for Deployment
- GitHub Actions will automatically build your site
- This takes 1-3 minutes
- You can watch the progress: Click **Actions** tab in your repository

### 6.3 Your Site is Live! 🎉
Visit: **https://ArnaudBougaham.github.io**

**✅ Checkpoint**: Site is live online!

---

## STEP 7: Future Updates (Making Changes) 🔄

Whenever you want to update your site:

```powershell
cd C:\Users\arb\hugo-resume-site

# Make your changes (edit files, add photos, etc.)

# Test locally first
hugo server -D

# When ready, commit and push
git add .
git commit -m "Update resume content"
git push
```

GitHub Actions will automatically rebuild and deploy your site!

---

## 🆘 Troubleshooting

### Hugo not found
- Make sure Hugo is in your PATH, or run it from the installation folder
- Verify with: `hugo version`

### Theme not showing
- Make sure you added the theme as a submodule
- Check that `theme = "hugo-resume"` in `config.toml` matches your theme folder name
- Try: `git submodule update --init --recursive`

### Site not building on GitHub
- Check the **Actions** tab for error messages
- Make sure you selected "GitHub Actions" as the source (not "Deploy from a branch")
- Verify your `config.toml` has no syntax errors

### Images not showing
- Make sure photos are in `static/images/photos/`
- Check file names match exactly (case-sensitive)
- Verify file paths in `config.toml` and content files

---

## 📝 Quick Reference

| Step | Command | What It Does |
|------|---------|--------------|
| Test locally | `hugo server -D` | View site at localhost:1313 |
| Build site | `hugo` | Generate static files in `public/` |
| Add theme | `git submodule add <theme-url> themes/hugo-resume` | Add Hugo theme |
| Push changes | `git add . && git commit -m "msg" && git push` | Update live site |

---

## ✅ Final Checklist

Before going live, make sure:
- [ ] Hugo is installed and working
- [ ] Theme is added
- [ ] Profile photo is added (optional)
- [ ] Site looks good locally (`hugo server -D`)
- [ ] GitHub repository is created
- [ ] Code is pushed to GitHub
- [ ] GitHub Pages is enabled with "GitHub Actions"
- [ ] Site is live at https://ArnaudBougaham.github.io

---

**🎉 Congratulations!** Your professional resume site is now live!

**Need help?** Check the `README.md` and `SETUP.md` files for more details.

