# Changelog

## 1.0.0 — 2026-10-10

- Removed development notes and unnecessary explanatory text from the app.
- Raised cursor effects above application windows, including System Settings, while keeping click-through input.
- Added persistent Free, Pro and Pro trial labels in settings and the menu bar.
- Dimmed and locked unavailable Pro effects, appearance controls and presets.
- Improved Gumroad key paste normalization, specific seller-test-key errors and retry behavior.
- Added an installed-application picker with names, icons, search and browsing for effect exclusions.
- Added a direct $2.99 Pro checkout button. The same app upgrades after license verification; no separate Pro installation is needed.
- Published the free DMG on GitHub. The optional Gumroad support page remains available.



## 0.8.1 Beta — 2026-10-10

- Changed the user-started Pro trial to 3 days (72 hours), preserving the original stored start time and one-trial limit.
- Updated the English/Korean license UI, detailed product guide and beta installation instructions.
- Added Gumroad purchase verification, refund/chargeback rejection, provider-specific receipts and local license removal.
- Prepared Magic Cursor Pro as a $2.99 USD one-time product; checkout is live; actual paid-purchase validation remains pending.
- Added a persisted-trial regression check and AppKit checks for the 72-hour boundary.

## 0.8.0 Beta — 2026-10-10

- Added Free/Pro entitlement enforcement while preserving saved settings and presets.
- Added an explicit 14-day trial with device-local Keychain persistence, expiry and clock rollback checks.
- Added Lemon Squeezy activation, validation and deactivation with product/device matching, offline grace and private license storage.
- Added pinned Sparkle 2.9.4 integration, manual and optional automatic update controls, signed feed/archive configuration and nested framework signing.
- Added validated public release configuration, English source/distribution documentation, CI preparation and release support templates.
- Extended deterministic unit and GUI smoke checks to cover licensing transitions and storage/network failures.

This is a local development beta. Live merchant setup, production signing/notarization, real updates and broader runtime QA remain pending.

## 0.7.0 Developer Preview — 2026-10-10

Initial native menu bar app with all five effects, presets, live settings, schema recovery, per-display overlays, power/accessibility/session handling, app exclusions, onboarding, English/Korean, login launch and Universal app/DMG build scripts.
