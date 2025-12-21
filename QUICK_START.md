# ⚡ Quick Start Checklist

**Follow these steps in order. Test locally FIRST, then deploy online.**

---

## ✅ STEP 1: Install Hugo
- [ ] Download Hugo Extended from: https://gohugo.io/getting-started/installing/
- [ ] Extract to a folder (e.g., `C:\Users\arb\Hugo`)
- [ ] Verify: Run `C:\Users\arb\Hugo\hugo.exe version` in PowerShell

## ✅ STEP 2: Add Your Photo (Optional)
- [ ] Copy your profile photo to: `static/images/photos/profile.jpg`

## ✅ STEP 3: Add Theme
- [ ] Run this command:
  ```powershell
  cd C:\Users\arb\hugo-resume-site
  git init
  git submodule add -b master https://github.com/eddiewebb/hugo-resume.git themes/hugo-resume
  ```

## ✅ STEP 4: Test Locally (IMPORTANT - Do This First!)
- [ ] Run: `C:\Users\arb\Hugo\hugo.exe server -D`
- [ ] Open: http://localhost:1313
- [ ] Check: Site looks good? All content visible?
- [ ] Press `Ctrl+C` to stop when done

## ✅ STEP 5: Create GitHub Repository
- [ ] Go to: https://github.com/new
- [ ] Name: `ArnaudBougaham.github.io` (exact match!)
- [ ] Make it **Public**
- [ ] **Don't** add README, .gitignore, or license
- [ ] Click "Create repository"

## ✅ STEP 6: Push to GitHub
- [ ] Run these commands:
  ```powershell
  cd C:\Users\arb\hugo-resume-site
  git add .
  git commit -m "Initial commit"
  git branch -M main
  git remote add origin https://github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
  git push -u origin main
  ```

## ✅ STEP 7: Enable GitHub Pages
- [ ] Go to your repo: https://github.com/ArnaudBougaham/ArnaudBougaham.github.io
- [ ] Click **Settings** → **Pages**
- [ ] Source: Select **"GitHub Actions"**
- [ ] Wait 1-2 minutes
- [ ] Visit: **https://ArnaudBougaham.github.io**

---

## 🎉 Done!

Your resume site is now live!

**For detailed instructions, see:** `STEP_BY_STEP.md`

