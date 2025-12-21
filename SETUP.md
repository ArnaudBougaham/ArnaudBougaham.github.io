# 🚀 Quick Setup Guide

## Step 1: Install Hugo

**Windows (Manual Installation)**:
1. Go to: https://github.com/gohugoio/hugo/releases
2. Download the latest `hugo_extended_X.X.X_windows-amd64.zip`
3. Extract and copy `hugo.exe` to a folder (e.g., `C:\Users\arb\Hugo`)
4. Use the full path to run Hugo: `C:\Users\arb\Hugo\hugo.exe`

**Note**: Replace `C:\Users\arb\Hugo` with your Hugo installation folder.

## Step 2: Choose and Add a Theme

You need to add a Hugo theme. Here are recommended options:

### Option A: hugo-resume (Best for Resumes)
```powershell
git submodule add -b master https://github.com/eddiewebb/hugo-resume.git themes/hugo-resume
```

### Option B: hugo-theme-codex (Minimalist)
```powershell
git submodule add -b main https://github.com/jakewies/hugo-theme-codex.git themes/hugo-resume
```

### Option C: hugo-resume-theme (Modern)
```powershell
git submodule add -b main https://github.com/ojroques/hugo-resume-theme.git themes/hugo-resume
```

**Note**: The theme name in `config.toml` is set to `hugo-resume`, so make sure your submodule uses that directory name, or update `config.toml` to match.

## Step 3: Test Locally

```powershell
C:\Users\arb\Hugo\hugo.exe server -D
```

Visit http://localhost:1313 to see your site!

## Step 4: Deploy to GitHub Pages (FREE!)

1. **Create GitHub Repository**:
   - Go to https://github.com/new
   - Repository name: `ArnaudBougaham.github.io`
   - Make it **PUBLIC** (required for free hosting)
   - **DO NOT** initialize with README, .gitignore, or license

2. **Push Your Code**:
   ```powershell
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to your repository on GitHub
   - Click **Settings** → **Pages**
   - Under **Source**, select **"GitHub Actions"**
   - Save

4. **Wait 1-2 minutes**, then visit: **https://ArnaudBougaham.github.io**

## Step 5: Customize

- Edit `config.toml` for site settings
- Edit files in `content/` for your information
- Each theme has different customization options - check the theme's documentation

## 🎉 That's it!

Your resume site is now live and will automatically update whenever you push changes to GitHub!

