# Changelog

All notable changes to this project will be documented in this file.

## [0.2.0] - 2026-01-06
### Added
- Created `CHANGELOG.md`.

### Changed
- Bumped userscript version to **0.2.0** in `Chase-One-Click-Offer-Activator.user.js`.
- Updated route detection to handle hashes with query parameters (use `startsWith` and href fallback).
- Improved offer activation logic to dispatch a `MouseEvent` on the nearest interactive ancestor (e.g., `[role="button"]` or `[data-cy="commerce-tile"]`) instead of calling `.click()` on SVGs, fixing `btn.click is not a function` errors.
- Added console error logging and an activation success count.

### Notes
- If you want more robust SPA navigation handling (e.g., pushState-based), we can add a `MutationObserver` or patch history methods in a follow-up.


[Unreleased]: https://github.com/phuanh004/Chase-One-Click-Offer-Activator/compare/v0.2.0...HEAD
