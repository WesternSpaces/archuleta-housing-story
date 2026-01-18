# UX Guide for Public Engagement

**Western Spaces — Digital Engagement Design Reference**

*Last updated: January 18, 2026*

---

This guide synthesizes research from Nielsen Norman Group, federal plain language guidelines, WCAG accessibility standards, and civic engagement best practices. Use it as a reference when designing interactive stories, surveys, and digital engagement tools for community planning projects.

---

## Contents

1. [Know Your Audience](#1-know-your-audience)
2. [Plain Language](#2-plain-language)
3. [Visual Design](#3-visual-design)
4. [Forms & Surveys](#4-forms--surveys)
5. [Navigation & Page Structure](#5-navigation--page-structure)
6. [Mobile Considerations](#6-mobile-considerations)
7. [Accessibility Essentials](#7-accessibility-essentials)
8. [Legal Requirements](#8-legal-requirements)
9. [Quick Reference Checklist](#9-quick-reference-checklist)

---

## 1. Know Your Audience

### Older Adults (65+)

Users aged 65+ are **43% slower** at completing web tasks than younger users. This isn't a failure of the user — it's a design opportunity.

**Common challenges:**
- **Vision changes** — Reduced contrast sensitivity, smaller text harder to read
- **Motor control** — Smaller targets harder to tap/click, especially on touch screens
- **Unfamiliar patterns** — Dropdowns, sliders, and gestures may not be intuitive
- **Cognitive load** — More steps = more chances to lose the thread

**Design responses:**
- Larger text (minimum 16px body, prefer 18px+)
- High contrast (4.5:1 minimum, aim higher)
- Generous tap targets (minimum 44x44px)
- Avoid dropdowns and sliders when possible
- Define jargon inline — don't assume familiarity with terms like "AMI" or "cost-burdened"

> "The internet is unfriendly to people with bad eyesight." — NN/g study participant

**Source:** [Usability for Older Adults: Challenges and Changes](https://www.nngroup.com/articles/usability-for-senior-citizens/) — Nielsen Norman Group

---

### Mixed Digital Literacy

Over **50% of U.S. adults** score below international literacy benchmarks. Roughly 20% score at the lowest levels. These aren't edge cases — they're your audience.

**Implications:**
- Don't assume people know how to use common UI patterns
- Provide clear affordances (buttons should look like buttons)
- Use progressive disclosure — show basics first, details on demand
- Test with real users who aren't tech-comfortable

**Source:** [An Introduction to Plain Language](https://digital.gov/resources/an-introduction-to-plain-language) — Digital.gov

---

### Civic Engagement Context

Public engagement has different goals than commercial UX. You're not optimizing for conversion — you're building trust and gathering meaningful input.

**Key principles:**
- **Treat people as citizens, not consumers** — They're participating in democracy, not shopping
- **Transparency** — Be clear about what you're asking and why
- **Reciprocity** — Show how input will be used; close the feedback loop
- **Inclusivity** — Digital participation should complement, not replace, in-person options

> "The goal of civic participation is to reveal the conclusions people reach when they are informed about the issues and have the opportunity and motivation seriously to discuss them."

**Digital platforms reach different people than in-person meetings.** Traditional meetings attract those with time, transportation, and existing engagement. Digital tools can reach working parents, shift workers, people with mobility limitations, and others who can't attend a Tuesday evening meeting.

**Source:** [A Framework for Digital Civic Infrastructure](https://ash.harvard.edu/resources/a-framework-for-digital-civic-infrastructure/) — Harvard Ash Center

---

## 2. Plain Language

Plain language is **required by federal law** (Plain Writing Act of 2010) and is simply good practice for any public-facing content.

### Core Principles

| Do | Don't |
|----|-------|
| Use common, everyday words | Use jargon or technical terms without explanation |
| Write short sentences (15-20 words) | Write long, complex sentences |
| Use active voice | Use passive voice |
| Address the reader directly ("you") | Write in third person ("residents should...") |
| Put the most important information first | Bury the key point |
| Use headings and bullet points | Write dense paragraphs |

### Readability Targets

- **8th grade reading level** is a common target for public communications
- Use tools like Hemingway Editor or readable.com to check
- Shorter is almost always better

### Defining Terms

When you must use technical terms:
- Define them on first use
- Consider a glossary or "info" toggles
- Repeat definitions — don't assume people read linearly

**Example:**
> "Area Median Income (AMI) is the midpoint of household incomes in an area — half of households earn more, half earn less."

**Source:** [Federal Plain Language Guidelines](https://www.plainlanguage.gov/) — plainlanguage.gov

---

## 3. Visual Design

### Contrast Requirements (WCAG)

| Text Type | Minimum Contrast Ratio |
|-----------|----------------------|
| Normal text (<24px) | 4.5:1 |
| Large text (24px+ or 19px+ bold) | 3:1 |
| UI components (buttons, inputs) | 3:1 |

**Check your colors:** [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/)

**Common failures:**
- Light gray text on white backgrounds
- Colored text on colored backgrounds
- Placeholder text in form fields (often too light)

### Typography

| Element | Recommendation |
|---------|---------------|
| Body text | 16px minimum, 18px+ preferred |
| Line height | 1.5 to 1.6 |
| Line length | 50-75 characters per line |
| Font choice | Sans-serif for screen (Arial, Open Sans, etc.) |

**Avoid:**
- All caps for body text (harder to read)
- Justified text (creates uneven spacing)
- Decorative fonts for content

### Tap Targets

- **Minimum 44x44 pixels** for any tappable element
- Add padding around links in text
- Space interactive elements apart (minimum 8px gap)

**Source:** [Understanding Accessible Fonts and Typography](https://www.section508.gov/develop/fonts-typography/) — Section508.gov

---

## 4. Forms & Surveys

### Reduce Cognitive Load

NN/g's **EAS Framework:**
1. **Eliminate** — Remove unnecessary questions
2. **Automate** — Pre-fill what you can
3. **Simplify** — Make what remains as easy as possible

### Question Design

**One thing at a time.** Avoid "double-barreled" questions:
- Bad: "How satisfied are you with the content and design?"
- Good: "How satisfied are you with the content?" (separate question for design)

**Provide an opt-out.** Always include options like:
- "None of the above"
- "I'm not sure"
- "I haven't experienced this"

**Make most questions optional.** Forced completion causes abandonment and bad data.

### Layout

- **Single column only** — Multi-column forms confuse scanning patterns
- **Group related fields** with clear visual separation
- **Left-align labels** above fields (not to the side)
- **Make buttons look like buttons** — Clear, high-contrast, adequate size

### Rating Scales

- Use **balanced scales** (equal positive and negative options)
- Label all points, not just endpoints
- 5 points is usually sufficient; 7 maximum
- Consider semantic differential scales for nuanced attitudes

**Source:** [Website Forms Usability: Top 10 Recommendations](https://www.nngroup.com/articles/web-form-design/) — Nielsen Norman Group

---

## 5. Navigation & Page Structure

### The Fold Still Matters

**80% of attention** goes to content above the fold. Users do scroll, but only if what's visible is "promising enough."

**Implications:**
- Put your most important content first
- Avoid "false floors" — designs that look complete but aren't
- Don't fill prime real estate with decorative images

### Long Pages

Long pages can work well with proper structure:

| Pattern | When to Use |
|---------|-------------|
| **Mini table of contents** | Jump links at top showing page structure |
| **Sticky navigation** | Persistent access to sections |
| **Back-to-top button** | Easy return after scrolling |
| **Progress indicator** | Show position in multi-section content |
| **Accordions** | Progressive disclosure of detail |

### Accordions

Accordions work well for:
- FAQ-style content
- "Learn more" / "Dig deeper" expansions
- Keeping overview scannable while detail is available

**Best practices:**
- Clear visual affordance (chevron, +/- icon)
- Descriptive labels (not just "More")
- Consider starting some open if content is critical

**Source:** [Scrolling and Attention](https://www.nngroup.com/articles/scrolling-and-attention/) — Nielsen Norman Group

---

## 6. Mobile Considerations

### Mobile Users Are Different

- **Smaller screens** — Less visible at once, more scrolling
- **Touch interaction** — Fingers are less precise than cursors
- **Variable contexts** — Bright sun, one hand, distractions
- **Data constraints** — Some users have limited data plans

### Mobile-Specific Guidelines

| Element | Mobile Consideration |
|---------|---------------------|
| Tap targets | 44x44px minimum, with spacing |
| Text size | 16px minimum (prevents zoom on iOS) |
| Forms | Use appropriate input types (email, tel, number) |
| Images | Optimize file size; provide alt text |
| Tables | Make horizontally scrollable or reformat |

### Don't Just Shrink Desktop

Mobile-first design doesn't mean squeezing desktop content onto small screens. Consider:
- What's essential for the mobile user's goal?
- Can content be progressively disclosed?
- Are there mobile-specific needs (click-to-call, maps)?

**Source:** [The State of Mobile User Experience](https://www.nngroup.com/articles/state-mobile-ux/) — Nielsen Norman Group

---

## 7. Accessibility Essentials

Accessibility isn't just compliance — it's reaching your full audience.

### Quick Wins

1. **Alt text for images** — Describe the content and function
2. **Heading hierarchy** — Use H1, H2, H3 in order (don't skip levels)
3. **Link text** — Descriptive ("Read the full report") not generic ("Click here")
4. **Color isn't the only indicator** — Don't rely on color alone to convey meaning
5. **Keyboard navigation** — All interactive elements reachable via Tab key
6. **Focus indicators** — Visible outline when elements are focused

### Testing Tools

- **WAVE** — Browser extension for accessibility checking
- **Lighthouse** — Built into Chrome DevTools
- **WebAIM Contrast Checker** — For color combinations
- **Screen reader testing** — VoiceOver (Mac), NVDA (Windows)

### WCAG Levels

| Level | Description |
|-------|-------------|
| A | Minimum accessibility (legal baseline) |
| **AA** | Standard target for most organizations |
| AAA | Enhanced accessibility (not always achievable) |

**Source:** [WebAIM: Contrast and Color Accessibility](https://webaim.org/articles/contrast/) — WebAIM

---

## 8. Legal Requirements

Digital accessibility isn't just good practice — it's the law. This section covers requirements relevant to Western Spaces' work with Colorado local governments.

### The Legal Landscape

| Law/Rule | Applies To | Standard | Deadline |
|----------|-----------|----------|----------|
| **Section 508** | Federal agencies | WCAG 2.0 AA | Current |
| **ADA Title II** | State & local government | WCAG 2.1 AA | 2026-2027 |
| **Colorado HB 21-1110** | CO state & local government | WCAG 2.1 AA | July 1, 2024* |
| **DOJ 2024 Rule** | All state & local government | WCAG 2.1 AA | April 2026/2027 |

*Colorado deadline had grace period extension to July 1, 2025

---

### Colorado HB 21-1110

**Colorado was the first state to legally mandate website accessibility for state and local governments** (enacted June 30, 2021).

#### Who Must Comply

- All state government agencies
- All local governments (cities, counties, towns)
- Public K-12 schools and school districts
- Public colleges and universities
- Special districts

#### What's Covered

The law covers **all technology** that is public-facing OR internal-facing:
- Websites and web applications
- Mobile applications
- Documents (PDFs, Word docs, spreadsheets, presentations)
- Video and audio content
- Kiosks and digital signage
- Third-party tools procured by government entities

#### Technical Standard

**WCAG 2.1 Level AA** — This includes 50 specific success criteria covering:
- Text alternatives for images
- Captions and transcripts for media
- Keyboard accessibility
- Color contrast
- Resizable text
- Consistent navigation
- Error identification and suggestions

#### Compliance Path

Organizations can be **in compliance even if not perfectly accessible** if they:
1. Publish an accessibility statement
2. Provide two methods of contact for assistance requests
3. Are actively working toward full conformance

#### Enforcement & Penalties

- **No enforcement agency** — Compliance is enforced through courts
- Individuals can sue in Colorado court for discrimination
- Penalties: **$3,500 per violation** or actual monetary damages
- Courts can order remediation

**Sources:**
- [Colorado Digital Accessibility Law](https://oit.colorado.gov/accessibility-law) — Colorado OIT
- [HB 21-1110 FAQ](https://oit.colorado.gov/hb21-1110-faq) — Colorado OIT
- [Colorado's Accessibility Law (HB21-1110)](https://www.cuanschutz.edu/accessibility/digital-accessibility/colorado-law-hb21-1110) — CU Anschutz

---

### DOJ 2024 ADA Title II Rule

On April 24, 2024, the Department of Justice finalized a rule requiring **all state and local governments nationwide** to make websites and mobile apps accessible.

#### Technical Standard

**WCAG 2.1 Level AA** — Same as Colorado's requirement. Compliance means meeting all 50 success criteria.

> "Although WCAG includes the word 'guidelines,' complying with WCAG 2.1 Level AA is **required** under the rule."

#### Compliance Deadlines

| Entity Type | Population | Deadline |
|-------------|-----------|----------|
| General government | 50,000+ | **April 24, 2026** |
| General government | Under 50,000 | **April 26, 2027** |
| Special district (any size) | Any | **April 26, 2027** |

**Archuleta County** (population ~14,000) falls under the **April 26, 2027** deadline, but Colorado's HB 21-1110 has an earlier deadline.

#### What's Covered

- All web content (text, images, audio, video, interactive elements)
- Mobile applications
- Electronic documents
- Internal tools used by government employees
- Online services provided to the public

#### Exceptions

Limited exceptions exist for:
- **Archived content** not currently used for services
- **Pre-existing documents** (PDFs, Word docs, etc.) unless used to apply for or access services
- **Third-party content** posted by members of the public (with conditions)
- **Password-protected individualized documents**
- **Pre-existing social media posts**

> **Important:** Even when exceptions apply, governments must still provide accessible alternatives upon request.

#### Practical Implications for Consultants

When Western Spaces creates digital engagement tools for government clients:

1. **The tool should meet WCAG 2.1 AA** — This protects both the client and the participants
2. **Documents matter** — PDFs, handouts, and reports should be accessible
3. **Third-party content exception doesn't apply** — Content we create for governments isn't "third-party"
4. **Test before delivery** — Use automated tools + manual testing

**Sources:**
- [Fact Sheet: New Rule on Web Accessibility](https://www.ada.gov/resources/2024-03-08-web-rule/) — ADA.gov
- [First Steps Toward Compliance](https://www.ada.gov/resources/web-rule-first-steps/) — ADA.gov
- [DOJ Final Rule (Federal Register)](https://www.federalregister.gov/documents/2024/04/24/2024-07758/nondiscrimination-on-the-basis-of-disability-accessibility-of-web-information-and-services-of-state)

---

### Accessibility Statements

Both Colorado law and best practice call for publishing an **accessibility statement**. Include:

1. **Commitment statement** — Organization's commitment to accessibility
2. **Standard being followed** — "We aim to conform to WCAG 2.1 Level AA"
3. **Known limitations** — Any areas not yet fully accessible
4. **Contact information** — At least two ways to request assistance
5. **Feedback mechanism** — How to report accessibility issues
6. **Date** — When the statement was last updated

**Example language:**

> "We are committed to ensuring digital accessibility for people with disabilities. We are continually improving the user experience for everyone and applying the relevant accessibility standards. If you experience difficulty accessing any content or functionality, please contact us at [email] or [phone]. We will work with you to provide the information or service you need through an alternative communication method."

---

### Document Accessibility

Documents (PDFs, Word, Excel, PowerPoint) are covered under both Colorado and federal requirements.

#### Key Requirements

| Element | Requirement |
|---------|-------------|
| **Reading order** | Logical sequence for screen readers |
| **Headings** | Proper heading structure (H1, H2, H3) |
| **Alt text** | Descriptions for images and charts |
| **Tables** | Header rows identified; simple structure |
| **Links** | Descriptive link text |
| **Color** | Not sole means of conveying information |
| **Language** | Document language specified |

#### Creating Accessible PDFs

1. **Start accessible** — Create in Word/InDesign with proper structure
2. **Export correctly** — Use "Save as PDF" with accessibility options
3. **Check and remediate** — Use Adobe Acrobat's accessibility checker
4. **Test** — Verify with screen reader

#### Pre-existing Documents

Under the DOJ rule, pre-existing documents (created before compliance deadline) don't need to be remediated unless:
- Used to apply for, gain access to, or participate in services/programs
- Currently linked from the website

**Practical approach:** Prioritize high-traffic, high-impact documents first.

---

### Risk Assessment for Western Spaces

When creating digital engagement tools:

| Risk Level | Situation | Recommendation |
|------------|-----------|----------------|
| **Low** | Interactive story hosted on WS site, linked from client | Ensure WCAG 2.1 AA compliance |
| **Medium** | Tool embedded directly on government site | Same standard; coordinate with client IT |
| **Higher** | Documents provided for government distribution | Ensure document accessibility |

**Best practice:** Treat all government-adjacent work as requiring WCAG 2.1 AA compliance.

---

## 9. Quick Reference Checklist

Use this checklist when reviewing digital engagement tools:

### Content
- [ ] Language is plain and jargon-free (or jargon is defined)
- [ ] Reading level is appropriate (8th grade or below)
- [ ] Most important information comes first
- [ ] Headings create clear structure

### Visual Design
- [ ] Body text is 16px+ (18px+ preferred)
- [ ] Contrast ratio meets 4.5:1 for normal text
- [ ] Tap targets are 44x44px minimum
- [ ] Interactive elements are clearly distinguishable

### Forms & Surveys
- [ ] Single-column layout
- [ ] One question per question (no double-barreled)
- [ ] Opt-out options available
- [ ] Most questions are optional
- [ ] Buttons are clear and prominent

### Navigation
- [ ] Key content is above the fold
- [ ] Long pages have navigation aids (TOC, back-to-top)
- [ ] Accordions have clear labels and affordances
- [ ] Progress is visible on multi-section content

### Mobile
- [ ] Tested on actual mobile devices
- [ ] Text readable without zooming
- [ ] Forms use appropriate input types
- [ ] Tables are responsive or scrollable

### Accessibility
- [ ] Images have alt text
- [ ] Headings are hierarchical (H1 → H2 → H3)
- [ ] Links have descriptive text
- [ ] Color isn't the only indicator
- [ ] Keyboard navigation works
- [ ] Focus states are visible

### Legal Compliance (Colorado & Federal)
- [ ] Meets WCAG 2.1 Level AA standard
- [ ] Accessibility statement published (if government-hosted)
- [ ] Two contact methods for assistance requests
- [ ] Documents (PDFs, handouts) are accessible
- [ ] Alt text on all informational images
- [ ] Video/audio has captions or transcripts
- [ ] Tested with automated tool (WAVE, Lighthouse)
- [ ] Manual keyboard navigation test completed

---

## Additional Resources

### Research & Guidelines
- [Nielsen Norman Group](https://www.nngroup.com/) — Evidence-based UX research
- [plainlanguage.gov](https://www.plainlanguage.gov/) — Federal plain language guidelines
- [WebAIM](https://webaim.org/) — Web accessibility resources
- [WCAG 2.1 Guidelines](https://www.w3.org/WAI/WCAG21/quickref/) — W3C accessibility standards
- [U.S. Web Design System](https://designsystem.digital.gov/) — Federal design patterns

### Tools
- [Hemingway Editor](https://hemingwayapp.com/) — Readability checker
- [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/) — Color contrast tool
- [WAVE](https://wave.webaim.org/) — Accessibility evaluation tool
- [Lighthouse](https://developers.google.com/web/tools/lighthouse) — Chrome DevTools auditing

### Civic Engagement
- [Harvard Ash Center — Digital Civic Infrastructure](https://ash.harvard.edu/resources/a-framework-for-digital-civic-infrastructure/)
- [mySociety — State of Digital Public Engagement](https://research.mysociety.org/html/digital-public-engagement/)

### Legal & Compliance
- [Colorado Digital Accessibility Law](https://oit.colorado.gov/accessibility-law) — Colorado OIT
- [HB 21-1110 FAQ](https://oit.colorado.gov/hb21-1110-faq) — Colorado OIT
- [ADA.gov Web Accessibility Guidance](https://www.ada.gov/resources/web-guidance/) — DOJ
- [DOJ 2024 Rule Fact Sheet](https://www.ada.gov/resources/2024-03-08-web-rule/) — ADA.gov
- [Section 508 Standards](https://www.section508.gov/) — Federal accessibility requirements

---

*This guide is a living document. Update as new research emerges or project-specific learnings accumulate.*
