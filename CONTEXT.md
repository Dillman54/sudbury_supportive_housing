# Sudbury's Supportive Housing - Project Context & Research

## Project Overview

**Property:** 30 Ste Anne Road, Sudbury, ON P3C 5E1  
**Purpose:** Recovery-focused sober living / supportive housing intake landing page  
**Owner:** Brett Dillman (14730437 Canada Inc.)  
**Created:** January 2026

---

## Business Context

### Target Audience
- Individuals with 30+ days of documented sobriety seeking stable housing
- Adults 18+ with ties to the Greater Sudbury community
- Referral partners: healthcare providers, treatment centers, social service agencies

### Program Details (from landing page)
- **Capacity:** 135 private rooms
- **Cost:** $900/month (compatible with OW/ODSP)
- **Typical Stay:** 12-18 months
- **Support:** 24/7 wraparound services, 1:25 staff ratio

### Intake Flow
1. Visitor lands on page → reviews eligibility requirements
2. Clicks "Apply Now" CTA → redirected to Monday.com form
3. Monday.com captures intake data → triggers workflow automation
4. Staff receives notification → phone screening → intake interview → acceptance

---

## Technical Architecture

### Current Hosting Setup
- **Platform:** AWS S3 static website hosting
- **Bucket:** `30steanne` (existing)
- **Authentication:** AWS CLI v2 with `Brettdillman` IAM profile
- **Credentials:** Static access keys stored in `~/.aws/credentials`

### Form Integration
- **Form Platform:** Monday.com Forms
- **Form URL:** `https://forms.monday.com/forms/cf24c85d4581488165542fc332a17b0f?r=use1`
- **Workflow:** Form submissions create items in Monday.com board, triggering task automation and notifications

### Deployment Process
```bash
# Authenticate (credentials already configured)
aws sts get-caller-identity --profile Brettdillman

# Deploy to S3
aws s3 cp index.html s3://30steanne/index.html --profile Brettdillman

# If using CloudFront, invalidate cache
aws cloudfront create-invalidation --distribution-id <ID> --paths "/*"
```

---

## Design Decisions

### Color Palette
| Variable | Hex | Usage |
|----------|-----|-------|
| `--mint` | #3eb489 | Primary brand color |
| `--mint-dark` | #2d8968 | CTA buttons, emphasis |
| `--mint-darker` | #236b52 | Header nav CTA |
| `--forest` | #2f4f4f | Body text, headings |
| `--slate` | #4a5d5d | Secondary text |

### Typography
- **Font:** Inter (Google Fonts)
- **Weights:** 300 (light), 400 (regular), 700 (bold), 800-900 (headings)

### Key UX Fixes Applied
1. **CTA Visibility:** Changed from light mint to dark green (`--mint-darker`) for header Apply Now button
2. **Footer Section Contrast:** Changed from transparent gradient to solid `#1e3a3a` background with inline `!important` styles to override CSS specificity issues
3. **Mobile Responsiveness:** Nav stacks vertically, grids collapse to single column, padding adjusts
4. **Form Links:** All CTAs now link directly to Monday.com form (previously were anchor links)

### Logo
- Custom SVG recreation of Sudbury's Supportive Housing brand
- Elements: Navy house silhouette, green leaf accent, three figures with connected arms
- Embedded inline in hero section on white card background

---

## Infrastructure Insights

### Web Hosting Philosophy
The "pretty pages stitched together with links" approach is architecturally sound for this use case:
- **JAMstack pattern:** Static HTML + external form handling (Monday.com)
- **Benefits:** Fast, secure (no database), essentially free at low traffic (<100 visits/month)
- **Trade-off:** Manual updates required for each page (no CMS)

### AWS CLI Evolution (2024-2025)
AWS now recommends `aws login` for browser-based authentication instead of static access keys:
```bash
aws login  # Opens browser, gets temporary credentials valid 12 hours
```
However, this requires additional setup and may not work in all environments. The static key approach (`aws configure`) remains functional.

### Future Scaling Options
If page count grows beyond 5-10 and updates become tedious:
1. **Static Site Generator:** Eleventy (11ty) for templated components
2. **Managed Hosting:** Framer or Webflow for visual editing + hosting
3. **Hybrid:** Keep S3 hosting but use build system for shared headers/footers

---

## Claude Code Integration

### Workflow Established
Claude Code can now manage S3-hosted pages conversationally:
```
"Pull index.html from s3://30steanne, update the phone number to 705-XXX-XXXX, and push it back"
```

### Recommended CLAUDE.md for Project
```markdown
# Sudbury Supportive Housing - Claude Code Context

## AWS Configuration
- Profile: Brettdillman
- Region: ca-central-1
- Bucket: 30steanne

## Deployment Commands
aws s3 cp index.html s3://30steanne/index.html --profile Brettdillman

## Key Files
- index.html: Main intake landing page
- assets/logo.svg: Brand logo

## Form Integration
All "Apply Now" buttons link to: https://forms.monday.com/forms/cf24c85d4581488165542fc332a17b0f?r=use1
```

---

## Open Questions / Future Considerations

1. **Custom Domain:** Is there a domain like `30steanne.ca` or `sudburysupportivehousing.ca`? Would need CloudFront + ACM certificate for HTTPS.

2. **Analytics:** No tracking currently implemented. Consider adding Plausible or Simple Analytics for privacy-respecting visitor insights.

3. **Partner Portal:** Landing page mentions `partners@30steanne.ca` for referrals—is there a separate partner intake form needed?

4. **Multiple Properties:** If Brett expands supportive housing to additional properties, a template system would reduce maintenance overhead.

5. **Email Addresses:** Page shows `intake@30steanne.ca` and `partners@30steanne.ca`—ensure these are configured and receiving.

---

## Files in This Repository

```
sudbury_supportive_housing/
├── index.html                    # Main landing page (ready for S3 deployment)
├── assets/
│   └── logo.svg                  # Standalone logo file
├── docs/
│   ├── aws-cli-setup-instructions.md
│   ├── CONTEXT.md                # This file
│   └── HANDOFF.md                # Next steps and deployment guide
└── README.md                     # Quick start guide
```

---

*Document generated from Claude conversation on January 13, 2026*
