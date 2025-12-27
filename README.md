# Arnaud Bougaham - Resume Website

Personal resume website built with Hugo and PaperMod theme, hosted on GitHub Pages.

## 🚀 Quick Start

### Prerequisites

- [Hugo Extended](https://gohugo.io/getting-started/installing/) (latest version)
- Git

### Local Development

1. **Clone the repository**:
   ```bash
   git clone https://github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
   cd ArnaudBougaham.github.io
   ```

2. **Initialize submodules** (to get the PaperMod theme):
   ```bash
   git submodule update --init --recursive
   ```

3. **Run Hugo locally**:
   ```powershell
   # Windows (manual installation)
   C:\Users\arb\Hugo\hugo.exe server -D
   ```
   
   Or if Hugo is in your PATH:
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
   - `content/awards.md` - Awards and recognition
   - `content/skills.md` - Skills
   - `content/certifications.md` - Licenses and certifications

### Current Theme: PaperMod

This site uses [PaperMod](https://github.com/adityatelange/hugo-PaperMod), a fast, clean, responsive Hugo theme with:
- Dark mode enabled by default
- Profile mode for homepage
- Modern navigation menu
- Social icons support
- Responsive design

### Theme Configuration

Key settings in `config.toml`:
- `theme = "PaperMod"`
- `defaultTheme = "dark"` (dark mode by default)
- Profile mode enabled with 400x400px profile picture
- Navigation menu: Home, Experience, Education, Publications, Awards, Skills, Certifications

## 🌐 Deployment to GitHub Pages

### Automatic Deployment (Already Configured)

This repository is configured with **GitHub Actions** for automatic deployment. The workflow file is located at `.github/workflows/gh-pages.yml`.

#### How It Works

1. **Push your changes**:
   ```bash
   git add .
   git commit -m "Update content"
   git push origin main
   ```

2. **GitHub Actions automatically**:
   - Triggers on every push to the `main` branch
   - Checks out your repository and submodules (including the PaperMod theme)
   - Sets up Hugo Extended (latest version)
   - Builds your site with `hugo --minify` (production mode)
   - Uploads the built site to GitHub Pages
   - Deploys to https://ArnaudBougaham.github.io

3. **Deployment Time**: Usually takes 1-3 minutes after pushing

#### Checking Deployment Status

1. Go to your repository: https://github.com/ArnaudBougaham/ArnaudBougaham.github.io
2. Click the **"Actions"** tab
3. You'll see a list of workflow runs
4. Click on the latest run to see detailed logs
5. A green checkmark ✅ means deployment succeeded
6. A red X ❌ means there was an error (check the logs)

#### What Gets Deployed

The workflow builds your site and deploys:
- All content files (`.md` files from `content/`)
- All static assets (images, CSS, etc.)
- The built HTML/CSS/JS files
- Theme files (PaperMod)

### Initial Setup

If setting up for the first time:

1. **Create Personal Access Token**:
   - Go to: https://github.com/settings/tokens
   - Click "Generate new token (classic)"
   - Name it (e.g., "GitHub Pages Deployment")
   - Select scopes: `repo` and `workflow` (both required!)
   - Generate and copy the token

2. **Push to GitHub**:
   ```bash
   git remote add origin https://YOUR_TOKEN@github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Under "Source", select **"GitHub Actions"** (not "Deploy from a branch")
   - Save

### Workflow File Details

The GitHub Actions workflow (`.github/workflows/gh-pages.yml`) performs these steps:

1. **Checkout**: Gets your code and theme submodules
2. **Setup Hugo**: Installs Hugo Extended (required for image processing)
3. **Setup Pages**: Configures GitHub Pages environment
4. **Build**: Runs `hugo --minify` to generate optimized static files
5. **Upload**: Uploads the `public/` directory as an artifact
6. **Deploy**: Deploys the artifact to GitHub Pages

### Troubleshooting Deployment

- **Build fails**: Check the Actions tab for error messages, usually related to:
  - Syntax errors in `config.toml`
  - Missing files or broken links
  - Theme submodule issues
- **Site not updating**: Wait a few minutes, clear browser cache, or check Actions tab
- **Authentication errors**: Ensure your Personal Access Token has `workflow` scope

## 📚 Resources

- [Hugo Documentation](https://gohugo.io/documentation/)
- [PaperMod Theme Wiki](https://github.com/adityatelange/hugo-PaperMod/wiki)
- [GitHub Pages Documentation](https://docs.github.com/en/pages)
- [Hugo Themes](https://themes.gohugo.io/)

## 💡 Tips

- **Free Hosting**: GitHub Pages is completely free for public repositories
- **Custom Domain**: You can add a custom domain in GitHub Pages settings
- **Automatic Updates**: With GitHub Actions, every push automatically rebuilds and deploys your site
- **Version Control**: All your content is version-controlled with Git
- **Local Testing**: Always test locally with `hugo server -D` before pushing changes

## 🎨 Site Features

- **Theme**: PaperMod (modern, fast, clean)
- **Default Mode**: Dark mode
- **Navigation**: Home, Experience, Education, Publications, Awards, Skills, Certifications
- **Social Icons**: GitHub, LinkedIn, Email, ORCID, Research Portal
- **Profile Mode**: Enabled with large profile picture

---

**Live Site**: https://ArnaudBougaham.github.io
