# ⚡ Quick Start Checklist

**Follow these steps in order. Test locally FIRST, then deploy online.**

---

## ✅ STEP 1: Install Hugo
- [ ] Download Hugo Extended from: https://gohugo.io/getting-started/installing/
- [ ] Extract to a folder (e.g., `C:\Users\arb\Hugo`)
- [ ] Verify: Run `C:\Users\arb\Hugo\hugo.exe version` in PowerShell

## ✅ STEP 2: Add Your Photo (Optional)
- [ ] Copy your profile photo to: `static/images/photos/profile.jpg`
- [ ] Also copy to: `assets/img/avatar.png` (for PaperMod theme)

## ✅ STEP 3: Add PaperMod Theme
- [ ] Run this command:
  ```powershell
  cd C:\Users\arb\hugo-resume-site
  git init
  git submodule add https://github.com/adityatelange/hugo-PaperMod.git themes/PaperMod
  ```

## ✅ STEP 4: Test Locally (IMPORTANT - Do This First!)
- [ ] Run: `C:\Users\arb\Hugo\hugo.exe server -D`
- [ ] Open: http://localhost:1313
- [ ] Check: Site looks good? All content visible? Dark mode working?
- [ ] Press `Ctrl+C` to stop when done

## ✅ STEP 5: Create GitHub Repository
- [ ] Go to: https://github.com/new
- [ ] Name: `ArnaudBougaham.github.io` (exact match!)
- [ ] Make it **Public**
- [ ] **Don't** add README, .gitignore, or license
- [ ] Click "Create repository"

## ✅ STEP 6: Create Personal Access Token
- [ ] Go to: https://github.com/settings/tokens
- [ ] Generate new token (classic) with `repo` and `workflow` scopes
- [ ] Copy the token

## ✅ STEP 7: Push to GitHub
- [ ] Run these commands (replace YOUR_TOKEN with your token):
  ```powershell
  cd C:\Users\arb\hugo-resume-site
  git add .
  git commit -m "Initial commit"
  git branch -M main
  git remote add origin https://YOUR_TOKEN@github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
  git push -u origin main
  ```

## ✅ STEP 8: Enable GitHub Pages
- [ ] Go to your repo: https://github.com/ArnaudBougaham/ArnaudBougaham.github.io
- [ ] Click **Settings** → **Pages**
- [ ] Source: Select **"GitHub Actions"**
- [ ] If workflow doesn't run, go to **Actions** tab and click **"Run workflow"**
- [ ] Wait 1-2 minutes
- [ ] Visit: **https://ArnaudBougaham.github.io**

---

## 🎉 Done!

Your resume site is now live!

**For detailed instructions, see:** `STEP_BY_STEP.md`
