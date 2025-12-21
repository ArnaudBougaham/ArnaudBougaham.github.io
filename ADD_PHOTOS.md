# 📸 How to Add Your Photos

## Quick Steps

1. **Get your photos ready** (profile picture, etc.)
2. **Place them in**: `static/images/photos/`
3. **Name them correctly** (see below)
4. **Done!** The Hugo theme will automatically use them

## Required Photo

### Profile Photo
- **File name**: `profile.jpg` or `profile.png`
- **Location**: `static/images/photos/profile.jpg`
- **Recommended size**: 400x400px or larger (square format works best)
- **Format**: JPG or PNG
- **Usage**: Will appear on your homepage/about section

## Optional Photos

### Hero/Banner Image (Optional)
- **File name**: `hero.jpg` or `hero.png`
- **Location**: `static/images/photos/hero.jpg`
- **Recommended size**: 1920x600px (wide format)
- **Usage**: Banner/header image if your theme supports it

### Research Photo (Optional)
- **File name**: `research.jpg` or `research.png`
- **Location**: `static/images/photos/research.jpg`
- **Usage**: Can be added to publications or about section

## File Structure

```
hugo-resume-site/
└── static/
    └── images/
        └── photos/
            ├── profile.jpg      ← Your profile photo (REQUIRED)
            ├── hero.jpg         ← Optional banner image
            └── research.jpg     ← Optional research photo
```

## Image Tips

- ✅ Use a professional headshot for profile photo
- ✅ Ensure good lighting and clear background
- ✅ Keep file sizes reasonable (under 500KB for web)
- ✅ Square format (1:1 ratio) works best for profile photos
- ✅ Use JPG for photos, PNG for graphics with transparency

## Compression Tools

Before uploading, consider compressing images:
- [TinyPNG](https://tinypng.com/) - Compress PNG/JPG
- [Squoosh](https://squoosh.app/) - Google's image compression tool

## After Adding Photos

Once you've added your photos:
1. Test locally: `hugo server -D`
2. Check that images appear correctly
3. Deploy to GitHub Pages

The Hugo theme will automatically style and display your photos beautifully!

---

**Note**: If you don't have a profile photo yet, the site will still work - you can add it later. Just make sure the file path matches: `static/images/photos/profile.jpg`

