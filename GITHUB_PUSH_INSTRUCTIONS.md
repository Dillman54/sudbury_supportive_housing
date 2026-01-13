# Push to GitHub Instructions

## For Claude Code

Unzip the `sudbury_supportive_housing.zip` file to your projects folder, then give Claude Code these instructions:

```
Initialize a git repo in the sudbury_supportive_housing folder and push it to GitHub. 
Create the repo if it doesn't exist. Use the repo name "sudbury_supportive_housing".
```

## Manual Steps (if needed)

### 1. Extract the zip
```bash
cd ~/Projects  # or your preferred location
unzip sudbury_supportive_housing.zip
cd sudbury_supportive_housing
```

### 2. Initialize Git
```bash
git init
git add .
git commit -m "Initial commit: Supportive housing intake landing page"
```

### 3. Create GitHub repo and push

**Option A: GitHub CLI (if installed)**
```bash
gh repo create sudbury_supportive_housing --public --source=. --push
```

**Option B: Manual**
1. Go to github.com → New repository
2. Name: `sudbury_supportive_housing`
3. Create (don't initialize with README)
4. Copy the remote URL, then:
```bash
git remote add origin https://github.com/YOUR_USERNAME/sudbury_supportive_housing.git
git branch -M main
git push -u origin main
```

## Repository Contents

```
sudbury_supportive_housing/
├── index.html              # Landing page (deploy to S3)
├── README.md               # Project overview
├── CLAUDE.md               # Context for Claude Code
├── assets/
│   └── logo.svg            # Brand logo
└── docs/
    ├── CONTEXT.md          # Full project research & decisions
    ├── HANDOFF.md          # Deployment & next steps
    └── aws-cli-setup-instructions.md
```
