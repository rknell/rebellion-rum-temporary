# Rebellion Rum Co - Temporary Static Website

This is a temporary static website for Rebellion Rum Co while the main website is undergoing maintenance.

## Contents

- `index.html`: The main webpage with information about opening hours, location, and contact details
- `assets/`: Directory containing images and other static assets
  - `logo.png`: Rebellion Rum Co logo
  - `background.jpg`: Fixed background image for the page
  - `header-background.jpg`: Background image for the header section

## Deployment Instructions for GitHub Pages

### Method 1: Using GitHub Pages directly from repository

1. Create a new GitHub repository
2. Push this folder content to the repository
3. Go to repository Settings > Pages
4. Under "Source", select "main" branch and the root directory (or the "docs" folder if you moved the content there)
5. Click Save
6. Your site will be published at `https://[your-username].github.io/[repository-name]/`

### Method 2: Using GitHub CLI (gh)

1. Create a new GitHub repository (or use an existing one):
   ```bash
   gh repo create temporary-rebellion-rum --public
   ```
   
2. Navigate to your project directory and initialize git:
   ```bash
   cd temporary-static-website
   git init
   git add .
   git commit -m "Initial commit"
   ```

3. Add the GitHub repository as remote and push:
   ```bash
   git remote add origin https://github.com/[your-username]/temporary-rebellion-rum.git
   git push -u origin main
   ```

4. Enable GitHub Pages through the GitHub interface as described in Method 1

### Custom Domain Setup

1. In your domain registrar, create a CNAME record pointing your domain to `[your-username].github.io`
2. In your GitHub repository, go to Settings > Pages
3. Under "Custom domain", enter your domain name and click Save
4. Check "Enforce HTTPS" if you want secure access to your site

## Local Development

To view the site locally, simply open the `index.html` file in your web browser. 