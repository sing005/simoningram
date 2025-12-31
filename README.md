# Simon Ingram - Artist Website

Minimal, text-focused website inspired by brutalist/programmer aesthetic.

# Simon Ingram - Artist Website

Minimal, text-focused website inspired by brutalist/programmer aesthetic.

## Files

```
index.html              - Home page with background image and numbered work list
list.html               - Complete exhibition index (no hyperlinks)
style.css               - Minimal stylesheet
about.html              - About page
contact.html            - Contact page
images/                 - Directory for images
  rotokare.jpg          - Background image for home page
*.html                  - Individual project pages
```

## Image Setup

### Home Page Background Image

**File:** `images/rotokare.jpg`

**Recommended Dimensions:**
- Minimum: 1920 x 1080 pixels (Full HD)
- Better: 2560 x 1440 pixels (ideal for most screens)
- Best: 3840 x 2160 pixels (4K, only if file size is reasonable)

**File Size:**
- Keep under 500KB for fast loading
- Use JPG format, quality 80-85%
- Optimize with tools like TinyJPG or Squoosh

**Where to Host:**

1. **In Your GitHub Repo (Recommended)**
   - Upload to `images/rotokare.jpg`
   - Free, simple, works forever
   - Max file size: 100MB (but keep it small!)

2. **External Image Hosting (Alternative)**
   - Imgur: Free, reliable
   - Cloudinary: Free tier available
   - Update CSS to point to external URL:
     ```css
     background-image: url('https://yourhost.com/rotokare.jpg');
     ```

### Uploading to GitHub

```bash
# If using Git locally:
git add images/rotokare.jpg
git commit -m "Add background image"
git push

# Or upload directly:
1. Go to repository on GitHub
2. Click "Add file" → "Upload files"
3. Drag rotokare.jpg into images folder
4. Commit
```

## Local Testing

Open `index.html` in any web browser. No build process needed.

## Deployment Options

### Option 1: Neocities (Easiest, Free)

1. Go to https://neocities.org
2. Create account (Free)
3. Upload all files
4. Your site will be at `yourname.neocities.org`
5. Add custom domain in settings (optional, $5/month)

### Option 2: GitHub Pages (Free)

1. Create GitHub account
2. Create repository named `yourusername.github.io`
3. Upload all files to main branch
4. Enable GitHub Pages in Settings → Pages
5. Add custom domain:
   - In repository: Create file `CNAME` with your domain
   - At domain registrar: Add A records:
     - 185.199.108.153
     - 185.199.109.153
     - 185.199.110.153
     - 185.199.111.153

### Option 3: Netlify (Free)

1. Go to https://netlify.com
2. Drag and drop your folder
3. Done! Custom domain included for free

## Custom Domain

For `simoningram.com`:
1. Buy domain (~$12/year at Porkbun, Namecheap, or Cloudflare)
2. Point to hosting service (see above)

## Design Philosophy

- Minimal HTML/CSS only
- No JavaScript needed
- Works in all browsers
- Fast loading
- Sustainable for 20+ years
- Inspired by: ambiancejeune.com, simplifier.neocities.org

## Customization

### Colors
Edit `style.css`:
- `.work-number`: Line numbers color
- `.work-title`: Project title color
- `.work-meta`: Metadata (year, place) color

### Content
- Edit `index.html` to update project list
- Edit individual project pages
- Add images by replacing `<div class="placeholder-image"></div>` with:
  `<img src="yourimage.jpg" alt="Description">`

## Notes

- All files are static HTML - no database
- Change dates/info directly in HTML files
- Add new projects by creating new .html file and adding to index.html list
- For videos: upload to Vimeo/YouTube and embed with iframe
