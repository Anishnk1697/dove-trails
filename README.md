# Dove Trails — Where San Antonio Comes Home

This is the fully optimized, self-contained website for **Dove Trails** (5135 Wurzbach Road, San Antonio Medical District). 

## 🚀 Key Improvements & Optimizations
We took the single-file demo HTML (7.8 MB) and transformed it into a premium, production-ready codebase:
1. **Extracted Base64 Assets**: All embedded images have been parsed, decoded, and saved to the `assets/` folder, reducing `index.html` from **7.8 MB to ~140 KB** for near-instant page loads.
2. **Decoupled Brochure**: The huge 5.2 MB embedded PDF/HTML brochure was extracted into a standalone `brochure.html` file, further optimizing the load time of the homepage.
3. **CDN Asset Downloader**: Downloaded all external image files (from Unsplash and Webflow CDNs) directly into the local `assets/` directory. The site is now completely self-contained and will never suffer from broken images or external downtime.
4. **Vercel Integration**: Added `vercel.json` to enable clean URLs (`/brochure` instead of `/brochure.html`) and configure high-performance caching for local assets.

---

## 🛠️ Step-by-Step Deployment Guide

Follow these steps to push your website to GitHub and host it live on Vercel for free:

### Step 1: Initialize Git and Make First Commit
We have already initialized a local Git repository and created the initial commit for you. The files are ready to go.

### Step 2: Create a New GitHub Repository
1. Go to [github.com](https://github.com) and log in.
2. Click the **"+"** icon in the top-right corner and select **"New repository"**.
3. Name your repository (e.g., `dove-trails`) and keep it Public or Private as you prefer.
4. Leave "Add a README file", "Add .gitignore", and "Choose a license" **unchecked** (we already have these in our code).
5. Click **"Create repository"**.

### Step 3: Link Local Project to GitHub and Push
Open your terminal, navigate to the project directory, and run the following commands (replacing `YOUR_USERNAME` and `YOUR_REPO_NAME` with your actual GitHub username and repository name):

```bash
git remote add origin https://github.com/YOUR_USERNAME/YOUR_REPO_NAME.git
git branch -M main
git push -u origin main
```

### Step 4: Deploy to Vercel
1. Go to [vercel.com](https://vercel.com) and log in (you can sign up using your GitHub account).
2. On your Vercel Dashboard, click **"Add New..."** and choose **"Project"**.
3. Import the repository you just pushed (`YOUR_REPO_NAME`).
4. Keep the default settings (Vercel will automatically detect it as a static website).
5. Click **"Deploy"**.

Within seconds, your site will be live on a custom `.vercel.app` domain, and Vercel will automatically redeploy it every time you push changes to your GitHub repository!

---

## 📂 Project Structure
```text
├── assets/            # All optimized local images & design assets
├── .gitignore         # Ignores OS-specific cache files (like .DS_Store)
├── index.html         # Homepage (Optimized)
├── brochure.html      # Digital Brochure (Optimized)
├── vercel.json        # Vercel-specific routing & headers config
└── README.md          # This instruction file
```
