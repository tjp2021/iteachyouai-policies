# ITeachYouAI Policies Site - GitHub Pages Setup

This folder contains the legal/compliance pages for iteachyouai.com (needed for Chrome extension).

## Files:
- `index.html` - Landing page with links to policies
- `privacy-policy.html` - Privacy Policy for Promptimize extension
- `terms-of-service.html` - Terms of Service for Promptimize extension

## Setup Instructions (10 minutes)

### Step 1: Create GitHub Repository

1. Go to https://github.com/new
2. **Repository name:** `iteachyouai-policies`
3. **Description:** "Legal and compliance pages for iteachyouai.com"
4. **Public** (required for free GitHub Pages)
5. **DO NOT** initialize with README
6. Click **Create repository**

### Step 2: Upload Files to GitHub

**Option A: Upload via GitHub Web Interface (Easiest)**

1. On your new empty repo page, click **uploading an existing file**
2. Drag and drop these 3 files:
   - `index.html`
   - `privacy-policy.html`
   - `terms-of-service.html`
3. Add commit message: "Add legal pages for Chrome extension"
4. Click **Commit changes**

**Option B: Use Git Command Line**

```bash
cd /Users/timothyjoo/YNG/ITEACHYOUAI/iteachyouai-policies

git init
git add index.html privacy-policy.html terms-of-service.html
git commit -m "Add legal pages for Chrome extension"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/iteachyouai-policies.git
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. In your GitHub repo, click **Settings** (top right)
2. Scroll down left sidebar, click **Pages**
3. Under "Source", select:
   - **Branch:** `main`
   - **Folder:** `/ (root)`
4. Click **Save**
5. Wait 1-2 minutes for deployment

### Step 4: Get Your Live URLs

Your site will be live at:
```
https://YOUR_USERNAME.github.io/iteachyouai-policies/
https://YOUR_USERNAME.github.io/iteachyouai-policies/privacy-policy.html
https://YOUR_USERNAME.github.io/iteachyouai-policies/terms-of-service.html
```

**Use these URLs in your Chrome extension manifest!**

### Step 5 (Optional): Connect to iteachyouai.com Domain

If you want cleaner URLs like `policies.iteachyouai.com`:

1. In your domain registrar (Namecheap, GoDaddy, etc.), add CNAME record:
   - **Host:** `policies`
   - **Value:** `YOUR_USERNAME.github.io`
   
2. In GitHub Pages settings, add custom domain:
   - **Custom domain:** `policies.iteachyouai.com`
   - **Enforce HTTPS:** ✅ (check this)

3. Wait 10-15 minutes for DNS to propagate

Your URLs will become:
```
https://policies.iteachyouai.com/
https://policies.iteachyouai.com/privacy-policy.html
https://policies.iteachyouai.com/terms-of-service.html
```

## For Chrome Web Store Submission

Use these URLs in your extension manifest:
- **Privacy Policy URL:** Your privacy-policy.html URL from above
- **Terms of Service URL:** Your terms-of-service.html URL from above

---

**Questions? Something not working?** Let me know!

