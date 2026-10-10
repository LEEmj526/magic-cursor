# Privacy

Magic Cursor processes cursor motion and mouse-button events briefly in memory for visual effects. It does not send cursor paths, screen contents, keyboard input or app activity history. Settings and presets stay on your Mac. Trial and license records are stored in device-local macOS Keychain entries; deleting the app or ordinary preferences does not reset a retained trial record.

## License verification in 1.2.0

Activation, revalidation and deactivation use HTTPS POST to `magiccursor-licensing.cbnu-math-booking.workers.dev`, hosted on Cloudflare. Requests contain your Gumroad license key, an app-scoped hash identifying this Mac and, when applicable, its random activation ID. The hash is derived from the platform UUID so ordinary app reinstallations keep the same device identity; the raw hardware UUID and computer hostname are not sent.

The server forwards the key and public product ID to `api.gumroad.com` to verify the purchase. It does not retain the raw key or customer/payment details returned by Gumroad. Its D1 database stores a secret-keyed license hash, the device hash, activation ID, lease expiry and release status to enforce one registered Mac per license. Error logs contain only the failed stage and error type, not request bodies or license keys. Cloudflare and Gumroad process ordinary network metadata under their own policies.

Pro activation leases last five minutes and are normally renewed every two minutes while the app runs. An outage beyond that window temporarily returns the app to Free without deleting your purchase key. Deactivation releases the registered Mac; transfer to a different Mac waits for the previous lease to expire, up to five minutes. Production rejects seller-test purchases. The local developer test app uses a separate Keychain service and direct Gumroad verification; it is not distributed publicly.

Version 1.1.0 and earlier use direct Gumroad verification and do not have this server device limit. There is no automatic update feed in the current release. Checkout opens Gumroad in your browser; no payment information is entered into Magic Cursor.

Preview and smoke modes use isolated memory storage and fixture responses. Login launch uses macOS ServiceManagement. No analytics SDK is included. Future configured Sparkle update checks may contact the update feed/archive host; system profiling is disabled.
