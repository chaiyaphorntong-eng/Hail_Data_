#   GitHub Pages Deployment Instructions

##   1.  Create GitHub Repository

###   Go to GitHub:
1. Visit [github.com](https://github.com)
2. Click "New repository" (green button)
3. Repository name: `hail-data-web`
4. Make it **PUBLIC** (important!)
5. **DO NOT** initialize with README, .gitignore, or license
6. Click "Create repository"

---

##   2.  Upload Files

###   Option A: Use GitHub Desktop (Easiest)
1. Download and install [GitHub Desktop](https://desktop.github.com)
2. Click "Add Local Repository"
3. Select your `Hail_Data` folder
4. Commit changes: "Initial deploy"
5. Click "Publish repository"
6. Choose your GitHub account
7. Repository name: `hail-data-web`
8. Click "Publish"

###   Option B: Use Git Command Line
1. Open PowerShell in `Hail_Data` folder
2. Run these commands:
```bash
git init
git add .
git commit -m "Initial deploy"
git branch -M main
git remote add origin https://github.com/YOUR_USERNAME/hail-data-web.git
git push -u origin main
```

---

##   3.  Enable GitHub Pages

###   After uploading:
1. Go to your repository on GitHub
2. Click **Settings** tab
3. Scroll down to **GitHub Pages** section
4. Under "Source", select:
   - **Deploy from a branch**
   - **Branch**: `main`
   - **Folder**: `/ (root)`
5. Click **Save**

###   Wait for deployment:
- GitHub will take 1-2 minutes to deploy
- You'll see a green checkmark when ready
- Your site will be live at: `https://YOUR_USERNAME.github.io/hail-data-web/`

---

##   4.  Test Your Website

###   Visit your URL:
`https://YOUR_USERNAME.github.io/hail-data-web/`

###   What you should see:
- Beautiful landing page with 5 radar stations
- Click any station to see file listing
- Date filtering works
- Download buttons work

---

##   5.  Update Data Later

###   When you have new radar data:
1. Add new .npz files to station folders
2. Update `files.json` with new file information
3. Commit and push changes:
```bash
git add .
git commit -m "Add new radar data"
git push
```
4. GitHub Pages will auto-update in 1-2 minutes

---

##   6.  Troubleshooting

###   Common Issues:
- **404 Error**: Make sure repository is PUBLIC
- **Blank page**: Check GitHub Pages settings
- **Download not working**: Verify file URLs in files.json
- **Slow loading**: Large files may take time to load

###   Get Help:
- Check GitHub Pages documentation
- Verify all files are uploaded correctly
- Make sure files.json has correct URLs

---

##   7.  Success!

###   Your website is now:
-  Online 24/7
- Free forever
- Accessible worldwide
- Automatically updated
- Professional looking

###   Share your URL:
`https://YOUR_USERNAME.github.io/hail-data-web/`

---

##   Quick Summary

1. Create public GitHub repo: `hail-data-web`
2. Upload all files (Git or GitHub Desktop)
3. Enable GitHub Pages in Settings
4. Visit your live website
5. Done! 100% free forever!
