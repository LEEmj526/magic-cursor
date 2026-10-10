# Installation and troubleshooting

Download [Magic Cursor 1.1.0 from GitHub](https://github.com/LEEmj526/magic-cursor/releases/latest). No account or payment is required for the DMG. The release is ad hoc signed and not Apple notarized. On first launch, macOS may require System Settings → Privacy & Security → Open Anyway for this specific app.

For a released build, open the DMG and drag Magic Cursor to Applications. Launch it and complete onboarding. It lives in the menu bar, with no Dock icon. Enable effects from the menu bar panel; open Settings with Command-comma and quit with Command-Q.

The app keeps the macOS cursor and uses transparent overlays. Protected system UI, some fullscreen applications and games may limit overlay visibility. If global click effects are unavailable, movement effects remain usable. Launch-at-login approval is handled in macOS System Settings.

If macOS rejects a release, verify that it is the current official download and include the exact message in a support issue. Do not disable Gatekeeper globally. Include macOS version, Mac model/architecture, display setup, preset and reproduction steps. Remove personal data, license keys and payment details from screenshots and logs.

To uninstall, disable launch at login, quit Magic Cursor and remove it from Applications. Effect settings reside under `~/Library/Application Support/MagicCursor/`. Trial/license records are stored separately in Keychain. Remove a Gumroad license locally with Settings → License → Remove license from this Mac. This does not cancel the purchase or revoke the key on Gumroad.

Pause effects in specific apps with Settings → General → Add application… and select an installed app by name. To upgrade, choose Settings → License → Upgrade to Pro, complete Gumroad checkout, paste the key from the receipt and select Activate license. Seller test keys require the separate local developer test app.
