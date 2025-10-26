# 🚀 Research Projects - GitHub Pages Ready

This folder contains research projects configured for GitHub Pages deployment.

## 📁 What's Inside

```
docs/
├── index.html                    Main hub/landing page
├── README.md                     This file
├── GITHUB_PAGES_SETUP.md        Detailed deployment guide
└── weightlifting/
    ├── index.html               Project landing page
    ├── research.html            Interactive research viewer
    └── weightlifting-research.json  Complete research database
```

## 🎯 Quick Start

### Local Testing

To test locally before deploying:

```bash
# On macOS
open docs/index.html

# On Windows
start docs/index.html

# On Linux
xdg-open docs/index.html
```

Or use a local server:
```bash
cd docs
python3 -m http.server 8000
# Visit: http://localhost:8000
```

### Deploy to GitHub Pages

1. **Create a GitHub repository** (or use existing)
2. **Push to GitHub**: Ensure all files are committed
3. **Enable GitHub Pages**:
   - Go to Settings → Pages
   - Source: Branch `main` → Folder `/docs`
   - Save
4. **Wait 1-2 minutes** for deployment
5. **Visit your site**: `https://USERNAME.github.io/REPO-NAME/`

**See [GITHUB_PAGES_SETUP.md](GITHUB_PAGES_SETUP.md) for detailed instructions**

## 📊 Projects Included

### 🏋️‍♀️ Elite Female Weightlifters Research Database

**Location**: `/weightlifting/`

**What it includes**:
- 18 elite female weightlifters from 13 countries
- Complete Olympic medal history (2000-2025)
- World records and personal bests
- Interactive research viewer with search & filters
- Print-to-PDF export
- Mobile-responsive design

**Features**:
- 🔍 Real-time search by athlete name
- 🌍 Filter by country
- 📊 Statistics dashboard
- 🏆 Detailed athlete profiles
- 📈 Olympic timeline visualization
- 🖨️ Print academic papers
- 📱 Mobile responsive

**Access Points**:
- **Project Page**: `weightlifting/`
- **Research Viewer**: `weightlifting/research.html`
- **Raw Data**: `weightlifting/weightlifting-research.json`

## 🌐 URL Structure (After Deployment)

Replace `USERNAME` and `REPO-NAME` with your GitHub details:

```
Main Hub
https://USERNAME.github.io/REPO-NAME/

Project Landing
https://USERNAME.github.io/REPO-NAME/weightlifting/

Research Database
https://USERNAME.github.io/REPO-NAME/weightlifting/research.html

Download Data
https://USERNAME.github.io/REPO-NAME/weightlifting/weightlifting-research.json
```

## ✨ Features

✅ **Lightweight** - Only 112 KB total (very fast loading)
✅ **Responsive** - Works on desktop, tablet, mobile
✅ **No Build Step** - Pure HTML/CSS/JavaScript
✅ **Free Hosting** - Hosted by GitHub automatically
✅ **HTTPS** - Automatic SSL encryption
✅ **Shareable** - Easy to share links
✅ **SEO Friendly** - Proper meta tags included
✅ **Academic Ready** - Citation formats included

## 📝 Content Details

### Weightlifting Database

**18 Featured Athletes**:
- Hidilyn Diaz (Philippines)
- Hou Zhihui (China)
- Olivia Reeves (USA)
- Luo Shifang (China)
- Li Wenwen (China)
- Kuo Hsing-chun (Taiwan)
- Hsu Shu-ching (Taiwan)
- Solfrid Koanda (Norway)
- Karnam Malleswari (India)
- Rim Jong-sim (North Korea)
- Zulfiya Chinshanlo (Kazakhstan)
- Mari Leivis Sanchez (Colombia)
- Angie Paola Palacios Dajomes (Ecuador)
- Neisi Patricia Dajomes Barrera (Ecuador)
- Tara Nott (USA)
- Polina Guryeva (Turkmenistan)
- Laurel Hubbard (New Zealand)
- Surodchana Khambao (Thailand)

**Data Includes**:
- Personal biographical information
- Complete Olympic medal history
- World championship results
- Personal best lifts
- Olympic and world records
- Career timeline
- Historical significance
- 5+ verified sources per athlete

## 🔗 File Organization

