# Deployment Guide: dev → prod

## Overview
This guide explains how to promote code from `dev.saadaziz.com` (development) to `saadaziz.com` (production) safely.

---

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
