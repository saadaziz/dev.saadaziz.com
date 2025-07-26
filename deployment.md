# Deployment Guide: dev → prod

## Overview
This guide explains:
1. How to promote code from `dev.saadaziz.com` (development) to `saadaziz.com` (production) safely.
2. How to create feature branches, develop, and merge using GitHub Flow

---

# How to create feature branches, develop, and merge using GitHub Flow
## Steps

## 1. Branch-to-PR Workflow

### Purpose
Guide for developing new features and merging into production using GitHub Flow.

---

### 1. Create a Feature Branch
git checkout main
git pull origin main
git checkout -b feature/short-description

### 2. Develop & Commit
git add .
git commit -m "Feature: <describe work>"

Push branch to remote:
git push --set-upstream origin feature/<short-description>

### 3. Test in Development Environment

### 4. Open a Pull Request (PR)
- Compare feature/* → main
- PR should include:
  - Description of changes
  - Testing performed
  - Risks or dependencies
  - Screenshots if UI changes

### 5. Review & Approval
- Address code review feedback.
- Ensure CHANGELOG.md is updated before merge.

### 6. Merge to Main
- Merge PR after approval.

Delete feature branch (local and remote):

git branch -d feature/<short-description>
git push origin --delete feature/<short-description>

---

# How to promote code from `dev.saadaziz.com` (development) to `saadaziz.com` (production) safely.
## Steps

### 1. Verify Dev Branch
- Confirm feature branch is tested on `dev.saadaziz.com`
- Run browser QA checklist (resume, demo pages, version footer)

### 2. Create Pull Request
- Merge `feature/*` → `main`
- Ensure CHANGELOG.md and WORKFLOW.md are updated

### 3. Update GitHub Pages Settings
- Confirm `main` branch is configured for production domain
- Verify CNAME: `saadaziz.com`

### 4. Test Production
- Open `saadaziz.com` in browser
- Validate cache bust (Ctrl+Shift+R) and confirm version timestamp

---

## Notes
- Dev uses `dev.saadaziz.com`
- Prod uses `saadaziz.com`
- Both share the same repo but separate branches
