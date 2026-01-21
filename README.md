# Interactive Housing Story

Materials for Open House #1 - January 21, 2026

> **Note:** This is a **separate git repository** from the main Western Spaces repo. When making changes, ensure you're in this directory:
> ```
> cd "/Users/sarah/Documents/Western Spaces/Archuletta County/HAP/Engagement/Session One/Interactive_Story"
> ```
> The parent `Western Spaces` folder has its own repo that ignores this directory.

---

## Quick Links

| Resource | URL |
|----------|-----|
| **Live Interactive Story** | https://westernspaces.github.io/archuleta-housing-story/housing_story.html |
| **GitHub Repo** | https://github.com/WesternSpaces/archuleta-housing-story |
| **Formspree Dashboard** | https://formspree.io/ (form ID: `xreepgko`) |

---

## What's Here

```
Interactive_Story/
├── housing_story.html       # Main interactive page (deployed to GitHub Pages)
├── story_content.md         # Source content for all 6 chapters
├── print_handout.html       # Tri-fold handout (print-ready)
├── print_response_card.html # Response cards, 2-up (print-ready)
├── qr_housing_story.png     # QR code linking to live page
├── DEPLOY.md                # Detailed deployment documentation
├── README.md                # This file
└── images/
    ├── hap_framework.svg    # HAP components diagram (not currently used)
    ├── 01_affordability_gap.png
    └── 02_housing_need_by_income.png
```

---

## The Story

An interactive narrative following 5 households through the housing crisis:

1. **Anna** - Healthcare worker, can't afford rent ($1,050/mo gap)
2. **Mike & Jenny** - Young family, can't find a home to buy ($168,500 gap)
3. **Linda & Tom** - Retirees wanting to downsize, limited options
4. **Pat & Chris** - Restaurant owners, can't find workers (employer perspective)
5. **Sam** - Seasonal worker facing housing instability

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

### Chapter Colors
Each chapter has a distinct color used in both the navigation and section borders:

| Chapter | Color | Hex | Theme |
|---------|-------|-----|-------|
| 1 - Community | Cyan | `#0e7490` | Meet the households |
| 2 - The Math | Blue | `#2563eb` | Affordability gap |
| 3 - Impact | Orange | `#d97706` | Economic effects |
| 4 - Current Work | Green | `#059669` | Resources & programs |
| 5 - Your Turn | Purple | `#7c3aed` | Reflection & input |
| 6 - Next Steps | Gold | `#FACE6A` | Timeline & process |

### Base Colors

| Color | Hex | Use |
|-------|-----|-----|
| Slate | `#2D3E4F` | Headers, primary |
| Gold | `#FACE6A` | Accents, highlights |
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

- `/Reference Documents/Archuleta_County_HNA.md` - **HNA converted to markdown** (full text, searchable)
- `/Reference Documents/Archuleta County HNA - Final 04 08 2025.docx` - Original HNA document
- `/Engagement/Session One/Story_Guide_Handout.md` - Original handout content spec
- `/Engagement/Session One/Story_Response_Card.md` - Original response card spec
- `/Engagement/Session One/Open_House_1_Planning.md` - Original planning doc

---

## Changelog

### January 20, 2026 - Pre-Event UX Improvements

**Content fixes (from coworker feedback):**
- Added "Subsidized housing" definition (distinct from "Affordable housing")
- Spelled out "Certified Nursing Assistant (CNA)" in Anna's profile
- Added tenure split explanation in "Dig Deeper: Housing Need by 2035"
- Fixed sentence fragment in Section 3 intro
- Updated inventory table: removed Timberline, added Archuleta Housing Inc. (173 total units)
- Updated pipeline table: Timberline now shows "2025-2026" (not "Now in inventory")
- Updated Pat & Chris section: Timberline as separate bullet item

**UX improvements (from fresh review against UX guide):**
- Fixed timeline: Strategy Group Sessions now shows as in-progress (was incorrectly marked complete)
- Added "Not sure" option to all 12 rating buttons (urgency + objectives)
- Reworded similar open questions for clarity:
  - "What's Being Missed?" (awareness/understanding)
  - "If You Could Focus on One Thing..." (action/priority)
- Replaced alert() with inline success message after form submission
- Added privacy statement in submit section
- Added "I'm not sure housing is a major problem here" option for skeptics
- Added Western Spaces (Sarah Brown McClain) credit in footer

**Reference documents:**
- `UX_Guide_Public_Engagement.md` - UX best practices for civic engagement (used for this review)

### January 18, 2026 - Final Pre-Event Updates

**Response Card (`print_response_card.html`):**
- Restructured for proper double-sided printing (Page 1: both fronts, Page 2: both backs)
- Updated Sam's icon to 🏕 (tent) with red background to match canonical materials
- Changed "Restaurant owners" to "Business owners" for Pat & Chris
- Added dashed cut line between cards
- Tightened layout to fit 2 cards per page

