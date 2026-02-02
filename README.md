# Fawn & Craig Wedding Website 💍

A beautiful, sage green spring-themed wedding website with countdown timer, story section, schedule, venue info, and gift guide.

## 🚀 Quick Deploy to GitHub Pages

### First-Time Setup (5 minutes)

1. **Go to GitHub** and log into your account

2. **Create a new repository:**
   - Click the **+** icon (top right) → **New repository**
   - Repository name: `fawn-and-craig`
   - Keep it **Public** (required for free GitHub Pages)
   - Do NOT initialize with README (we have one)
   - Click **Create repository**

3. **Upload your files:**
   - On the new repository page, click **"uploading an existing file"** link
   - Drag and drop BOTH files: `index.html` and `README.md`
   - Scroll down, click **Commit changes**

4. **Enable GitHub Pages:**
   - Go to **Settings** (tab at the top of your repo)
   - Scroll down to **Pages** (left sidebar)
   - Under "Source", select **Deploy from a branch**
   - Under "Branch", select **main** and **/ (root)**
   - Click **Save**

5. **Wait 1-2 minutes**, then visit:
   ```
   https://YOUR-USERNAME.github.io/fawn-and-craig
   ```
   (Replace YOUR-USERNAME with your actual GitHub username)

---

## ✏️ How to Update Your Website

### Method 1: Edit Directly on GitHub (Easiest)

1. Go to your repository: `github.com/YOUR-USERNAME/fawn-and-craig`
2. Click on `index.html`
3. Click the **pencil icon** (Edit this file) in the top right
4. Make your changes
5. Scroll down and click **Commit changes**
6. Wait 1-2 minutes for the site to update

### Method 2: Upload a New Version

1. Edit `index.html` on your computer
2. Go to your repository on GitHub
3. Click on `index.html`
4. Click the **pencil icon** → delete all content → paste new content
5. Or: Delete the file and upload a new one

---

## 📝 What to Customize

Open `index.html` and search for these sections:

### 1. Wedding Date (for countdown timer)
Search for: `const weddingDate`
```javascript
const weddingDate = new Date(2025, 5, 14, 15, 0, 0);
// Format: Year, Month (0-11), Day, Hour, Minute, Second
// Note: Month is 0-indexed! January=0, June=5, December=11
```

### 2. Display Date Text
Search for: `June 14, 2025` and update in these places:
- The hero section (line ~270)
- The footer (line ~540)

### 3. Couple Names
Search for: `Fawn` and `Craig` to update throughout

### 4. Our Story Section
Search for: `Your love story goes here`
Replace the placeholder div with your story text

### 5. Schedule Section
Search for: `UNCOMMENT AND EDIT THE TIMELINE`
Remove the `<!--` and `-->` around the timeline, then edit:
```html
<div class="timeline-item">
    <div class="timeline-time">3:00 PM</div>
    <div class="timeline-event">Ceremony</div>
    <div class="timeline-detail">Doors open at 2:30 PM</div>
</div>
```

### 6. Venue Section
Search for: `UNCOMMENT AND EDIT WHEN READY`
Remove the `<!--` and `-->` around the venue info, then edit:
```html
<div class="venue-info">
    <h3 class="venue-name">Your Venue Name</h3>
    <p class="venue-address">
        123 Beautiful Lane<br>
        City, State 12345
    </p>
    <a href="https://maps.google.com/YOUR-LINK" target="_blank" class="venue-btn">Get Directions</a>
</div>
```

### 7. Add a Google Maps Embed (Optional)
Replace the map placeholder with:
```html
<iframe 
    src="https://www.google.com/maps/embed?pb=YOUR-EMBED-CODE"
    width="100%" 
    height="250" 
    style="border:0;" 
    allowfullscreen="" 
    loading="lazy">
</iframe>
```
(Get embed code: Google Maps → Search location → Share → Embed a map)

### 8. Add Your Photo
Replace the photo-frame div with:
```html
<div class="photo-frame" style="padding: 0; overflow: hidden;">
    <img src="YOUR-IMAGE-URL" alt="Fawn and Craig" style="width: 100%; height: 100%; object-fit: cover;">
</div>
```
(Upload image to GitHub or use a link from Google Photos/Imgur)

### 9. Hashtag
Search for: `#FawnAndCraig2025` in the footer

---

## 🖼️ Adding Photos

### Option 1: Upload to GitHub
1. In your repository, click **Add file** → **Upload files**
2. Upload your image (e.g., `couple-photo.jpg`)
3. In `index.html`, reference it as: `src="couple-photo.jpg"`

### Option 2: Use External Image Host
1. Upload to Imgur, Google Photos (shared link), or similar
2. Get the direct image URL
3. Use that URL in the `src` attribute

---

## 🎨 Color Reference

The site uses these sage green colors (CSS variables in the file):
- `--sage-deep: #4a5d4a` (darkest - headings)
- `--sage: #7d9478` (primary - buttons, accents)
- `--sage-light: #a8c0a1` (medium - decorations)
- `--sage-pale: #d4e4cf` (light - borders)
- `--sage-whisper: #eef4ec` (lightest - backgrounds)

---

## ❓ Troubleshooting

**Site not updating?**
- Wait 2-5 minutes (GitHub Pages can be slow)
- Hard refresh your browser: `Ctrl+Shift+R` (Windows) or `Cmd+Shift+R` (Mac)

**404 error?**
- Make sure the file is named exactly `index.html` (lowercase)
- Check that GitHub Pages is enabled in Settings → Pages

**Need help?**
- GitHub Pages docs: https://docs.github.com/en/pages

---

Made with 💚 for Fawn & Craig's special day!
