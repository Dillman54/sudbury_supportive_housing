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
- `assets/logo.svg` - Brand logo (inline in HTML, standalone for other uses)

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

## Brand Colors
- Primary: #3eb489 (mint)
- Dark: #2d8968 (mint-dark)  
- Darker: #236b52 (mint-darker, used for header CTA)
- Text: #2f4f4f (forest)

## Notes
- Footer section uses inline `!important` styles to override CSS specificity
- Logo is embedded as inline SVG in the hero section
- Page is mobile-responsive with breakpoints at 968px and 600px
