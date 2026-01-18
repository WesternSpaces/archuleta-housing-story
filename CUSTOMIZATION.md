# Interactive Housing Story - Customization Guide

This guide explains how to adapt the interactive housing story for a different county or project.

## Quick Start

1. Copy `housing_story_template.html` to a new file (e.g., `housing_story.html`)
2. Find and replace all `{{PLACEHOLDER}}` values with your project data
3. Update the Formspree endpoint or replace with your own form handler
4. Test locally, then deploy

---

## Placeholder Reference

### Project & Location

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{COUNTY_NAME}}` | County name | Archuleta County |
| `{{TOWN_NAME}}` | Town/city name (if applicable) | Town of Pagosa Springs |
| `{{REGION_NAME}}` | Combined name for joint projects | Archuleta County & Town of Pagosa Springs |
| `{{STATE}}` | State | Colorado |

### Dates & Timeline

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{HNA_COMPLETION_DATE}}` | When needs assessment was completed | April 2025 |
| `{{STRATEGY_GROUP_DATES}}` | Strategy group session period | Jan-Mar 2026 |
| `{{OPEN_HOUSE_1_DATE}}` | First open house date | January 21, 2026 |
| `{{OPEN_HOUSE_2_DATE}}` | Second open house date | Spring 2026 |
| `{{PLAN_ADOPTION_DATE}}` | Target adoption date | Fall 2026 |

### AMI Data (from CHFA or HUD)

| Placeholder | Description |
|-------------|-------------|
| `{{AMI_100_2PERSON}}` | 100% AMI for 2-person household |
| `{{AMI_[LEVEL]_[SIZE]PERSON}}` | Pattern: AMI level (30/50/80/100/120) + household size (1-6) |

**Full AMI table placeholders:**
- `{{AMI_120_1PERSON}}` through `{{AMI_120_6PERSON}}`
- `{{AMI_100_1PERSON}}` through `{{AMI_100_6PERSON}}`
- `{{AMI_80_1PERSON}}` through `{{AMI_80_6PERSON}}`
- `{{AMI_50_1PERSON}}` through `{{AMI_50_6PERSON}}`
- `{{AMI_30_1PERSON}}` through `{{AMI_30_6PERSON}}`

### Housing Market Data

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{MEDIAN_RENT}}` | Median monthly rent | $2,783 |
| `{{MEDIAN_HOME_PRICE}}` | Median home sale price | $553,500 |
| `{{RENTAL_VACANCY_RATE}}` | Rental vacancy rate | 0.5% |
| `{{COST_BURDENED_PERCENT}}` | % of households cost-burdened | 44-48% |
| `{{RENT_INCREASE_PERCENT}}` | Rent increase since base year | 57% |
| `{{RENT_INCREASE_SINCE}}` | Base year for rent increase | 2012 |
| `{{HOME_PRICE_INCREASE_PERCENT}}` | Home price increase since base year | 56% |
| `{{HOME_PRICE_INCREASE_SINCE}}` | Base year for price increase | 2020 |

### Demographics

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{AVG_HOUSEHOLD_SIZE}}` | Average household size | 2.3 |
| `{{MEDIAN_AGE}}` | Median age | 51 |
| `{{STATE_MEDIAN_AGE}}` | State median age for comparison | 37 |
| `{{PERCENT_65_PLUS}}` | % of residents 65+ | 27% |
| `{{PERCENT_BELOW_80_AMI}}` | % of households below 80% AMI | 43% |
| `{{HOUSEHOLDS_BELOW_80_AMI}}` | Number of households below 80% AMI | 2,637 |

### Employment Data

| Placeholder | Description | Example |
|-------------|-------------|---------|
| `{{TOTAL_JOBS}}` | Total jobs in area | 7,523 |
| `{{PROJECTED_JOBS}}` | Projected jobs | 8,069 |
| `{{PROJECTED_JOBS_YEAR}}` | Year for projection | 2034 |
| `{{JOBS_PER_HOUSEHOLD}}` | Jobs per working household ratio | 3.5 |
| `{{COMMUTERS_IN}}` | Workers commuting in daily | 1,456 |
| `{{PERCENT_COMMUTERS}}` | % of workforce commuting in | 20% |
| `{{EMPLOYERS_HIRING_HARDER}}` | % employers saying hiring is harder | 63% |
| `{{EMPLOYERS_HOUSING_BARRIER}}` | % citing housing as #1 barrier | 60% |
| `{{POSITIONS_UNFILLED}}` | % positions unfilled at peak | 17% |

### Housing Need Projections

