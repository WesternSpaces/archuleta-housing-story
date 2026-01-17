# Interactive Housing Story

Materials for Open House #1 - January 21, 2026

---

## Quick Links

| Resource | URL |
|----------|-----|
| **Live Interactive Story** | https://westernspaces.github.io/archuleta-housing-story/housing_story.html |
| **GitHub Repo** | https://github.com/WesternSpaces/archuleta-housing-story |
| **Formspree Dashboard** | https://formspree.io/ (form ID: `xzznvopz`) |

---

## What's Here

```
Interactive_Story/
├── housing_story.html      # Main interactive page (deployed to GitHub Pages)
├── story_content.md        # Source content for all 6 chapters
├── print_handout.html      # Tri-fold handout (print-ready)
├── print_response_card.html # Response cards, 2-up (print-ready)
├── qr_housing_story.png    # QR code linking to live page
├── DEPLOY.md               # Detailed deployment documentation
└── README.md               # This file
```

---

## The Story

An interactive narrative following 4 households through the housing crisis:

1. **Maria** - Healthcare worker, can't afford rent ($1,733/mo gap)
2. **The Garcias** - Young family, can't find a home to buy ($203,500 gap)
3. **The Rodriguezes** - Restaurant owners, can't find workers (employer perspective)
4. **Robert** - Retiring teacher, can't find a place to downsize

This restores the **employer perspective** missing from Echo's boards and uses **correct HNA data** (median rent $2,783, not the lower averages).

---

## Printing Materials

### Tri-fold Handout (`print_handout.html`)

- **Size:** Letter (8.5" x 11")
- **Orientation:** Landscape
- **Paper:** 80-100lb text weight
- **Quantity:** 50-75 copies
- **Folding:** Fold right panel over center, then left panel on top

**To print:**
1. Open `print_handout.html` in browser
2. Cmd+P (Mac) or Ctrl+P (Windows)
3. Set orientation to **Landscape**
4. Print or Save as PDF

### Response Cards (`print_response_card.html`)

- **Size:** Letter, cut in half horizontally (makes 5.5" x 8.5" cards)
- **Orientation:** Portrait
- **Paper:** 65-80lb cardstock (uncoated, easier to write on)
- **Quantity:** 100+ copies
- **Double-sided:** Front = household icons to circle; Back = open question + QR

**To print:**
1. Open `print_response_card.html` in browser
2. Cmd+P (Mac) or Ctrl+P (Windows)
3. Keep Portrait orientation
4. Enable double-sided printing
5. Print on cardstock
6. Cut sheets in half horizontally

---

## Making Updates

### Update the interactive story:

```bash
cd "/Users/sarah/Documents/Western Spaces/Archuletta County/HAP/Engagement/Session One/Interactive_Story"

# Edit housing_story.html

# Commit and push
git add housing_story.html
git commit -m "Update: description of changes"
git push
```

Changes go live in 1-5 minutes.

### Regenerate QR code:

```bash
qrencode -o qr_housing_story.png -s 10 "https://westernspaces.github.io/archuleta-housing-story/housing_story.html"
```

---

## Form Submissions

Responses submitted through the interactive story go to **sarah@westernspaces.co** via Formspree.

**To check submissions:**
1. Go to https://formspree.io/
2. Sign in
3. View form `xzznvopz`

**Form captures:**
- Which households resonate (checkboxes)
- Personal experience notes
- Employer perspective (if applicable)
- "One thing for decision-makers" response
- Email (optional)

---

## Color Palette

Matches Echo's boards:

| Color | Hex | Use |
|-------|-----|-----|
| Teal | `#0d6b6e` | Headers, primary accent |
| Gold | `#c9a227` | Secondary accent, highlights |
| Orange | `#d97706` | Tertiary accent |
| Light BG | `#f5f7f5` | Page background |
| Dark text | `#1a1a1a` | Body text |

---

## Key Data (from HNA)

These are the correct figures - verify any updates against the HNA:

| Metric | Value | Source |
|--------|-------|--------|
| Median rent | $2,783/mo | HNA p. 45 |
| Median home price | $553,500 | HNA p. 52 |
| Rental vacancy | 0.5% | HNA p. 41 |
| Cost-burdened households | 44-48% | HNA p. 58 |
| Rent increase since 2012 | +57% | HNA p. 46 |
| Home price increase since 2020 | +56% | HNA p. 53 |
| Employers citing housing barrier | 60% | HNA p. 72 |
| Positions unfilled at peak | 17% | HNA p. 73 |
| Jobs per working household | 3.5 | HNA p. 74 |
| Workers commuting in | 1,456 | HNA p. 75 |

---

## Event Day Checklist

### Materials
- [ ] Printed handouts (50-75)
- [ ] Printed response cards (100+)
- [ ] QR code poster/table tent
- [ ] Response card collection box

### Setup
- [ ] QR codes visible at welcome table
- [ ] Response cards at each board station
- [ ] Collection box labeled at exit
- [ ] Test QR scan on-site

### After Event
- [ ] Collect response cards
- [ ] Check Formspree for digital submissions
- [ ] Compile input for analysis

---

## Troubleshooting

**QR code not scanning:**
- Print larger (at least 1.5" square)
- Ensure adequate lighting
- Test on multiple devices

**Page not loading:**
- Check GitHub Pages status
- Clear browser cache
- Wait 5 minutes after any push

**Form not submitting:**
- Check Formspree quota (free tier: 50/month)
- Verify form ID in HTML
- Check browser console for errors

---

## Related Files

- `/Engagement/Session One/Story_Guide_Handout.md` - Original handout content spec
- `/Engagement/Session One/Story_Response_Card.md` - Original response card spec
- `/Engagement/Session One/Open_House_1_Planning.md` - Original planning doc
- `/Reference Documents/Archuleta County HNA - Final 04 08 2025.docx` - Source data

---

*Last updated: January 17, 2026*
