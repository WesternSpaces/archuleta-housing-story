# Deployment Guide
## Housing Story Interactive Page

This guide documents the deployed interactive housing story for the Open House.

---

## DEPLOYED

**Live URL:** https://westernspaces.github.io/archuleta-housing-story/housing_story.html

**Repository:** https://github.com/WesternSpaces/archuleta-housing-story

**QR Code:** `qr_housing_story.png` (included in this folder)

---

## Quick Reference

The page is live and ready to use. To make updates:

```bash
cd "/Users/sarah/Documents/Western Spaces/Archuletta County/HAP/Engagement/Session One/Interactive_Story"

# Make changes to housing_story.html

# Commit and push
git add housing_story.html
git commit -m "Update: description of changes"
git push
```

Changes will be live in 1-5 minutes.

---

## File Structure

```
archuleta-housing-story/
├── housing_story.html     # Main interactive page
├── story_content.md       # Source content (reference)
├── DEPLOY.md              # This file
└── README.md              # Optional: project description
```

---

## Generate QR Code

### Option 1: Free Online Generator

1. Go to https://www.qrcode-monkey.com/ or https://www.qr-code-generator.com/
2. Enter the GitHub Pages URL
3. Download PNG at high resolution (at least 300x300 px)
4. Test by scanning with your phone

### Option 2: Command Line (if qrencode installed)

```bash
# Install qrencode (macOS)
brew install qrencode

# Generate QR code
qrencode -o qr_housing_story.png -s 10 "https://westernspaces.github.io/archuleta-housing-story/housing_story.html"
```

---

## Formspree Setup

The HTML page uses Formspree for form submissions. Current configuration:
- Form ID: `xzznvopz`
- Sends to: sarah@westernspaces.co

### To Change the Form Endpoint

1. Go to https://formspree.io/ and sign in
2. Create a new form or use existing
3. Copy the form ID
4. In `housing_story.html`, find:
   ```javascript
   fetch('https://formspree.io/f/xzznvopz',
   ```
5. Replace `xzznvopz` with your new form ID

---

## Testing Checklist

Before the event, test the following:

### Mobile Testing
- [ ] Page loads on iPhone
- [ ] Page loads on Android
- [ ] Text is readable without zooming
- [ ] Checkboxes are tappable
- [ ] Sidebar collapses on mobile
- [ ] Form submission works

### QR Code Testing
- [ ] QR code scans correctly
- [ ] Opens to the right URL
- [ ] Test with multiple phones

### Form Testing
- [ ] Submit a test response
- [ ] Verify email received
- [ ] Check all fields are captured

### Print Testing
- [ ] Print page (Ctrl/Cmd + P)
- [ ] Verify sidebar is hidden
- [ ] Content fits on pages
- [ ] Submit button hidden

### Link Testing
- [ ] Email link works (sarah@westernspaces.co)
- [ ] HNA PDF link works (when added)

---

## Embedding in mypagosa

### Option A: Direct Link

Add a prominent link on the virtual open house page:
```html
<a href="https://westernspaces.github.io/archuleta-housing-story/housing_story.html" target="_blank">
  Explore the Interactive Housing Story
</a>
```

### Option B: Embed via iframe

```html
<iframe
  src="https://westernspaces.github.io/archuleta-housing-story/housing_story.html"
  width="100%"
  height="800"
  frameborder="0"
  title="Housing in Archuleta County: Follow the Story">
</iframe>
```

Note: iframe may have limitations depending on mypagosa's platform.

---

## Print Materials Preparation

### Story Guide Handout (Tri-fold)

1. Open `Story_Guide_Handout.md` for content
2. Create design in Canva:
   - Use template: Tri-fold brochure, Letter size
   - Apply color palette: teal (#0d6b6e), gold (#c9a227)
3. Add QR code (prominently on cover)
4. Export as PDF (Print quality)
5. Print 50-75 copies on 80lb text paper

### Story Response Card (Half-sheet)

1. Open `Story_Response_Card.md` for content
2. Create design in Canva:
   - 5.5" x 8.5" or postcard size
3. Add household icons in circles
4. Add QR code on back
5. Export as PDF
6. Print 100+ copies on cardstock

---

## Event Day Checklist

### Materials to Bring
- [ ] Printed handouts (50-75)
- [ ] Printed response cards (100+)
- [ ] QR code poster/table tent
- [ ] Response card collection box
- [ ] Signup sheet for email updates

### Setup
- [ ] QR codes visible at welcome table
- [ ] Response cards at each board station
- [ ] Collection box clearly labeled at exit
- [ ] Test QR scan on-site (WiFi may vary)

### After Event
- [ ] Collect response cards
- [ ] Check Formspree for digital submissions
- [ ] Compile input for analysis

---

## Troubleshooting

### QR Code Not Scanning
- Ensure adequate lighting
- Print QR at larger size (at least 1.5" square)
- Test on multiple devices

### Page Not Loading
- Check GitHub Pages is enabled
- Wait 5 minutes after deployment
- Clear browser cache

### Form Not Submitting
- Check Formspree quota (free tier: 50 submissions/month)
- Verify form ID in code
- Check browser console for errors

### Mobile Display Issues
- Clear cache and refresh
- Try different browser (Safari, Chrome)
- Check viewport meta tag in HTML

---

## Future Updates

To update the page after deployment:

```bash
# Make changes to housing_story.html

# Commit and push
git add housing_story.html
git commit -m "Update: description of changes"
git push
```

Changes will be live in 1-5 minutes.

---

## Contact

Questions about deployment: sarah@westernspaces.co

---

*Last updated: January 17, 2026*