| Placeholder | Description |
|-------------|-------------|
| `{{NEED_30_TOTAL}}` | Units needed at ≤30% AMI |
| `{{NEED_30_RENTAL}}` | Rental units at ≤30% AMI |
| `{{NEED_30_OWNER}}` | Ownership units at ≤30% AMI |
| `{{NEED_50_TOTAL/RENTAL/OWNER}}` | Units at 31-50% AMI |
| `{{NEED_80_TOTAL/RENTAL/OWNER}}` | Units at 51-80% AMI |
| `{{NEED_100_TOTAL/RENTAL/OWNER}}` | Units at 81-100% AMI |
| `{{NEED_120_TOTAL/RENTAL/OWNER}}` | Units at 100-120% AMI |
| `{{NEED_TOTAL}}` | Total units needed |
| `{{NEED_RENTAL_TOTAL}}` | Total rental units needed |
| `{{NEED_OWNER_TOTAL}}` | Total ownership units needed |

### Existing Resources (customize sections entirely)

These sections should be rewritten for each community:
- Existing affordable housing inventory
- Current programs (vouchers, DPA, etc.)
- Pipeline projects
- Local organizations

### Form Submission

| Placeholder | Description |
|-------------|-------------|
| `{{FORMSPREE_ENDPOINT}}` | Formspree form URL |
| `{{CONTACT_EMAIL}}` | Contact email address |

---

## Household Stories

The five household archetypes can be customized but follow this pattern:

1. **The Essential Worker** (Anna) - ~50% AMI, single, renter, healthcare/service worker
2. **The Working Family** (Mike & Jenny) - ~100% AMI, family with kids, trying to buy
3. **The Retirees** (Linda & Tom) - ~80% AMI, want to downsize, aging in place
4. **The Employers** (Pat & Chris) - Business owners struggling to hire due to housing
5. **The Unstable** (Sam) - Seasonal/variable income, housing instability, limited options

For each household, update:
- Name(s) and occupation(s)
- Income and AMI level
- Specific situation/story
- Affordability calculations (Max Affordable vs Median Market)

---

## Chapter Structure & Colors

The story has 6 chapters plus an About section. Each chapter has a distinct color used in the navigation and section borders:

| Chapter | Class | Color | Hex |
|---------|-------|-------|-----|
| 1 - Meet the Community | `community` | Cyan | `#0e7490` |
| 2 - The Math | `math` | Blue | `#2563eb` |
| 3 - Impact | `economic` | Orange | `#d97706` |
| 4 - Current Work | `resources` | Green | `#059669` |
| 5 - Your Turn | `reflection` | Purple | `#7c3aed` |
| 6 - Next Steps | `next` | Gold | `#FACE6A` |

To customize colors, update:
1. CSS classes `.chapter-section.[class]` for border colors
2. CSS classes `.chapter-section.[class] .chapter-number` for number badges
3. CSS classes `.chapter-nav a.nav-[class]` for navigation buttons
4. HTML classes on `<section>` elements and `<nav>` links

### Navigation Features

The chapter navigation includes:
- **Start button** (↑) - jumps back to top of page
- **Color-coded chapter buttons** - match section themes
- **Hover labels** - show chapter names on hover
- **Active state** - highlights current section while scrolling

---

## Data Sources

Typical sources for placeholder values:

| Data Type | Source |
|-----------|--------|
| AMI limits | CHFA Income Limits (chfainfo.com) or HUD |
| Market data | Housing Needs Assessment |
| Demographics | Census, ACS, HNA |
| Employment | BLS, employer surveys, HNA |
| Housing need projections | Housing Needs Assessment |
| Pipeline projects | Local planning departments |
| Existing programs | Housing authority, local nonprofits |

---

## Formspree Setup

1. Create account at formspree.io
2. Create new form
3. Copy the form endpoint URL
4. Replace `{{FORMSPREE_ENDPOINT}}` in template

The form submits these fields:
- `name`, `email`
- `familiar_households` (comma-separated)
- `gap_experience` (comma-separated)
- `housing_impact` (comma-separated)
- `knew_programs` (comma-separated)
- `who_are_you` (comma-separated)
- `urgent_rental`, `urgent_homeownership`, `urgent_senior`, `urgent_workforce`, `urgent_emergency` (low/medium/high)
- `obj_workforce`, `obj_rental`, `obj_ownership`, `obj_preserve`, `obj_displacement`, `obj_resources` (low/medium/high)
- `experience`, `one_thing`, `anything_else` (text)

---

## Deployment

### GitHub Pages
1. Create repository
2. Push files
3. Enable GitHub Pages in repo settings
4. Site will be at `https://[username].github.io/[repo-name]/`

### Other hosting
The file is a single static HTML file with no dependencies. It can be hosted anywhere that serves HTML.

---

## Checklist

Before deploying, verify:

- [ ] All `{{PLACEHOLDER}}` values replaced
- [ ] AMI table has correct local data
- [ ] Household stories reflect local situations
- [ ] Pipeline projects are current
- [ ] Existing programs/resources are accurate
- [ ] Contact email is correct
- [ ] Formspree endpoint is set up and working
- [ ] Tested on mobile device
- [ ] All expandable sections work
- [ ] Form submission works
