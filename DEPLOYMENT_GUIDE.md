# 🚀 Simple Deployment Guide

## Step 1: Create a GitHub Account (if you don't have one)
1. Go to [github.com](https://github.com)
2. Click "Sign up"
3. Follow the steps to create your free account

## Step 2: Install Git on Your Computer
- **Windows**: Download from [git-scm.com](https://git-scm.com/download/win)
- **Mac**: Run `brew install git` or download from [git-scm.com](https://git-scm.com/download/mac)
- **Linux**: Run `sudo apt-get install git`

## Step 3: Upload Your Site to GitHub

### Option A: Using GitHub Desktop (Easiest)
1. Download [GitHub Desktop](https://desktop.github.com/)
2. Sign in with your GitHub account
3. Click "Create New Repository"
4. Name it something like "my-portfolio"
5. Choose the `/home/js/repos/personal-profile` folder
6. Click "Create Repository"
7. Click "Publish repository"

### Option B: Using Command Line
Open terminal in the `/home/js/repos/personal-profile` folder and run:

```bash
# Initialize git
git init

# Add all files
git add .

# Create first commit
git commit -m "Initial portfolio site"

# Create repository on GitHub (do this on github.com first)
# Then connect your local folder to GitHub:
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git

# Push your code
git branch -M main
git push -u origin main
```

## Step 4: Enable GitHub Pages

1. Go to your repository on GitHub.com
2. Click **Settings** (in the repository, not your profile)
3. Scroll down to **Pages** section (left sidebar)
4. Under "Source", select **GitHub Actions**
5. Wait 2-3 minutes for deployment

## Step 5: Visit Your Site!

Your site will be live at:
```
https://YOUR_USERNAME.github.io/YOUR_REPO_NAME
```

Example: If your username is "johndoe" and repo is "my-portfolio":
`https://johndoe.github.io/my-portfolio`

## 🎯 Quick Checklist

- [ ] Created GitHub account
- [ ] Installed Git
- [ ] Created new repository on GitHub
- [ ] Pushed code to repository
- [ ] Enabled GitHub Pages with "GitHub Actions" source
- [ ] Waited 2-3 minutes
- [ ] Visited your live site!

## 🆘 Troubleshooting

**"Site not found" error?**
- Wait 5 more minutes (first deploy can be slow)
- Check Settings > Pages to see if there are any error messages
- Make sure you selected "GitHub Actions" as source

**Can't push code?**
- Make sure you're logged into git: `git config --global user.email "your-email@example.com"`
- Check that you created the repository on GitHub first

**Need more help?**
- GitHub Pages docs: https://pages.github.com/
- Ask me for specific help with any step!