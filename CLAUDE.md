# Sudbury Supportive Housing - Claude Code Context

## Project Purpose
Recovery-focused supportive housing intake landing page for 30 Ste Anne Road, Sudbury.

## AWS Configuration
- **Profile:** Brettdillman
- **Region:** ca-central-1  
- **Bucket:** 30steanne

## Deployment
```bash
aws s3 cp index.html s3://30steanne/index.html --profile Brettdillman
```

## Key Files
- `index.html` - Main intake landing page (deploy to S3 root)
- `assets/brand/` - Brand identity package (logos in EPS, JPG, PNG formats)
- `assets/brand/PNG/SSH_LogoPRO.png` - Primary logo used in HTML

## Form Integration
All "Apply Now" CTAs link to Monday.com form:
```
https://forms.monday.com/forms/cf24c85d4581488165542fc332a17b0f?r=use1
```

## Common Tasks

### Update phone number
Search and replace in index.html, then redeploy.

### Update email addresses
Look for `intake@30steanne.ca` and `partners@30steanne.ca`.

### Change CTA button link
Search for `forms.monday.com` and update the form URL.

## Brand Colors (SSH Brand Identity)
- **Bright Green:** #84BD00 (PMS 376 C) - Primary accent, CTAs
- **Dark Blue:** #082861 (PMS 2787 C) - Primary color, text, headers
- Green Dark: #6a9700 (hover states)
- Blue Light: #0d3a8a (gradients, secondary)

## Typography
- Primary: Coolvetica (brand identity)
- Web fallbacks: Arial, Roboto, Open Sans

## Notes
- CTA section uses inline `!important` styles to override CSS specificity
- Logo is PNG image from brand assets (`assets/brand/PNG/SSH_LogoPRO.png`)
- Page is mobile-responsive with breakpoints at 968px and 600px
- Brand identity PDF located at `assets/brand/SSH_BrandIdentity_December2025.pdf`
