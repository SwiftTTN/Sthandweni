# Images Reference Guide

## Current Status

Images are currently **referenced via URL** from Wikimedia Commons and official sources rather than stored locally. This approach:

✅ Respects Creative Commons licenses
✅ Keeps repository size small (112 KB instead of 5+ MB)
✅ Provides live, up-to-date images
✅ No licensing compliance issues

## How to Display Images

To show athlete images on the research webpage, you have two options:

### Option 1: Use Wikimedia Commons Images (Recommended)

Wikimedia Commons hosts freely licensed images for most athletes. URLs follow this pattern:

```
https://commons.wikimedia.org/wiki/Special:FilePath/[FILENAME]
```

**Available Wikimedia Categories:**
- Hidilyn Diaz: https://commons.wikimedia.org/wiki/Category:Hidilyn_Diaz
- Kuo Hsing-chun: https://commons.wikimedia.org/wiki/Category:Kuo_Hsing-chun
- Solfrid Koanda: https://commons.wikimedia.org/wiki/Category:Solfrid_Koanda
- Olivia Reeves: Search on Wikimedia Commons
- Hou Zhihui: Check Wikimedia Commons
- Li Wenwen: Check Wikimedia Commons

### Option 2: Add Direct Image Links to JSON

Update `weightlifting-research.json` athlete objects with real image URLs:

```json
"images": [
  {
    "type": "Olympic Champion",
    "url": "https://commons.wikimedia.org/wiki/Special:FilePath/[ACTUAL_FILENAME].jpg",
    "source": "Wikimedia Commons",
    "license": "CC-BY-4.0",
    "caption": "Athlete at [Event/Year]",
    "attribution": "Photo by [Photographer Name]"
  }
]
```

### Option 3: Download and Store Locally

If you want to store images locally:

1. Download from Wikimedia Commons (verify license)
2. Create folder: `/docs/weightlifting/images/`
3. Save as: `/docs/weightlifting/images/[athlete-name].jpg`
4. Update JSON with local paths:
   ```json
   "images": [
     {
       "type": "Olympic Champion",
       "url": "images/hidilyn-diaz.jpg",
       "source": "Wikimedia Commons",
       "license": "CC-BY-4.0",
       "caption": "Hidilyn Diaz at Tokyo 2020"
     }
   ]
   ```
5. Update `research.html` to display images

## Finding Images

### Wikimedia Commons Search
1. Go to https://commons.wikimedia.org
2. Search athlete name
3. Check license (CC0, CC-BY, CC-BY-SA)
4. Copy image URL

### Official Olympic Photos
- Olympics.com has official photos (often with restrictions)
- International Weightlifting Federation (IWF) may have competition photos

### Recommended Search Terms
- `[Athlete Name] Olympic`
- `[Athlete Name] weightlifting`
- `[Athlete Name] Olympics 2024`
- `[Athlete Name] Olympics 2020`

## License Types Found

| License | Usability | Attribution Required |
|---------|-----------|---------------------|
| CC0 | Free use, any purpose | No |
| CC-BY-4.0 | Free use, any purpose | Yes |
| CC-BY-SA | Free use, must share alike | Yes |
| Official Olympic | Usually restricted | Depends |

## Implementation Path

### To Add Images to Research Webpage:

1. **Update JSON** with image URLs
2. **Modify research.html** to display images:
   ```html
   <div class="athlete-image">
     <img src="${athlete.images[0]?.url}"
          alt="${athlete.name}"
          class="athlete-photo">
   </div>
   ```
3. **Add CSS** for image styling
4. **Test locally** before deploying
5. **Commit and push** to GitHub

## Sample Implementation

Here's how to modify `research.html` to show images:

```javascript
// In the renderAthletes() function, add:
if (athlete.images && athlete.images.length > 0) {
  const img = athlete.images[0];
  card.innerHTML += `
    <div class="athlete-image-container">
      <img src="${img.url}"
           alt="${athlete.name} - ${img.caption}"
           class="athlete-photo"
           onerror="this.src='https://via.placeholder.com/300x400?text=${athlete.name}'">
      <p class="image-credit">Photo: ${img.source}</p>
    </div>
  `;
}
```

## Next Steps

1. **Decide**: Which images to include and where to get them
2. **Update**: JSON with real image URLs
3. **Modify**: research.html to display images
4. **Test**: Locally to ensure images load
5. **Deploy**: Push to GitHub

## Resources

- **Wikimedia Commons**: https://commons.wikimedia.org
- **Olympics Official**: https://www.olympic.org
- **IWF Official**: https://iwf.sport
- **Creative Commons**: https://creativecommons.org

---

**Note**: Currently, the JSON has placeholder image URLs. To display actual images, you'll need to:
1. Find real image URLs from Wikimedia Commons or official sources
2. Update the JSON with those URLs
3. Modify the HTML to display them

This guide provides the framework to do that! 🖼️
