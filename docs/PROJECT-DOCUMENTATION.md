# Sudbury Supportive Housing - Project Documentation

## Complete Development Context & Strategy Guide

**Last Updated**: January 13, 2026  
**Project Status**: Active Development  
**Charity Registration**: #760828947RR0001

---

## Source Conversation Reference

**Claude.ai Conversation**: This documentation was generated from a Claude.ai conversation that included:

- Initial website development and design
- Comprehensive fact-checking against CBC News, Sudbury.com, and CRA databases
- Strategic analysis of 50+ nonprofit website archetypes
- Quick wins implementation (sticky donate, trust badges, partner verification)

The full conversation context is preserved in this document. For any questions about methodology or decisions made, this document serves as the authoritative reference.

---

## Table of Contents

1. [Executive Summary](#executive-summary)
2. [Organization Background](#organization-background)
3. [Website Files Overview](#website-files-overview)
4. [Fact-Check Report](#fact-check-report)
5. [Nonprofit Website Strategy Research](#nonprofit-website-strategy-research)
6. [Quick Wins Implementation](#quick-wins-implementation)
7. [Recommended Implementation Roadmap](#recommended-implementation-roadmap)
8. [Key Performance Indicators](#key-performance-indicators)
9. [Digital Asset Inventory](#digital-asset-inventory)
10. [Technical Notes](#technical-notes)

---

## Executive Summary

This repository contains the complete digital assets and documentation for **Sudbury Supportive Housing** (formerly Sudbury's Centre for Transitional Care / SCTC), a registered Canadian charity operating in Greater Sudbury, Ontario.

### Key Accomplishments Documented Here:

- **Comprehensive fact-checking** of all website content against CBC News, Sudbury.com, CRA databases, and official sources
- **Strategic analysis** of 50+ nonprofit website archetypes to inform optimization
- **Implementation of quick wins** including sticky donate buttons, CRA verification badges, trust indicators, and clickable partner verification links

### Verified Impact Statistics:

| Metric | Value | Source |
|--------|-------|--------|
| People housed | 40+ | CBC News, Sudbury.com |
| Applicants served | 180+ | Organization records |
| Reside units | 10 | Raising the Roof |
| People housed through Reside | 29 | Raising the Roof |
| Trainees employed | 31 | Community Builders |
| Properties renovated | 5 | Verified media coverage |

---

## Organization Background

### Legal Entity

- **Legal Name**: Sudbury's Centre for Transitional Care (transitioning to "Sudbury Supportive Housing")
- **Type**: Registered Canadian Charity (CRA)
- **Charity Number**: 760828947RR0001
- **Founded**: 2021
- **CRA Verification**: [apps.cra-arc.gc.ca](https://apps.cra-arc.gc.ca/ebci/hacc/srch/pub/dsplyBscSrch?q.srchNmFltr=sudbury+supportive+housing)

### Leadership

- **Founder & Executive Director**: Jehnna Morin (Associate Addictions Counsellor)

### Verified Partners

| Partner | Role | Verification |
|---------|------|--------------|
| Raising the Roof | Reside Program - 10-unit affordable housing | [raisingtheroof.org/what-we-do/reside](https://www.raisingtheroof.org/what-we-do/reside/) |
| City of Greater Sudbury | Municipal funding & service contracts | [greatersudbury.ca/live/housing](https://www.greatersudbury.ca/live/housing/) |
| Community Builders | Social enterprise construction training | [communitybuilderssudbury.com](https://www.communitybuilderssudbury.com/) |

### Historical Locations

| Address | Function | Status |
|---------|----------|--------|
| 495 Notre Dame Ave., Sudbury, ON P3C 5K9 | Drop-In Centre & Head Office | Closed Fall 2024 |
| 519 Notre Dame Ave., Sudbury, ON P3C 5L1 | Sober Living Apartments (18 units) | Closed Fall 2024 |
| 1517 Kingslea Ct. (Raising the Roof) | Reside affordable housing | Active |
| 1035 Bloor St. | Transitional housing | Active |
| 30 Ste Anne Road | 135-unit supportive housing (proposed) | In development |

---

## Website Files Overview

### File Structure

```
sudbury-supportive-housing/
├── index.html                    # Main homepage (86KB)
├── case-study-raising-roof.html  # Reside Program partnership (28KB)
├── case-study-bloor.html         # 1035 Bloor St. project (25KB)
├── case-study-ste-anne.html      # 30 Ste Anne Road development (22KB)
├── logo.png                      # Organization logo (8KB)
├── FACT-CHECK-REPORT.md          # Detailed fact-check documentation
└── PROJECT-DOCUMENTATION.md      # This file
```

### Key Features Implemented

- Responsive design (mobile-first)
- Sticky donate button with pulse animation
- CRA verification badge in footer
- Trust badges (CanadaHelps, Benevity, Reside Partner)
- Clickable partner logos with verification links
- Testimonial carousel (2 verified testimonials)
- Case study pages for each major project
- Impact statistics section
- News archive with verified sources

---

## Fact-Check Report

### Methodology

All claims in the website were verified against:

1. **Primary Sources**: CRA Charity Database, Raising the Roof official website, City of Greater Sudbury records
2. **Media Sources**: CBC News, Sudbury.com (verified journalist bylines)
3. **Public Records**: Municipal council meetings, Ontario Trillium Foundation grants

### Issues Identified & Corrected

| # | Issue | Original | Corrected | File |
|---|-------|----------|-----------|------|
| 1 | Timeline Date | "May 2023" | "April 2023" | case-study-raising-roof.html |
| 2 | Testimonial | Gail Spencer quote (unverifiable) | REMOVED | index.html |
| 3 | Testimonial | "Michael" Program Graduate (fabricated) | REMOVED | index.html |
| 4 | Service Claim | "24/7 Support Available" | "Ongoing Support Services" | index.html |
| 5 | Service Claim | "24/7 Support Available" | "On-Site Support Staff" | case-study-ste-anne.html |
| 6 | Partners | Unverified organizations listed | Removed (kept 3 verified) | index.html |

### Verified Claims Preserved

- Charity #760828947RR0001 ✓
- Phone 249-878-5544 ✓
- Address 495 Notre Dame Ave ✓
- Jehnna Morin Founder/ED ✓
- 180+ applicants ✓
- 40+ housed ✓
- 10 Reside units ✓
- 29 people housed through Reside ✓
- 31 trainees ✓
- 5 properties renovated ✓
- Mayor Paul Lefebvre quote ✓
- Leslie Bellingham quote ✓
- All news article dates ✓

### Testimonials Status

| Testimonial | Status | Source |
|-------------|--------|--------|
| Mayor Paul Lefebvre | ✓ VERIFIED | CBC News, Nov 2024 |
| Leslie Bellingham (Raising the Roof) | ✓ VERIFIED | CBC News, multiple articles |
| Gail Spencer | ✗ REMOVED | Quote unverifiable despite real person |
| "Michael" Program Graduate | ✗ REMOVED | Fabricated illustrative content |

---

## Nonprofit Website Strategy Research

### Research Methodology

Analyzed 50+ sources including:

- Webby Awards nonprofit winners
- CSS Design Awards - 50 Best Nonprofit Websites
- charity: water (benchmark for transparency)
- Habitat for Humanity (multi-pathway engagement)
- GuideStar/Candid (transparency seal impact data)
- Charity Navigator (donor trust metrics)
- BBB Wise Giving Alliance

### Five Nonprofit Website Outcome Archetypes

#### 1. TRANSPARENCY CHAMPION

**Primary Goal**: Build unshakeable donor trust through radical openness

**Exemplar**: charity: water (100% of public donations to projects, GPS coordinates of every well)

**Key Elements**:
- Third-party verification seals (GuideStar Platinum, Charity Navigator, BBB)
- Real-time impact dashboards
- Publicly accessible financials/990s
- Board member bios
- Proof points for every claim

**ROI Data**:
- Organizations with Gold/Platinum GuideStar seals viewed 2x more
- Receive 11% higher average donations
- Nonprofits with transparency seals average 53% more contributions

---

#### 2. STORY-DRIVEN CONVERTER

**Primary Goal**: Create emotional connection driving immediate action

**Exemplars**: Malala Fund, KidSport Canada, charity: water

**Key Elements**:
- Hero sections with beneficiary stories + professional photography
- "Someone Like You" personalization connecting donors to specific individuals
- Hope-focused narratives (not guilt-based)
- Video transformation journeys
- Every story ends with clear CTA

**ROI Data**:
- charity: water raised $260M+ since 2006 through hope-focused storytelling
- Donors feel like partners, not ATMs

---

#### 3. MULTI-PATHWAY ENGAGER

**Primary Goal**: Capture and nurture diverse audience segments

**Exemplars**: Habitat for Humanity, Boys & Girls Clubs ("I am a..." user journey selection)

**Key Elements**:
- Multiple entry points (Donor/Volunteer/Client/Partner/Media)
- Personalized pathways based on self-identification
- Graduated engagement (newsletter→volunteer→donate→major gift)
- "Not ready to donate?" alternatives
- Local affiliate finders

**ROI Data**:
- Habitat's ReStore model creates volunteer-to-donor pipelines
- Many volunteers become recurring donors

---

#### 4. CONVERSION OPTIMIZER

**Primary Goal**: Minimize friction, maximize donation completion rates

**Exemplars**: charity: water (homepage IS donation page), ASPCA (matching gift integration)

**Key Elements**:
- Donation button visible on every page (header + floating)
- Minimal form fields (only essentials)
- Pre-selected amounts with impact statements ("$20/month = one family served")
- Recurring giving emphasized ("Join The Spring" monthly program)
- Matching gift tools embedded in donation flow

**ROI Data**:
- Average nonprofit donation page abandonment: 50-70%
- Optimized forms with 3-5 fields achieve 19%+ conversion rates

---

#### 5. AUTHORITY BUILDER

**Primary Goal**: Establish thought leadership, attract institutional funding

**Exemplars**: National Alliance to End Homelessness, Candid

**Key Elements**:
- Research reports/white papers/data tools freely accessible
- Media/press section with downloadable assets
- Policy positions and advocacy toolkits
- Partnerships and awards prominently displayed
- SEO-optimized blog

**ROI Data**:
- 44% of nonprofit website visits from organic search
- Wonder Ink moved from 5 to 187 page-one keywords in 12 months through content strategy

---

### Key Statistics from Research

| Metric | Value | Source |
|--------|-------|--------|
| First impression based on design | 94% of consumers | Web design research |
| Donors need concrete impact info | 75% | Donor behavior studies |
| Nonprofit bounce rate | 60% (vs 40% general) | Industry benchmarks |
| Email vs. social media effectiveness | 40x | Nonprofit marketing data |
| Profiles with Gold/Platinum seals | 2x views, 11% higher donations | GuideStar |
| Organizations with transparency seals | 53% more contributions | Candid research |
| Average donation page conversion | 8-15% (optimized: 19%+) | Industry benchmarks |
| Donation page abandonment | 50-70% | Industry average |

---

### Recommended Strategy for Sudbury Supportive Housing

**PRIMARY ARCHETYPE**: Transparency Champion + Story-Driven Converter Hybrid

**Rationale**: Leverages existing strengths (verifiable charity status, Raising the Roof partnership, City relationship, documented outcomes) while building emotional connection needed to convert visitors into donors.

---

## Quick Wins Implementation

### Completed Implementations (January 2026)

#### 1. Sticky Donate Button (All Pages)

```css
.sticky-donate {
    position: fixed;
    bottom: 2rem;
    right: 2rem;
    z-index: 999;
    background: linear-gradient(135deg, var(--green), var(--green-dark));
    animation: pulse-glow 2s ease-in-out infinite;
}
```

- Fixed position bottom-right on all pages
- Animated pulse glow effect
- Mobile-responsive (smaller on mobile)
- Links to #donate section (index) or index.html#donate (case studies)

#### 2. CRA Verification Badge

- Green-highlighted badge in footer
- Links to CRA charity search for #760828947RR0001
- Provides instant donor verification
- Icon: Shield with checkmark

#### 3. Trust Badge Footer Section

All pages now include:

| Badge | Link | Purpose |
|-------|------|---------|
| CRA Verified | CRA charity search | Government verification |
| CanadaHelps | Donation platform profile | Third-party donation |
| Benevity | Workplace giving platform | Corporate matching |
| Reside Partner | Raising the Roof program page | Partnership verification |

#### 4. Clickable Partner Logos (index.html)

Partners section updated:

- **Heading**: "Our Verified Partners"
- **Subtitle**: "Click to verify our partnerships"
- External link icons appear on hover
- All links open in new tabs with `rel="noopener"`

| Partner | Verification Link |
|---------|------------------|
| Raising the Roof | raisingtheroof.org/what-we-do/reside/ |
| City of Greater Sudbury | greatersudbury.ca/live/housing/ |
| Community Builders | communitybuilderssudbury.com/ |

---

## Recommended Implementation Roadmap

### Phase 1: Transparency Foundation (2-4 Weeks)

- [x] Add charity registration badge to footer
- [x] Display partner logos with verification links
- [ ] Update Benevity/CanadaHelps profiles to 100%
- [x] Add sticky donate button to all pages
- [ ] Create "Transparency & Impact" dedicated page
- [ ] Add real-time/quarterly impact metrics dashboard

### Phase 2: Story Infrastructure (4-8 Weeks)

- [ ] Collect 3-5 client testimonials with consent
- [ ] Develop "Day in the Life" video content
- [ ] Create "Your $X Provides" impact calculator
- [ ] Professional photography of all properties
- [ ] Feature Jehnna Morin founder story prominently

### Phase 3: Conversion Optimization (8-12 Weeks)

- [x] Implement sticky donation button
- [ ] Create recurring giving program ("Housing Heroes")
- [ ] Add employer matching gift integration
- [ ] Simplify donation form to 5 fields maximum
- [ ] A/B test donation page headlines

---

## Key Performance Indicators

### Website Health Metrics

| Metric | Target | Industry Benchmark |
|--------|--------|-------------------|
| Bounce Rate | <50% | 60% (nonprofit avg) |
| Time on Site | >2 minutes | Average session |
| Pages per Session | >2.5 | Engagement indicator |
| Mobile Traffic | 50-60% | Ensure mobile parity |

### Conversion Metrics

| Metric | Target | Industry Benchmark |
|--------|--------|-------------------|
| Donation Page Conversion | ≥19% | 8-15% (average) |
| Email Signup Rate | 3-5% of visitors | Standard target |
| Recurring Donor % | 20% of donors | Monthly giving |
| Average Gift Size | Track monthly | +11% with seals |

### Trust & Authority Metrics

| Metric | Target |
|--------|--------|
| Third-Party Profile Completion | 100% on Benevity, CanadaHelps, Charity Intelligence |
| Media Mentions | Track CBC, Sudbury.com coverage |
| Organic Search Traffic | 44%+ (nonprofit benchmark) |

---

## Digital Asset Inventory

### Current Website Assets

| Asset | Status | Location |
|-------|--------|----------|
| Logo (PNG) | ✓ Available | logo.png |
| Homepage | ✓ Complete | index.html |
| Case Study: Reside | ✓ Complete | case-study-raising-roof.html |
| Case Study: Bloor | ✓ Complete | case-study-bloor.html |
| Case Study: Ste Anne | ✓ Complete | case-study-ste-anne.html |

### Existing External Assets

| Asset | Platform | URL |
|-------|----------|-----|
| CanadaHelps Profile | CanadaHelps | canadahelps.org/en/charities/sudburys-second-chance-transitional-centre/ |
| CRA Registration | CRA | apps.cra-arc.gc.ca |
| Raising the Roof Page | Raising the Roof | raisingtheroof.org/sudbury |

### Media Coverage (Verified Sources for Content)

| Date | Outlet | Article Topic | Journalist |
|------|--------|---------------|------------|
| Aug 2021 | CBC News | New grassroots group launch | Ezra Belotte-Cousineau |
| Oct 2021 | CBC News | Helping unhoused people | Aya Dufour |
| Apr 2023 | Sudbury.com | 1517 Kingslea Ct. grand opening | Jenny Lamothe |
| Jul 2023 | Sudbury.com | Grassroots organizations profile | Jenny Lamothe |
| May 2024 | CBC News | City funding for extended hours | CBC Staff |
| Nov 2024 | CBC News | National charity expansion | Erik White |

### Key Personnel for Photo/Content Permissions

| Name | Role | Contact Purpose |
|------|------|-----------------|
| Jehnna Morin | Founder/ED | Original photos, testimonials |
| Leslie Bellingham | Raising the Roof | Partnership content |
| Jenny Lamothe | Sudbury.com | Media photo licensing |
| Erik White | CBC | Media photo licensing |

---

## Technical Notes

### CSS Variables Used

```css
:root {
    --navy: #1e3a5f;
    --navy-dark: #152a45;
    --green: #7cb342;
    --green-dark: #689f38;
    --cream: #faf9f7;
    --text-dark: #1a1a1a;
    --text-muted: #5a6a7a;
}
```

### External Dependencies

- Google Fonts: Outfit, Source Sans 3
- Stripe.js (for donations)
- No other external JS libraries

### Browser Support

- Modern browsers (Chrome, Firefox, Safari, Edge)
- Mobile-responsive breakpoints at 968px and 640px
- CSS animations with appropriate fallbacks

### Accessibility Considerations

- All interactive elements have aria-labels
- External links have `rel="noopener"` for security
- Color contrast meets WCAG AA standards
- Sticky button includes aria-label="Donate Now"

---

## Appendix: Verified Quotes

### Mayor Paul Lefebvre

> "These renovations are a great model and I would like to see it expand in the city."

*Source: CBC News, November 2024*

### Leslie Bellingham (Raising the Roof)

> "It's a hub for northern Ontario and we see many people coming to the Sudbury area, or even from within Sudbury, who are in need of housing."

*Source: CBC News, multiple articles*

### Jehnna Morin (Founder)

> "Once they come out of those acute-care scenarios, just to put them under a roof is not sustainable — they will not sustain their homes and they will likely fall back into the system. And that's where the cycles were happening. So, in order to break those cycles, it's a matter of really teaching those life skills and getting their basic needs met."

*Source: CBC News, 2021*

> "Because honestly, even if it's a meal, or having fresh clothes on their backs, it just gives them a little bit more sense of belonging. And that is really the key to SCTC is providing that sense of belonging."

*Source: CBC News, 2021*

---

## Version History

| Date | Version | Changes |
|------|---------|---------|
| Jan 3, 2026 | 1.0 | Initial website development |
| Jan 3, 2026 | 1.1 | Fact-check corrections completed |
| Jan 3, 2026 | 1.2 | Nonprofit strategy research |
| Jan 13, 2026 | 1.3 | Quick wins implementation |
| Jan 13, 2026 | 1.4 | GitHub repository setup |

---

*This documentation is maintained alongside the codebase and should be updated with any significant changes to the website or strategy.*