**Chapter 4 - Resources:**
- Moved Housing Choice Vouchers from Anna's section to Sam's section (Sam more likely to qualify)

**Print & Sidebar:**
- Added print style to hide chapter navigation when printing
- Removed "Your reflections" section from sidebar (open-ended text cluttered the summary)

### January 18, 2026 - Seven Objectives Update

**Chapter 5 - Your Turn:**
- Changed from 6 to 7 draft objectives
- Added new objective #2: "Serve a Range of Income Levels — 43% of households below 80% AMI"
- Renumbered existing objectives 2-6 to become 3-7
- Updated JavaScript to track new objective (obj_income)
- Updated form submission to include obj_income_range field

**Seven Draft Objectives (Final):**
1. Support Workforce Stability — Help employers recruit and retain workers
2. Serve a Range of Income Levels — 43% of households below 80% AMI
3. Expand Rental Supply — Address the 0.5% vacancy rate
4. Enable Homeownership — Bridge the affordability gap for buyers
5. Preserve Existing Affordable Housing — Protect what we have
6. Protect Residents from Displacement — Keep longtime residents housed
7. Maximize Limited Resources — Target public funds effectively

### January 18, 2026 - Open House #1 Final Updates

**Title & Style:**
- Changed title from "The Housing Story" to "Our Housing Story"
- Changed "Key definitions:" to "Definitions:" per style guide

**Navigation & UX:**
- Added "Start" (↑) button to chapter nav for jumping back to top
- Moved "How to use this story" instructions to very top (before About section)
- Added color coding to all chapter nav buttons (see Color Palette section)
- Added "(tap to close)" hint that appears when info sections are expanded

**Chapter 2 - The Math:**
- Changed table headers: "Affordable" → "Max Affordable", "Market" → "Median Market"
- Changed Sam's gap from "No options" to "Very limited" (acknowledges Housing Solutions SW helps ~5/year)

**Chapter 3 - Impact:**
- Removed "Dig Deeper: Employment Data" section (redundant with existing content)

**Chapter 4 - Inventory (Critical):**
- Updated to match printed boards (171 total units):
  - Removed Housing Choice Vouchers (rental assistance, not physical units)
  - Rose Mountain Townhomes: 34 units
  - Hickory Ridge Apartments: 40 units (was 41)
  - Archuleta Housing for Elderly: 12 units, 0-30% AMI
  - Casa de los Arcos: 16 units
  - Socorro Senior Living: 19 units (was 12)
  - Timberline Apartments: 50 units, LIHTC 30-80% AMI (Coming soon)
- Updated pipeline: Timberline now shows "Now in inventory"

**Chapter 5 - Your Turn:**
- Added "Anything Else?" open-ended comment field
- Form submission updated to capture new field

### January 17, 2026 - Round 4 Updates

**Content & Accuracy:**
- Fixed Housing Need methodology description (now accurately describes catch-up + keep-up methodology from HNA)
- Converted HNA from .docx to markdown (`/Reference Documents/Archuleta_County_HNA.md`)
- Updated HNA and HAP descriptions with comprehensive explanations
- Changed section title from "Meet Your Neighbors" to "Meet the Community"

**AMI Section:**
- Added "Category" column to AMI table (Moderate Income, Area Median, etc.)
- Removed 5-person and 6-person columns
- Spelled out "U.S. Department of Housing and Urban Development (HUD)"
- Added context: AMI varies by county, used for funding programs

**Survey Updates:**
- Added "None of these stories are familiar to me" option
- Changed employer question to be more inclusive

**Visual Changes:**
- Changed red stat boxes to slate blue (#2D3E4F)
- Added 30% affordability standard explanation to Section 2 intro

**Bug Fixes:**
- Fixed dig deeper toggles not expanding in correct location (moved content divs to follow buttons)

### January 17, 2026 - Round 5 Updates

**Household Profiles:**
- Added jobs to Mike & Jenny intro (Jenny is deputy sheriff, Mike teaches middle school)
- Changed Linda's career from teacher to Forest Service (avoid duplicate teachers)
- Clarified Pat & Chris "can't find workers for their restaurant"
- Added "example households" language to clarify these are representative, not real people

**Section 3 - Community Impact:**
- Improved Employment Data dig deeper with narrative framing and data table
- Improved Who's Most Affected with prominent rent/home price stats and industry explanation
- Added reminder of who Pat & Chris are in intro paragraph
- Removed editorializing ("The worker, the business, and the community all lose")

**Section 5 - Your Turn:**
- Added visual separation between questions (question-card styling)
- Bolded all question text for consistency
- Added missing h3 heading for "What Matters Most" question

**Survey/Tally Updates:**
- Added "I haven't seen these impacts" option to affordability question
- Added "What brings you here" to Your Story So Far tally
- Added objective priorities to Your Story So Far tally

**Style Guide Compliance:**
- Spelled out all currency amounts ($385K → $385,000, etc.)
- Verified all household income/AMI calculations against HNA data

---

*Last updated: January 20, 2026 (pre-event UX improvements)*
