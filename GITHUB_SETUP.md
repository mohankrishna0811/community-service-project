# GitHub Setup Instructions

Follow these steps to push your website to GitHub:

## Step 1: Configure Git (if not already done)

Run these commands in your terminal (replace with your information):

```bash
git config --global user.name "Your Name"
git config --global user.email "your.email@example.com"
```

Or for this repository only:

```bash
git config user.name "Your Name"
git config user.email "your.email@example.com"
```

## Step 2: Create a GitHub Repository

1. Go to [GitHub.com](https://github.com) and sign in
2. Click the "+" icon in the top right corner
3. Select "New repository"
4. Name your repository (e.g., "health-hygiene-website")
5. Choose Public or Private
6. **DO NOT** initialize with README, .gitignore, or license (we already have these)
7. Click "Create repository"

## Step 3: Push Your Code

After creating the repository, GitHub will show you commands. Use these:

```bash
# Make sure you're in the project directory
cd "C:\Users\chenn\OneDrive\Desktop\health and hygiene"

# Add the remote repository (replace YOUR_USERNAME and REPO_NAME)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Rename branch to main (if needed)
git branch -M main

# Push your code
git push -u origin main
```

## Alternative: Using GitHub CLI

If you have GitHub CLI installed:

```bash
gh repo create health-hygiene-website --public --source=. --remote=origin --push
```

## That's it!

Your website is now on GitHub. You can:
- View it at: `https://github.com/YOUR_USERNAME/REPO_NAME`
- Enable GitHub Pages to host it for free
- Share it with others

## Enable GitHub Pages (Optional - Free Hosting)

1. Go to your repository on GitHub
2. Click "Settings"
3. Scroll to "Pages" in the left sidebar
4. Under "Source", select "main" branch
5. Click "Save"
6. Your site will be live at: `https://YOUR_USERNAME.github.io/REPO_NAME/`
