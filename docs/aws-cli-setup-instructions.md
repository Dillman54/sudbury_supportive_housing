# AWS CLI Setup Check

Run these checks in order and fix any issues before proceeding to the next step.

## Step 1: Check if AWS CLI is installed

```bash
aws --version
```

**If not found:** Install AWS CLI v2 using the appropriate method for the OS:
- macOS: `brew install awscli`
- Ubuntu/Debian: Download and install from https://docs.aws.amazon.com/cli/latest/userguide/getting-started-install.html
- Windows: Download MSI installer from same link

## Step 2: Verify version is 2.x

The output should show `aws-cli/2.x.x` — if it shows version 1.x, upgrade to v2.

## Step 3: Check current authentication state

```bash
aws sts get-caller-identity
```

**If this returns an error** about credentials or tokens, proceed to Step 4.
**If this returns account/user info**, CLI is already authenticated — skip to Step 5.

## Step 4: Authenticate using browser login

```bash
aws login
```

This opens a browser for authentication. Complete the login flow, then return to the terminal.

## Step 5: Confirm access

```bash
aws s3 ls
```

This should list available S3 buckets. If it does, setup is complete.

## Daily usage

Credentials expire after 12 hours. If you get auth errors, just run `aws login` again.
