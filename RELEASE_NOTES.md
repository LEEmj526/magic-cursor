# Magic Cursor 1.2.0

## One Mac per Pro license

- Added server-side device registration using Cloudflare Workers and D1.
- A license can register one Mac. Reinstalling on that same Mac reuses its registration.
- A second Mac is rejected until you deactivate on the old Mac and its previous lease expires (up to five minutes).
- Pro renews a five-minute activation lease every two minutes. Periodic internet access is required; a longer outage temporarily returns the app to Free while retaining the license key.
- Gumroad still handles checkout. Pro is $1.49 USD one-time; Free and the manually started 3-day trial remain available.
- Older 1.1.0/beta clients cannot be retroactively subject to the new server registration limit. Install 1.2.0 to use this activation flow.

## Validation and limits

48 Swift unit tests, 12 server tests using SQLite and 59 actual AppKit fixture checks passed. The deployed production server responds and rejects an actual seller-test key after live Gumroad verification.

The Universal DMG targets macOS 13+, is ad hoc signed and is not Apple notarized. Runtime testing covers macOS 15.8.1 on Apple silicon; Automatic update distribution is not configured.
