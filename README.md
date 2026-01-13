# Sudbury's Supportive Housing

Recovery-focused supportive housing intake landing page for 30 Ste Anne Road, Sudbury, ON.

## Quick Deploy

```bash
aws s3 cp index.html s3://30steanne/index.html --profile Brettdillman
```

## Project Structure

```
├── index.html          # Main landing page
├── assets/
│   └── logo.svg        # Brand logo (SVG)
└── docs/
    ├── CONTEXT.md      # Full project context & technical decisions
    ├── HANDOFF.md      # Deployment guide & next steps
    └── aws-cli-setup-instructions.md
```

## Form Integration

All "Apply Now" CTAs link to:  
`https://forms.monday.com/forms/cf24c85d4581488165542fc332a17b0f?r=use1`

Submissions flow into Monday.com for workflow automation.

## Tech Stack

- **Hosting:** AWS S3 static website
- **Forms:** Monday.com
- **Styling:** Vanilla CSS (no frameworks)
- **Font:** Inter (Google Fonts)

## Documentation

- [Project Context & Research](docs/CONTEXT.md) - Full background, architecture decisions, design rationale
- [Handoff & Next Steps](docs/HANDOFF.md) - Deployment checklist, future improvements

---

*14730437 Canada Inc.*
