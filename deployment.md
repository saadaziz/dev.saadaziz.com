Here’s the **updated `DEPLOYMENT.md`** with branch deletion instructions added and formatted for clarity:

---

# Deployment Guide: dev → prod

## Overview
This guide explains:
1. How to promote code from `dev.saadaziz.com` (development) to `saadaziz.com` (production) safely.
2. How to create feature branches, develop, and merge using GitHub Flow.

---

# How to create feature branches, develop, and merge using GitHub Flow

## 1. Branch-to-PR Workflow

### Purpose
Guide for developing new features and merging into production using GitHub Flow.

---

### 1. Create a Feature Branch
git checkout main
git pull origin main
git checkout -b feature/<short-description>

### 2. Develop & Commit

Don't forget to update:     <input type="hidden" id="build-version" value="v0.1.1 – July 26, 2025, 8:45 PM PT">

git add .
git commit -m "Feature: <describe work>"

Push branch to remote:

git push --set-upstream origin feature/<short-description>

### 3. Test in Development Environment

* Deploys automatically to `dev.saadaziz.com`
* Verify UI changes, version footer, and all links

### 4. Open a Pull Request (PR)

* Compare `feature/*` → `main`
* PR should include:

  * Description of changes
  * Testing performed
  * Risks or dependencies
  * Screenshots if UI changes

### 5. Review & Approval

* Address review feedback
* Ensure `CHANGELOG.md` is updated before merge

### 6. Merge to Main

* Merge PR after approval

### 7. Delete Feature Branches (Cleanup)

**Local branch:**

git branch -d feature/<short-description>

**Remote branch:**

git push origin --delete feature/<short-description>

---

# How to promote code from `dev.saadaziz.com` (development) to `saadaziz.com` (production) safely

## Steps

### 1. Verify Dev Branch

* Confirm latest code is live and tested on `dev.saadaziz.com`
* Run browser QA checklist (resume, demo pages, version footer)

### 2. Create Pull Request

* Merge `feature/*` → `main`
* Ensure `CHANGELOG.md` and this file (`DEPLOYMENT.md`) are updated

### 3. Update GitHub Pages Settings

* Confirm `main` branch is configured for production domain
* Verify CNAME: `saadaziz.com`

### 4. Test Production

* Open `saadaziz.com` in browser
* Hard refresh (`Ctrl+Shift+R`) to validate cache bust
* Confirm version footer displays correct timestamp (if applicable)

---

## Notes

* Dev uses `dev.saadaziz.com`
* Prod uses `saadaziz.com`
* Both share the same repo but separate deployment settings


