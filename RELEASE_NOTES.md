# Magic Cursor 1.1.0

## New in Free

- Optional shake-to-locate: move the cursor briskly back and forth to reveal a locator ring. Off by default, with a cooldown to avoid repeated flashes.
- Pause effects for 1, 5 or 15 minutes from General or the menu bar. A countdown and Resume now button make it easy to take a break. Effects resume when the timer ends and the current app/session allows them.
- Existing global shortcuts and cursor locator remain free.

## New in Pro and the 3-day trial

- Focus Spotlight dims the active display outside a clear circle around the cursor.
- Adjust the spotlight radius and background dimming.
- New Presentation preset combines the spotlight and click ripples.

**Pro stays $1.49 USD, one-time.** Free keeps basic Ink/Halo effects and practical workflow controls; Pro adds presentation effects and advanced customization.

## Installation and validation

Download MagicCursor-v1.1.0.dmg, drag Magic Cursor into Applications, then launch it. No account is required for the GitHub installer. The same app supports Free, the optional 3-day trial and Pro.

This Universal build targets macOS 13+, is ad hoc signed and has not been notarized by Apple. First launch may require Privacy & Security → Open Anyway for this specific app. Runtime testing covers macOS 15.8.1 on Apple silicon with one display. No automatic update feed is configured.

45 unit tests, 9 release configuration checks and 53 AppKit smoke checks passed. Native UI checks covered the Free/Pro locks, pause countdown and manual resume. Physical keyboard hotkeys, real shake gestures, other macOS versions, Intel runtime and multiple displays still need broader manual testing. Actual paid-purchase activation and refund testing remain unverified; seller test keys work only in the separate developer test app.