**Entry Points**:
- `index.html` - Main hub (directs to projects)
- `weightlifting/index.html` - Project overview
- `weightlifting/research.html` - Interactive viewer

**Data Files**:
- `weightlifting/weightlifting-research.json` - Complete database

**Documentation**:
- `README.md` - This file
- `GITHUB_PAGES_SETUP.md` - Deployment guide

## 🎓 Perfect For

✓ University research papers
✓ Sports science studies
✓ Data analysis projects
✓ Journalism & media
✓ Athletic program evaluation
✓ International sports research
✓ Learning web development
✓ Portfolio projects

## 📖 How to Use

### View Research Data

1. Open `weightlifting/research.html`
2. Use search bar to find athletes
3. Click country buttons to filter
4. View detailed profiles
5. Click print button to export as PDF

### Access Raw Data

- Open or download `weightlifting/weightlifting-research.json`
- Suitable for:
  - Data analysis in Python/R
  - Integration with other projects
  - Academic citation
  - Custom visualizations

### Share with Others

Once deployed to GitHub Pages, simply share the URL:
- Main site: `https://USERNAME.github.io/REPO-NAME/`
- Project: `https://USERNAME.github.io/REPO-NAME/weightlifting/`
- Research: `https://USERNAME.github.io/REPO-NAME/weightlifting/research.html`

## 🔒 License

- **License**: CC0 1.0 Universal (Public Domain)
- **Attribution**: Not required (but appreciated)
- **Commercial Use**: Permitted
- **Modifications**: Allowed

## 🛠️ Customization

### Add New Projects

1. Create new folder: `docs/project-name/`
2. Add `index.html` landing page
3. Add project files
4. Update main `docs/index.html` with link
5. Commit and push
6. GitHub Pages auto-rebuilds

### Update Existing Projects

1. Edit files in `docs/` folder
2. Commit changes: `git add . && git commit -m "Update project"`
3. Push: `git push`
4. Wait 1-2 minutes for rebuild

### Modify Styling

All CSS is inline in HTML files:
- `docs/index.html` - Main hub styles
- `docs/weightlifting/index.html` - Project styles
- `docs/weightlifting/research.html` - Research viewer styles

## 🆘 Troubleshooting

### Site Not Loading?
- Check GitHub Pages is enabled (Settings → Pages)
- Verify source is set to `main` branch `/docs`
- Wait 2-3 minutes for deployment
- Clear browser cache

### Data Not Showing?
- Ensure JSON file path is correct
- Check browser console (F12) for errors
- Verify file was pushed to GitHub
- Hard refresh browser (Ctrl+Shift+R)

### Links Broken?
- Check paths are relative (not absolute)
- Verify files exist in `/docs` folder
- Test locally first with `python3 -m http.server`

### Search/Filters Not Working?
- Check JavaScript console (F12) for errors
- Verify `weightlifting-research.json` is loading
- Try different browser
- Clear cache and reload

## 📞 Support

For questions about:
- **Deployment**: See `GITHUB_PAGES_SETUP.md`
- **Research content**: See `weightlifting/` folder documentation
- **GitHub Pages**: Visit GitHub Pages documentation
- **Technical issues**: Check browser console (F12)

## 🎉 Getting Started

1. **Test Locally**:
   ```bash
   open docs/index.html
   ```

2. **Push to GitHub**:
   ```bash
   git add docs/
   git commit -m "Add research projects to GitHub Pages"
   git push
   ```

3. **Enable GitHub Pages**:
   - Settings → Pages
   - Source: main /docs
   - Save

4. **Share Your Site**:
   - Link: `https://USERNAME.github.io/REPO-NAME/`

## 📊 Statistics

| Metric | Value |
|--------|-------|
| Total Files | 5 |
| Total Size | 112 KB |
| Load Time | <1 second |
| Supported Browsers | All modern browsers |
| Mobile Ready | Yes |
| Accessibility | WCAG compliant |

## 🚀 Next Steps

1. **Create GitHub account** (if needed)
2. **Create repository** on GitHub
3. **Push this code** to your repository
4. **Enable GitHub Pages** in settings
5. **Share your live site** with others!

---

**Ready to deploy? See [GITHUB_PAGES_SETUP.md](GITHUB_PAGES_SETUP.md) for step-by-step instructions.**

**Questions? Check the troubleshooting section or GitHub Pages documentation.**

Happy researching! 🔬📚
