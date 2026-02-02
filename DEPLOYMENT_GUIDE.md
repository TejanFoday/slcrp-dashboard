# GitHub Pages Deployment Guide

## How to Deploy the SLCRP Dashboard to GitHub

### Step 1: Create a New Repository on GitHub

1. Go to [GitHub.com](https://github.com) and log in
2. Click the **"+"** icon in the top right and select **"New repository"**
3. Name your repository (suggested: `slcrp-dashboard` or `slcrp-visual-dashboard`)
4. Add a description: "Sierra Leone Coastal Resilience Project - Visual Dashboard"
5. Choose **Public** (so it can be viewed online)
6. Check **"Add a README file"** (we'll update it later)
7. Click **"Create repository"**

### Step 2: Upload Your Files

#### Option A: Using GitHub Web Interface (Easiest)

1. In your new repository, click **"Add file"** → **"Upload files"**
2. Drag and drop these files:
   - `index.html` (your dashboard file)
   - `README.md` (the README file)
3. Scroll down and click **"Commit changes"**

#### Option B: Using Git Command Line

```bash
# Initialize git in your project folder
git init

# Add your files
git add index.html README.md

# Commit the files
git commit -m "Initial commit: SLCRP Dashboard"

# Link to your GitHub repository (replace YOUR-USERNAME and YOUR-REPO)
git remote add origin https://github.com/YOUR-USERNAME/YOUR-REPO.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### Step 3: Enable GitHub Pages

1. In your repository, go to **"Settings"** (top menu)
2. Scroll down to **"Pages"** in the left sidebar
3. Under **"Source"**, select:
   - Branch: **main**
   - Folder: **/ (root)**
4. Click **"Save"**
5. Wait 1-2 minutes for deployment

### Step 4: Access Your Dashboard

Your dashboard will be available at:
```
https://YOUR-USERNAME.github.io/YOUR-REPO-NAME/
```

For example:
```
https://tejan-epa.github.io/slcrp-dashboard/
```

### Step 5: Share Your Dashboard

Once deployed, you can share the URL with:
- EPA colleagues
- Implementing partners
- GCF stakeholders
- Consortium review meetings

### Updating Your Dashboard

To update the dashboard later:

1. Go to your repository on GitHub
2. Click on `index.html`
3. Click the pencil icon (✏️) to edit
4. Make your changes
5. Scroll down and click **"Commit changes"**
6. Your dashboard will update automatically (1-2 minutes)

### Tips for Success

✅ **Keep the filename as `index.html`** - This ensures GitHub Pages displays it automatically

✅ **Use descriptive commit messages** - Example: "Updated Activity 1.4.6 beneficiary numbers"

✅ **Test locally first** - Open the HTML file in your browser before uploading

✅ **Update the README** - Keep it current with latest project information

### Troubleshooting

**Dashboard not showing?**
- Check that the file is named exactly `index.html`
- Verify GitHub Pages is enabled in Settings → Pages
- Wait 2-3 minutes after uploading for changes to appear
- Clear your browser cache

**Need to make it private?**
- Go to Settings → General → Danger Zone
- Click "Change repository visibility"
- Note: Private repos need GitHub Pro for GitHub Pages

### Custom Domain (Optional)

If you want to use a custom domain (e.g., dashboard.epa-sl.org):

1. Buy a domain name
2. In your repository Settings → Pages
3. Add your custom domain
4. Configure DNS settings with your domain provider

---

**Need Help?**
- GitHub Pages Documentation: https://docs.github.com/pages
- GitHub Support: https://support.github.com

