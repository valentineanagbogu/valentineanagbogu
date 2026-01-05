# DevOps Portfolio

Minimal and elegant portfolio website with automated GitHub Pages deployment.

## Setup & Deployment

### 1. Create GitHub Repository

```bash
# Option A: Create repository named 'yourusername.github.io' for main portfolio site
# Your site will be at: https://yourusername.github.io

# Option B: Create any repository name for project portfolio
# Your site will be at: https://yourusername.github.io/repository-name
```

### 2. Customize Your Portfolio

Edit `index.html` and update:
- Hero section: Your name and tagline
- About section: Professional summary
- Skills section: Your technologies
- Projects section: Your actual projects with links
- Contact section: GitHub, LinkedIn, email links

### 3. Push to GitHub

```bash
git init
git add .
git commit -m "Initial portfolio setup"
git branch -M main
git remote add origin https://github.com/yourusername/repository-name.git
git push -u origin main
```

### 4. Enable GitHub Pages

1. Go to repository **Settings** → **Pages**
2. Under **Source**, select: **GitHub Actions**
3. The workflow will automatically deploy your site

### 5. Access Your Site

- Main portfolio: `https://yourusername.github.io`
- Project portfolio: `https://yourusername.github.io/repository-name`

Site deploys automatically on every push to `main` branch.

## Project Structure

```
.
├── .github/
│   └── workflows/
│       └── deploy.yml      # GitHub Actions deployment workflow
├── index.html              # Portfolio landing page
├── styles.css              # Minimal styling
├── .gitignore             # Git ignore rules
└── README.md              # This file
```

## Automated Deployment

The GitHub Actions workflow automatically:
- Triggers on push to `main` branch
- Packages your site files
- Deploys to GitHub Pages
- Completes in ~30 seconds

View deployment status: **Actions** tab in your GitHub repository

## Local Development

Simply open `index.html` in your browser to preview changes before pushing.

## Adding Projects

Replace the placeholder projects in `index.html` with your actual DevOps projects. Link to repositories that showcase:
- Infrastructure as Code (Terraform, CloudFormation)
- Kubernetes deployments and Helm charts
- CI/CD pipeline implementations
- Monitoring and observability solutions
- Automation scripts and tools

## Next Steps

- [ ] Customize all content in index.html
- [ ] Update contact links
- [ ] Create GitHub repository
- [ ] Push code and enable GitHub Pages
- [ ] Build and document your featured projects
