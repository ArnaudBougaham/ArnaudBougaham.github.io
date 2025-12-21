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

This repository is configured with GitHub Actions for automatic deployment:

1. **Push your changes**:
   ```bash
   git add .
   git commit -m "Update content"
   git push
   ```

2. **GitHub Actions automatically**:
   - Builds your Hugo site
   - Deploys to GitHub Pages
   - Your site updates at https://ArnaudBougaham.github.io

### Initial Setup

If setting up for the first time:

1. **Create Personal Access Token**:
   - Go to: https://github.com/settings/tokens
   - Generate new token (classic) with `repo` and `workflow` scopes

2. **Push to GitHub**:
   ```bash
   git remote add origin https://YOUR_TOKEN@github.com/ArnaudBougaham/ArnaudBougaham.github.io.git
   git push -u origin main
   ```

3. **Enable GitHub Pages**:
   - Go to repository Settings → Pages
   - Select "GitHub Actions" as source
   - Save

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
