# 🚀 Quick Setup Guide

## Step 1: Install Hugo

**Windows (Manual Installation - No PATH Required)**:
1. Go to: https://github.com/gohugoio/hugo/releases
2. Download the latest `hugo_extended_X.X.X_windows-amd64.zip`
3. Extract and copy `hugo.exe` to a folder (e.g., `C:\Users\arb\Hugo`)
4. Use the full path to run Hugo: `C:\Users\arb\Hugo\hugo.exe`

**Note**: Replace `C:\Users\arb\Hugo` with your Hugo installation folder.

## Step 2: Add PaperMod Theme

This site uses the **PaperMod** theme:

```powershell
cd C:\Users\arb\hugo-resume-site
git init
git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
```

## Step 3: Add Profile Photo

1. Copy your profile photo to: `static/images/photos/profile.jpg`
2. Also copy it to: `assets/img/avatar.png` (for PaperMod theme)

## Step 4: Test Locally

```powershell
C:\Users\arb\Hugo\hugo.exe server -D
```

Visit http://localhost:1313 to see your site!

## Step 5: Deploy to GitHub Pages (FREE!)

1. **Create GitHub Repository**:
   - Go to https://github.com/new
   - Repository name: `ArnaudBougaham.github.io`
   - Make it **PUBLIC** (required for free hosting)
   - **DO NOT** initialize with README, .gitignore, or license

2. **Create Personal Access Token**:
   - Go to: https://github.com/settings/tokens
   - Generate new token (classic) with `repo` and `workflow` scopes
   - Copy the token

3. **Push Your Code**:
   ```powershell
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://YOUR_TOKEN@github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
   git push -u origin main
   ```
   Replace `YOUR_TOKEN` with your Personal Access Token.

4. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click **Settings** → **Pages**
   - Under **Source**, select **"GitHub Actions"**
   - Save

5. **Wait 1-2 minutes**, then visit: **https://ArnaudBougaham.github.io**

## Step 6: Customize

- Edit `config.toml` for site settings
- Edit files in `content/` for your information
- Current theme: **PaperMod** (modern, fast, with dark mode default)

## 🎉 That's it!

Your resume site is now live and will automatically update whenever you push changes to GitHub!
