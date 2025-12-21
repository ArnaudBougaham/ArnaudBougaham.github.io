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

### Windows (Manual Installation - No PATH Required)

1. **Download Hugo Extended**:
   - Go to: https://github.com/gohugoio/hugo/releases
   - Download the latest `hugo_extended_X.X.X_windows-amd64.zip` file

2. **Extract Hugo**:
   - Extract the ZIP file
   - Copy `hugo.exe` to a folder you can access (e.g., `C:\Users\arb\Hugo`)

3. **Verify Installation**:
   ```powershell
   C:\Users\arb\Hugo\hugo.exe version
   ```
   You should see something like: `hugo v0.153.1+extended`

**Note**: If you put Hugo in a different folder, replace `C:\Users\arb\Hugo` with your folder path in all commands below.

**✅ Checkpoint**: Hugo is installed and working

---

## STEP 2: Add Your Profile Photo 📸

1. **Find your profile photo** (professional headshot recommended)
2. **Copy it** to: `C:\Users\arb\hugo-resume-site\static\images\photos\profile.jpg`
3. **Also copy it** to: `C:\Users\arb\hugo-resume-site\assets\img\avatar.png` (for PaperMod theme)

**Note**: If you don't have a photo yet, you can skip this and add it later. The site will still work.

**✅ Checkpoint**: Photo is in place (or you'll add it later)

---

## STEP 3: Add PaperMod Theme 🎨

This site uses the **PaperMod** theme - a modern, fast, and clean Hugo theme.

```powershell
cd C:\Users\arb\hugo-resume-site
git init
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

**✅ Checkpoint**: Theme is added as a submodule

---

## STEP 4: Test Locally (View Before Going Online) 🖥️

### Start the Hugo Server
```powershell
cd C:\Users\arb\hugo-resume-site
C:\Users\arb\Hugo\hugo.exe server -D
```

You should see:
```
Web Server is available at http://localhost:1313/
```

### View Your Site
1. Open your web browser
2. Go to: **http://localhost:1313/**
3. You should see your resume site with PaperMod theme!

### What to Check:
- [ ] Site loads without errors
- [ ] Your profile photo appears (if you added one)
- [ ] All sections are visible (Home, Experience, Education, Publications, Awards, Skills, Certifications)
- [ ] Navigation menu works
- [ ] Dark mode is enabled by default
- [ ] Social icons appear (GitHub, LinkedIn, Email, ORCID, Research Portal)
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

### 5.2 Create Personal Access Token
GitHub requires a Personal Access Token (not password) for authentication:

1. Go to: https://github.com/settings/tokens
2. Click **"Generate new token"** → **"Generate new token (classic)"**
3. Name it (e.g., "Hugo Site Deploy")
4. Select these scopes:
   - ✅ `repo` (full control of private repositories)
   - ✅ `workflow` (Update GitHub Action workflows)
5. Click **"Generate token"**
6. **Copy the token immediately** (you won't see it again!)

### 5.3 Push Your Code to GitHub
```powershell
cd C:\Users\arb\hugo-resume-site

# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit
git commit -m "Initial commit: Hugo resume site with PaperMod theme"

# Add remote with your token (replace YOUR_TOKEN with your actual token)
git remote add origin https://YOUR_TOKEN@github.com/ArnaudBougaham/ArnaudBougaham.github.io.git

# Push to GitHub
git branch -M main
git push -u origin main
```

**Note**: If the repository already exists and has content, you may need to pull first:
```powershell
git pull origin main --allow-unrelated-histories
git push -u origin main
```

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
- If no workflow runs automatically, click **"Run workflow"** to trigger it manually

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
C:\Users\arb\Hugo\hugo.exe server -D

# When ready, commit and push
git add .
git commit -m "Update resume content"
git push
```

GitHub Actions will automatically rebuild and deploy your site!

---

## 🆘 Troubleshooting

### Hugo not found
- If you installed Hugo manually, use the full path: `C:\Users\arb\Hugo\hugo.exe server -D`
- Replace `C:\Users\arb\Hugo` with wherever you installed Hugo
- Verify with: `C:\Users\arb\Hugo\hugo.exe version`

### Theme not showing
- Make sure you added the theme as a submodule
- Check that `theme = "PaperMod"` in `config.toml` matches your theme folder name
- Try: `git submodule update --init --recursive`

### Site not building on GitHub
- Check the **Actions** tab for error messages
- Make sure you selected "GitHub Actions" as the source (not "Deploy from a branch")
- Verify your `config.toml` has no syntax errors
- Ensure your Personal Access Token has `workflow` scope

### Images not showing
- Make sure photos are in `static/images/photos/` for content
- Profile photo should also be in `assets/img/avatar.png` for PaperMod theme
- Check file names match exactly (case-sensitive)
- Verify file paths in `config.toml` and content files

### Authentication errors
- Make sure your Personal Access Token has both `repo` and `workflow` scopes
- Update the remote URL with your token: `git remote set-url origin https://YOUR_TOKEN@github.com/ArnaudBougaham/ArnaudBougaham.github.io.git`

---

## 📝 Quick Reference

| Step | Command | What It Does |
|------|---------|--------------|
| Test locally | `C:\Users\arb\Hugo\hugo.exe server -D` | View site at localhost:1313 |
| Build site | `C:\Users\arb\Hugo\hugo.exe` | Generate static files in `public/` |
| Add theme | `git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod` | Add PaperMod theme |
| Push changes | `git add . && git commit -m "msg" && git push` | Update live site |

---

## ✅ Final Checklist

Before going live, make sure:
- [ ] Hugo is installed and working
- [ ] PaperMod theme is added
- [ ] Profile photo is added (optional)
- [ ] Site looks good locally (`C:\Users\arb\Hugo\hugo.exe server -D`)
- [ ] GitHub repository is created
- [ ] Personal Access Token is created with `repo` and `workflow` scopes
- [ ] Code is pushed to GitHub
- [ ] GitHub Pages is enabled with "GitHub Actions"
- [ ] Site is live at https://ArnaudBougaham.github.io

---

## 🎨 Current Site Features

- **Theme**: PaperMod (modern, fast, clean)
- **Default Mode**: Dark mode
- **Navigation Menu**: Home, Experience, Education, Publications, Awards, Skills, Certifications
- **Social Icons**: GitHub, LinkedIn, Email, ORCID, Research Portal
- **Profile Mode**: Enabled with large profile picture (400x400px)

---

**🎉 Congratulations!** Your professional resume site is now live!

**Need help?** Check the `README.md` and `SETUP.md` files for more details.
