# Changelog – dev.saadaziz.com

All notable changes to this project will be documented in this file.  
This project adheres to [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format and follows [Semantic Versioning](https://semver.org/).

---

<!-- Template for future releases -->
## [x.y.z] – YYYY-MM-DD
### Added
-
### Changed
-
### Fixed
-

---

## [Unreleased]
- Planned: Integration with CareerGPT backend (`aurorahours.com/careergpt`) for contextual responses.
- Planned: User authentication (Google OAuth + MySQL) for coaching signup.
- Planned: Secure API key exchange between `saadaziz.com` and `aurorahours.com` backend.

---

## [0.1.0] – 2025-07-26
### Added
- Created dedicated GitHub repository `dev.saadaziz.com`.
- Configured GitHub Pages for separate dev environment:
  - Branch: `main`
  - Custom Domain: `dev.saadaziz.com`
- Added `CNAME` file with `dev.saadaziz.com`.
- Set up GoDaddy DNS CNAME record (`dev` → `saadaziz.github.io`).
- Verified separation between production (`saadaziz.com`) and dev (`dev.saadaziz.com`) environments.
- Deployment instructions for promoting from dev.saadaziz.com to saadaziz.com.

### Changed
- Migrated development files from production repo to new dev repo for cleaner branching.
- Clarified workflow steps for branch promotion and QA signoff.

### Notes
- HTTPS certificate issuance pending; expected within 30 minutes of DNS propagation.
- DNS verified using [dnschecker.org](https://dnschecker.org).

---

## [0.2.0] – 2025-07-27
### Changed
- UI cleanup across `resume.html` and `index.html`:
  - Synced skills sections between pages for consistency.
  - Added version footer logic (visible only on `dev.saadaziz.com`).
  - Disabled "View Live" button for unavailable demos (grayed-out non-clickable state).
- Updated documentation:
  - Added `DEPLOYMENT.md` for branch → PR workflow and dev → prod promotion.

### Notes
- Refer to `DEPLOYMENT.md` for full deployment instructions.
