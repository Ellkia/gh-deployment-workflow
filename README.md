# GitHub Pages Deployment

Project: https://roadmap.sh/projects/github-actions-deployment-workflow

## Description
Automated deployment of a static website to GitHub Pages using GitHub Actions.
Every push to `main` that modifies `index.html` automatically triggers a deployment.

## Live Site
https://ellkia.github.io/gh-deployment-workflow/

## How it works
1. Modify `index.html` locally
2. Push to `main` branch
3. GitHub Actions workflow triggers automatically
4. Site is updated on GitHub Pages within 1-2 minutes

## Project Structure
gh-deployment-workflow/
├── index.html              # Main page
├── README.md               # This file
└── .github/
└── workflows/
└── deploy.yml      # GitHub Actions workflow

## Deploy workflow
The workflow is triggered only when `index.html` is modified:
- Checks out the code
- Configures GitHub Pages
- Uploads the site as an artifact
- Deploys to GitHub Pages

## Key Learnings
- GitHub Actions and workflow syntax
- GitHub Pages hosting
- CI/CD concepts: automatic deployment on push
- The difference between manual deployment (deploy.sh) and automated pipelines