# Arnaud Bougaham - Resume Website

Personal resume website built with Hugo and hosted on GitHub Pages.

## 🚀 Quick Start

### Prerequisites

- [Hugo Extended](https://gohugo.io/getting-started/installing/) (latest version)
- Git

### Local Development

1. **Clone the repository** (after pushing to GitHub):
   ```bash
   git clone https://github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
   cd ArnaudBougaham.github.io
   ```

2. **Add a Hugo Resume theme** (choose one):
   
   Option A - hugo-resume (recommended for resumes):
   ```bash
   git submodule add -b main https://github.com/eddiewebb/hugo-resume.git themes/hugo-resume
   ```
   
   Option B - hugo-theme-codex (minimalist):
   ```bash
   git submodule add -b main https://github.com/jakewies/hugo-theme-codex.git themes/hugo-resume
   ```
   
   Option C - hugo-resume-theme (modern):
   ```bash
   git submodule add -b main https://github.com/ojroques/hugo-resume-theme.git themes/hugo-resume
   ```

3. **Run Hugo locally**:
   ```bash
   hugo server -D
   ```

4. **View your site**: Open http://localhost:1313 in your browser

## 📝 Customization

### Update Your Information

1. **Edit `config.toml`**: Update your personal information, social links, and site settings
2. **Edit content files**: Modify the Markdown files in the `content/` directory:
   - `content/_index.md` - Homepage/About section
   - `content/experience.md` - Work experience
   - `content/education.md` - Education background
   - `content/publications.md` - Publications and projects

### Change Theme

1. Find a Hugo theme you like at [Hugo Themes](https://themes.gohugo.io/)
2. Add it as a submodule:
   ```bash
   git submodule add <theme-repo-url> themes/<theme-name>
   ```
3. Update `theme = "theme-name"` in `config.toml`

## 🌐 Deployment to GitHub Pages (FREE!)

### Automatic Deployment (Recommended)

This repository is already configured with GitHub Actions for automatic deployment:

1. **Create the repository** on GitHub:
   - Repository name: `ArnaudBougaham.github.io`
   - Make it **public** (required for free GitHub Pages)
   - **Do NOT** initialize with README, .gitignore, or license

2. **Push your code**:
   ```bash
   git init
   git add .
   git commit -m "Initial commit"
   git branch -M main
   git remote add origin https://github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to your repository settings on GitHub
   - Navigate to **"Pages"** in the left sidebar
   - Under **"Source"**, select **"GitHub Actions"**
   - The site will be automatically built and deployed on every push

4. **Your site will be live at**: `https://ArnaudBougaham.github.io` (usually takes 1-2 minutes)

### Manual Deployment (Alternative)

If you prefer manual deployment:

1. Build the site:
   ```bash
   hugo
   ```

2. Push the `public` folder to the `gh-pages` branch:
   ```bash
   cd public
   git init
   git add .
   git commit -m "Deploy site"
   git branch -M gh-pages
   git remote add origin https://github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
   git push -u origin gh-pages
   ```

## 🎨 Popular Hugo Resume Themes

- **[hugo-resume](https://github.com/eddiewebb/hugo-resume)** - Clean, professional resume theme
- **[hugo-theme-codex](https://github.com/jakewies/hugo-theme-codex)** - Minimalist blog/resume theme
- **[hugo-resume-theme](https://github.com/ojroques/hugo-resume-theme)** - Modern resume theme
- **[hugo-theme-stack](https://github.com/CaiJimmy/hugo-theme-stack)** - Feature-rich theme

## 📚 Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Hugo Themes](https://themes.gohugo.io/)

## 💡 Tips

- **Free Hosting**: GitHub Pages is completely free for public repositories
- **Custom Domain**: You can add a custom domain (like `arnaudbougaham.io`) in GitHub Pages settings
- **Automatic Updates**: With GitHub Actions, every push automatically rebuilds and deploys your site
- **Version Control**: All your content is version-controlled with Git

---

**Note**: Remember to add your chosen theme as a Git submodule before deploying!

