# Handoff Document: Sudbury's Supportive Housing Landing Page

## Current Status: Ready for Deployment

The landing page is complete and ready to deploy to your S3 bucket.

---

## Immediate Next Steps

### 1. Deploy to S3 (5 minutes)

**Option A: Via Claude Code**
Open Claude Code in this repo folder and say:
```
Deploy index.html to s3://30steanne using the Brettdillman profile
```

**Option B: Manual CLI**
```bash
cd sudbury_supportive_housing
aws s3 cp index.html s3://30steanne/index.html --profile Brettdillman
```

**Option C: AWS Console**
1. Go to S3 → 30steanne bucket
2. Upload `index.html`
3. Ensure public read access is enabled

### 2. Verify Deployment
Visit your S3 website URL (format: `http://30steanne.s3-website.ca-central-1.amazonaws.com`) and confirm:
- [ ] Page loads correctly
- [ ] Logo displays in hero section
- [ ] "Apply Now" buttons link to Monday.com form
- [ ] Footer section has dark background with readable white text
- [ ] Mobile view works (test on phone or browser dev tools)

### 3. Test the Form Flow
1. Click any "Apply Now" button
2. Confirm Monday.com form opens
3. Submit a test entry
4. Verify it appears in your Monday.com board
5. Confirm any automations/notifications trigger correctly

---

## Short-Term Tasks (This Week)

### Update Contact Information
The page currently shows placeholder data:
- **Phone:** 705-555-0199 (update to real number)
- **Email:** intake@30steanne.ca (ensure mailbox exists)
- **Partner Email:** partners@30steanne.ca (ensure mailbox exists)

To update, edit `index.html` and search for these values, or ask Claude Code:
```
Update the phone number in index.html to 705-XXX-XXXX and redeploy to S3
```

### CloudFront + Custom Domain (Optional but Recommended)
For HTTPS and a professional URL:
1. Register domain (e.g., `30steanne.ca`) if not already owned
2. Create CloudFront distribution pointing to S3 bucket
3. Request SSL certificate via AWS Certificate Manager
4. Configure Route53 or external DNS

Claude Code can walk through this setup when ready.

---

## Medium-Term Improvements

### Analytics
Add privacy-respecting analytics to understand traffic:
- **Plausible:** `<script defer data-domain="yourdomain.ca" src="https://plausible.io/js/script.js"></script>`
- **Simple Analytics:** Similar lightweight option

### SEO Optimization
- Verify meta description is accurate
- Submit to Google Search Console
- Consider adding structured data (LocalBusiness schema)

### Partner Referral Form
If partner referrals need a dedicated intake:
1. Create separate Monday.com form for partners
2. Build `partners.html` landing page
3. Link from main page's Partner Referrals section

---

## Long-Term Considerations

### Template System
If you add more properties or pages:
1. Set up Eleventy (11ty) static site generator
2. Extract header, footer, nav into reusable components
3. Each page becomes a simple content file
4. Build process generates full HTML

### Multiple Properties
If expanding beyond 30 Ste Anne:
```
sudbury_supportive_housing/
├── src/
│   ├── _includes/
│   │   ├── header.njk
│   │   ├── footer.njk
│   │   └── nav.njk
│   ├── 30-ste-anne/
│   │   └── index.md
│   ├── other-property/
│   │   └── index.md
│   └── _data/
│       └── properties.json
├── dist/           # Generated HTML (deploy this)
└── eleventy.config.js
```

---

## Key Contacts & Resources

| Resource | Location |
|----------|----------|
| Monday.com Form | https://forms.monday.com/forms/cf24c85d4581488165542fc332a17b0f?r=use1 |
| AWS Console | https://console.aws.amazon.com |
| S3 Bucket | s3://30steanne |
| AWS CLI Profile | Brettdillman |

---

## Troubleshooting

### Page not updating after S3 upload
- Browser cache: Hard refresh (Ctrl+Shift+R / Cmd+Shift+R)
- CloudFront cache: Create invalidation for `/*`
- S3 permissions: Verify bucket policy allows public read

### AWS CLI authentication errors
```bash
aws sts get-caller-identity --profile Brettdillman
```
If this fails, re-run `aws configure --profile Brettdillman` with your access keys.

### Form not receiving submissions
1. Check Monday.com form is published and active
2. Verify URL matches exactly (including `?r=use1` parameter)
3. Test form directly at the URL

---

## Handoff Complete

This project is ready for:
- [x] Deployment to production
- [x] Content updates via Claude Code
- [x] Future expansion with documented architecture

**Questions?** Start a new Claude conversation and reference this repo for context.

---

*Handoff prepared January 13, 2026*
