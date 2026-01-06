# Cloudflare Pages Deployment Guide

## Your website is ready to deploy! 🚀

Follow these steps to deploy your portfolio website to Cloudflare Pages:

---

## Method 1: Direct Upload (Easiest - No GitHub Required)

### Step 1: Install Wrangler CLI (if needed)
Since Node.js is not installed, you can either:
- Install Node.js from https://nodejs.org/ (recommended)
- Or use the GitHub method below

Once Node.js is installed:
```bash
npm install -g wrangler
```

### Step 2: Login to Cloudflare
```bash
wrangler login
```

### Step 3: Deploy
```bash
cd /Users/mapalopenza/Documents/website
wrangler pages deploy . --project-name=mapalo-portfolio
```

---

## Method 2: Deploy via GitHub (Recommended - Continuous Deployment)

### Step 1: Create a GitHub Repository

1. Go to https://github.com/new
2. Name your repository (e.g., `portfolio` or `mapalo-portfolio`)
3. Keep it public or private (your choice)
4. **DO NOT** initialize with README (we already have one)
5. Click "Create repository"

### Step 2: Push Your Code to GitHub

Run these commands in your terminal:

```bash
cd /Users/mapalopenza/Documents/website

# Add GitHub repository as remote (replace YOUR_USERNAME with your GitHub username)
git remote add origin https://github.com/YOUR_USERNAME/REPO_NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Deploy to Cloudflare Pages

1. Go to https://pages.cloudflare.com/
2. Click "Log in" (or "Sign up" if you don't have an account)
3. Once logged in, click "Create a project"
4. Click "Connect to Git"
5. Authorize Cloudflare to access your GitHub account
6. Select your repository from the list
7. Configure build settings:
   - **Project name**: `mapalo-portfolio` (or your preferred name)
   - **Production branch**: `main`
   - **Build command**: (leave empty)
   - **Build output directory**: `/` (or leave empty)
8. Click "Save and Deploy"

That's it! Cloudflare will deploy your site and give you a URL like:
`https://mapalo-portfolio.pages.dev`

### Step 4: Custom Domain (Optional)

After deployment, you can add a custom domain:
1. Go to your project in Cloudflare Pages dashboard
2. Click "Custom domains"
3. Click "Set up a domain"
4. Follow the instructions to add your domain

---

## Method 3: Drag & Drop (Quick Test)

If you just want to test deployment quickly:

1. Go to https://pages.cloudflare.com/
2. Log in or sign up
3. Click "Create a project"
4. Click "Upload assets"
5. Drag and drop these files from `/Users/mapalopenza/Documents/website`:
   - index.html
   - images/ (folder)
   - README.md (optional)
6. Click "Deploy site"

**Note**: This method doesn't support continuous deployment from Git.

---

## What Happens Next?

After deployment, Cloudflare Pages will:
- ✅ Serve your website on a global CDN (super fast!)
- ✅ Provide free HTTPS
- ✅ Give you a unique `.pages.dev` URL
- ✅ Auto-deploy when you push to GitHub (if using Git method)
- ✅ Support custom domains for free

---

## Need Help?

If you encounter any issues:
1. Check the Cloudflare Pages documentation: https://developers.cloudflare.com/pages/
2. Make sure all files are committed to Git (if using Git method)
3. Verify your GitHub repository is accessible

---

## Your Current Status

✅ Website is complete and ready
✅ Git repository initialized
✅ All files committed
⏳ Ready to deploy!

Choose one of the methods above and follow the steps to deploy your portfolio to Cloudflare Pages!
