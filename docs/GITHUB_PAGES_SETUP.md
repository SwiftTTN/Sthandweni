# 🚀 GitHub Pages Setup Guide

This guide will help you deploy your research projects to GitHub Pages.

## Prerequisites

You need:
- A GitHub account (free at github.com)
- This repository cloned/pushed to GitHub
- Git installed on your computer

## Step-by-Step Setup

### 1. **Create/Push Repository to GitHub**

If you haven't already, create a repository on GitHub:

```bash
# Navigate to your repo
cd /path/to/Sthandweni

# Initialize git (if not already done)
git init

# Add all files
git add .

# Commit
git commit -m "Add research projects"

# Add remote origin (replace USERNAME/REPO-NAME)
git remote add origin https://github.com/USERNAME/REPO-NAME.git

# Push to GitHub
git branch -M main
git push -u origin main
```

### 2. **Enable GitHub Pages**

In your GitHub repository:

1. Go to **Settings** → **Pages**
2. Under "Build and deployment":
   - **Source**: Select "Deploy from a branch"
   - **Branch**: Select `main`
   - **Folder**: Select `/ (root)` OR `/docs` (if using docs folder)
3. Click **Save**

**Important**: Make sure you select the **`/docs`** folder since all your content is in the `docs/` directory!

### 3. **Access Your Site**

GitHub will provide you a URL like:
```
https://USERNAME.github.io/REPO-NAME/
```

Your site will be live at:
- **Main Hub**: `https://USERNAME.github.io/REPO-NAME/`
- **Weightlifting**: `https://USERNAME.github.io/REPO-NAME/weightlifting/`
- **Research DB**: `https://USERNAME.github.io/REPO-NAME/weightlifting/research.html`

---

## Current Project Structure

```
Sthandweni/
├── docs/                          ← GitHub Pages Source!
│   ├── index.html                 ← Main landing page
│   └── weightlifting/
│       ├── index.html             ← Project landing page
│       ├── research.html          ← Interactive research viewer
│       └── weightlifting-research.json  ← Raw data
└── [other files]
```

---

## Why Use `/docs`?

GitHub Pages can serve from:
- `main` branch `/` (entire root folder)
- `main` branch `/docs` (only the docs folder) ← **We're using this**
- `gh-pages` branch `/` (separate branch)

Using `/docs` is cleaner because:
✅ Keeps source code separate from web content
✅ No need for separate branches
✅ Easier to maintain
✅ All web files in one place

---

## After Deployment

### Check Your Live Site

Once published (usually within 1-2 minutes), visit:
```
https://USERNAME.github.io/REPO-NAME/
```

You should see:
1. **Main Hub** with project list
2. Link to **Elite Female Weightlifters** project
3. Access to research database

### Test the Links

Verify all pages work:
- ✅ Main page loads
- ✅ Weightlifting project page loads
- ✅ Research database page loads and displays data
- ✅ JSON data loads in browser
- ✅ Filters work
- ✅ Search functionality works
- ✅ Print to PDF works

---

## Updating Your Site

After making changes:

```bash
# Navigate to repository
cd /path/to/Sthandweni

# Stage changes
git add docs/

# Commit changes
git commit -m "Update research data or website"

# Push to GitHub
git push
```

GitHub Pages will automatically rebuild within 1-2 minutes.

---

## Custom Domain (Optional)

Want to use your own domain instead of `github.io`?

1. In **Settings** → **Pages**
2. Add your custom domain
3. Update DNS records at your domain registrar
4. GitHub will verify and enable HTTPS

---

## Troubleshooting

### Site Not Loading?

1. Check **Settings** → **Pages** shows "Your site is live"
2. Verify source is set to `main` branch `/docs` folder
3. Wait 2-3 minutes for rebuild
4. Clear browser cache (Ctrl+Shift+Delete)
5. Check repository is public (Settings → General)

### Data Not Loading?

1. Verify JSON file path: `/docs/weightlifting/weightlifting-research.json`
2. Check browser console (F12) for errors
3. Ensure JSON file was pushed to GitHub
4. Check file is not in `.gitignore`

### Styling Issues?

1. Clear browser cache
2. Hard refresh (Ctrl+Shift+R or Cmd+Shift+R)
3. Check that CSS is loading (F12 → Network tab)

### Search/Filters Not Working?

1. Check JavaScript console (F12) for errors
2. Verify data file is loading
3. Try in different browser
4. Check that `weightlifting-research.json` is in correct folder

---

## GitHub Pages URL Format

Replace placeholders:

```
https://[USERNAME].github.io/[REPO-NAME]/

Examples:
- https://john.github.io/Sthandweni/
- https://jane.github.io/research-projects/
- https://dev.github.io/my-research/
```

---

## File Hierarchy for Pages

```
docs/
├── index.html
│   └── Links to weightlifting project
├── weightlifting/
│   ├── index.html
│   │   └── Landing page, links to research
│   ├── research.html
│   │   └── Interactive research viewer
│   │       (Loads weightlifting-research.json from same folder)
│   └── weightlifting-research.json
│       └── Data file loaded by research.html
```

---

## Making Your Site Discoverable

### Add to GitHub Profile

1. Go to your GitHub profile
2. Edit bio/README
3. Add link: `https://[USERNAME].github.io/[REPO-NAME]/`

### SEO Tips

The pages already have:
✅ Proper meta tags
✅ Descriptive titles
✅ Semantic HTML
✅ Mobile responsive design

---

## Quick Reference

| File | Purpose | URL |
|------|---------|-----|
| `/docs/index.html` | Main hub | `/` |
| `/docs/weightlifting/index.html` | Project landing | `/weightlifting/` |
| `/docs/weightlifting/research.html` | Research viewer | `/weightlifting/research.html` |
| `/docs/weightlifting/weightlifting-research.json` | Data file | `/weightlifting/weightlifting-research.json` |

---

## Example Complete URLs

Once published to GitHub Pages with username `john` and repo `Sthandweni`:

```
Main Hub
https://john.github.io/Sthandweni/

Project Landing
https://john.github.io/Sthandweni/weightlifting/

Research Database
https://john.github.io/Sthandweni/weightlifting/research.html

Raw JSON Data
https://john.github.io/Sthandweni/weightlifting/weightlifting-research.json
```

---

## Support & Help

If your site isn't working:

1. **Check Settings**: Verify GitHub Pages is enabled
2. **Check Files**: Ensure all files are in `/docs` folder
3. **Check Logs**: GitHub Pages build logs (Settings → Pages → Recent deployments)
4. **Test Locally**: Open `docs/index.html` in browser locally first
5. **Browser Cache**: Clear cache and hard refresh

---

## Next Steps

1. Push this repository to GitHub
2. Enable GitHub Pages in Settings
3. Wait 1-2 minutes for deployment
4. Visit your GitHub Pages URL
5. Share with others!

---

**Happy researching! 🚀**

For questions about the research database itself, see the README in the weightlifting folder.
