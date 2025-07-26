# Changelog – dev.saadaziz.com

All notable changes to this project will be documented in this file.  
This project adheres to [Keep a Changelog](https://keepachangelog.com/en/1.0.0/) format and follows [Semantic Versioning](https://semver.org/).

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

### Changed
- Migrated development files from production repo to new dev repo for cleaner branching.

### Notes
- HTTPS certificate issuance pending; expected within 30 minutes of DNS propagation.
- DNS verified using [dnschecker.org](https://dnschecker.org).

---

