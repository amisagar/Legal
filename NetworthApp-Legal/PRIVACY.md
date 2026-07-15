# Vaulted — Privacy Policy

**Effective: {EFFECTIVE_DATE}**

## The short version

Vaulted stores your financial data on your device. We don't collect it, we don't see it, and we don't sell it. If you enable iCloud sync, your data goes directly from your device to your iCloud account under your Apple ID — we're not in the middle. There are no analytics, no tracking pixels, no third-party SDKs.

That's it. The rest of this policy is the legal detail.

## What Vaulted stores

Vaulted stores the following on your device only:

- Account names, categories, currencies, and balances you enter
- Historical balance snapshots you record
- Financial goals you set
- Your app preferences (currency, display name, notification schedule, app-lock setting)
- Notes you write on snapshots or accounts

None of this information leaves your device unless you enable iCloud sync (see below), export data manually via the Export screen, or share a screenshot yourself.

## iCloud sync

If you enable iCloud sync in Settings, your account data is stored in your private iCloud database using CloudKit. This is Apple's system for personal cloud storage tied to your Apple ID. Vaulted:

- Cannot read or access your iCloud data
- Cannot see other data in your iCloud account
- Uses only the CloudKit **private** database (never the public or shared one)
- Cannot sync your data to anyone else's device unless they sign in with your Apple ID

Apple's privacy policy governs how iCloud handles your data: <https://www.apple.com/legal/privacy/>

## What Vaulted does NOT do

- We do not use analytics services (no Firebase, no Mixpanel, no Amplitude, no Meta / Facebook SDK, no equivalents)
- We do not embed advertising SDKs
- We do not track your usage
- We do not integrate with bank-aggregation services like Plaid, MX, Yodlee, or similar
- We do not send push notifications from our servers (all notifications are scheduled locally on your device)
- We do not require an account signup — no email, no password, no phone number

## StoreKit and subscriptions

If Vaulted offers subscriptions, purchases are handled entirely by Apple through StoreKit. When you subscribe:

- Apple processes payment, not us
- Your Apple ID handles subscription entitlement
- We receive only an entitlement flag confirming your subscription status
- We do not receive your credit card number, address, or purchase history

Apple's App Store & Privacy policy governs this: <https://www.apple.com/legal/privacy/data/en/app-store/>

## Face ID / Touch ID / passcode

The optional App Lock feature uses your device's Face ID, Touch ID, or passcode. Authentication happens entirely on your device via Apple's LocalAuthentication framework. We never see your biometric data or your passcode — Apple's Secure Enclave handles it.

The App Lock preference itself is stored in the iOS Keychain on your device.

## Notifications

Reminder notifications are scheduled locally on your device using `UNUserNotificationCenter`. They do not travel through any server. If you disable notifications for Vaulted in iOS Settings, they simply stop firing.

## Data export

You can export all your data as JSON or CSV from Settings → Export Data. The exported file is written to a temporary location on your device and shared via the standard iOS share sheet. We do not receive a copy.

## Data deletion

Because we don't have your data, we can't delete it for you. To delete your data from Vaulted:

- Delete accounts one-by-one within the app (permanently removes them and their snapshots after a short undo window)
- Reset all preferences from Settings
- Delete the app entirely, which removes the local SwiftData store
- If you use iCloud sync, delete Vaulted data from your iCloud account in iOS Settings → your name → iCloud → Manage Account Storage → Vaulted

## Children

Vaulted is not directed at children under 13 and does not knowingly collect information about them. It does not knowingly collect information about anyone.

## Changes to this policy

If we update this policy, the new version will be published at the same URL as this one, with a new effective date. Material changes will also be noted in the app's release notes.

## Contact

Privacy questions? {SUPPORT_EMAIL}

---

*Published by {YOUR_NAME_OR_ENTITY}.*
