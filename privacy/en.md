---
title: Privacy Policy
permalink: /privacy/en/
lang: en
alt_url: /privacy/ja/
alt_label: 日本語
---

# Veiler Privacy Policy

**Effective: 15 July 2026**
**Last revised: 21 August 2026**

This Privacy Policy (the "Policy") describes how Hiroki Kataoka ("we", "us") handles user information in the iOS application "Veiler" (the "App"). Please read it before using the App.

The App keeps photos, videos and documents on your device and locks them behind a passcode or biometrics (Face ID and similar). It requires no account, and we operate no server or database of our own for it. What you store stays on your device. For vaults with iCloud sync switched on under the paid "Veiler Pro" plan, an encrypted copy is also kept in your own iCloud (see section 5). On the free plan, the App displays advertising (see section 2.3).

> This Policy is a translation provided for convenience. The Japanese version is the original and governs in the event of any discrepancy: [プライバシーポリシー](../ja/).

## 1. Who we are

- Provider: Hiroki Kataoka (independent developer)
- Contact: kyataoka.deve@gmail.com
- Application: Veiler (iOS)

We are an independent developer and provide the App as a personal development activity.

## 2. Information we collect

### 2.1 What you store — never sent to us

The App stores the photos, videos and documents you keep in it, together with their titles, albums and other organising information, on your device. We operate no server for the App, and none of this is ever sent to us.

Only for vaults where you have switched iCloud sync on under the paid "Veiler Pro" plan, an encrypted copy of their contents (photos, videos and documents, and their titles, albums and other organising information) is stored in the App's own area of the iCloud account tied to your Apple ID. Sync is chosen by you, per vault, and is off by default. See section 5.

We include no analytics SDK and no crash-reporting SDK in the App, and we neither collect nor hold any record of what you view or what you do inside it. The App does use an SDK for managing purchases (2.2) and an SDK for displaying advertising on the free plan (2.3); what those providers collect under their own terms is described in each section.

### 2.2 Exception — subscription purchases

Only when you buy or restore the paid "Veiler Pro" plan, the App uses the SDK of a third-party service, RevenueCat (RevenueCat, Inc.), to manage the purchase. The following is then sent to and held on RevenueCat's servers.

- Purchase history: receipts from Apple's In-App Purchase, and the state of purchases, cancellations and trials
- An anonymous app user ID the App uses to associate a purchase state (it is not linked to your name, email address or anything else that identifies you directly)
- Device information incidental to processing the purchase (device type, OS version, approximate region)

This is used to provide the paid features, to restore purchases, and to prevent fraud. We do not use it for advertising or profiling. RevenueCat's handling of information is governed by its own privacy policy (<https://www.revenuecat.com/privacy/>).

Payment itself is processed by Apple (the App Store). Neither we nor RevenueCat receive your credit card number or any other payment details.

### 2.3 Information related to advertising

The free plan displays advertising in the App. Advertising is delivered using the SDK of Google's advertising service "Google AdMob" (Google LLC), and the following is sent to Google to deliver ads, measure impressions and prevent fraud.

- Device identifiers such as the advertising identifier (IDFA). The IDFA is used only if you allow it at the iOS tracking permission prompt
- Approximate location inferred from your IP address (at the level of country or region; we do not collect precise GPS location)
- Device information (device type, OS version and similar), usage such as ad impressions and taps, and diagnostic information about the ad SDK's operation

Google handles this under its own privacy policy, and may use it for delivering and measuring advertising and for personalised advertising by Google and its advertising partners. See Google's privacy policy (<https://policies.google.com/privacy>) and "How Google uses information from sites or apps that use our services" (<https://policies.google.com/technologies/partner-sites>).

**The advertising SDK does not read the photos, videos or documents you keep in the App, nor their titles or album names.** What we receive about advertising is aggregate figures only — impressions, revenue and the like — never anything that identifies an individual user to us.

Your choices about advertising are as follows.

- In the European Economic Area, the United Kingdom and other covered regions, we present a consent screen through Google's User Messaging Platform (UMP). If you do not consent, non-personalised advertising is delivered.
- If you choose "Ask App Not to Track" at the iOS prompt, the IDFA is not used. You can change this at any time under iOS Settings > Privacy & Security > Tracking.
- On the paid "Veiler Pro" plan, no advertising is displayed, the ad SDK is not initialised, and no information is sent for the delivery of advertising.

### 2.4 Usage records (measurement for improving the App)

The App records which of its features are used (for example, that an import completed, or that the settings screen was opened), using a fixed set of event names only. This is sent using Google Analytics for Firebase and Firebase Crashlytics (both Google LLC, USA). If the App fails to work correctly, the kind of failure and where in the program it occurred are recorded as well.

Nothing from inside a vault is ever sent — no file names, no album names, no counts. These records are not linked to anything that identifies you, nor to the advertising identifier (IDFA). You can stop this recording at any time from the App's settings ("Share usage data", under About).

### 2.5 Feedback submissions

When you write in through the App's feedback screen, what is sent is the kind you picked (bug, request or other), the text you wrote, plus the app version, iOS version and device model — nothing else. Because nothing identifies you, we cannot reply. Submissions are stored in Google Cloud Firestore (Google LLC, USA).

## 3. Why we use it

We use the purchase-related information described in 2.2 only for the following purposes.

- Providing the paid "Veiler Pro" plan and enabling or disabling paid features
- Restoring purchases when you change device or reinstall
- Resolving problems with billing and preventing fraudulent use
- Complying with the law and performing the Terms of Service

The advertising-related information described in 2.3 is used by Google to deliver, display and measure advertising and to prevent fraud, so that the free plan can be funded by advertising revenue. We do not use it to identify you, nor do we cross-reference it against any other information.

## 4. Disclosure and processors

We do not sell or rent the information we receive to third parties, and we do not disclose it to third parties except as required by law.

We engage the following providers to process information for the purposes of the paid plan and advertising. They handle it within the scope we specify.

- Apple Inc. (App Store / In-App Purchase): payment processing, and the provision, renewal and cancellation of subscriptions. Information handled: purchase and billing information (payment details are held by Apple and are not received by us).
- RevenueCat, Inc.: managing subscription state and restoring purchases. Information handled: the purchase history, anonymous user ID and device information described in 2.2.
- Google LLC (Google AdMob): delivering and measuring advertising on the free plan. Information handled: the device identifiers, approximate location, device information and advertising usage described in 2.3. Google handles this independently under its own privacy policy, for advertising by itself and by its advertising partners.
- Google LLC (Firebase: Google Analytics / Crashlytics / Cloud Firestore): aggregating the usage and failure records described in 2.4, and storing the feedback described in 2.5.

The servers of these providers may be located outside Japan, including in the United States. They handle information under their own privacy policies and applicable law.

## 5. Where data is kept, and for how long

- The photos, videos and documents you keep in the App, and their organising information, are stored on your device, in the App's own storage area. They are not stored on any server of ours.
- For vaults with iCloud sync switched on (Veiler Pro), an encrypted copy is stored in the App's own container within the iCloud account tied to your Apple ID. The destination is your own iCloud; we neither obtain nor view its contents. This copy is kept until you delete it.
- Data stored on the device is excluded from device backups, including iCloud Backup and backups to a computer. The contents of a vault are not duplicated into a backup of your device.
- Deleting (uninstalling) the App removes all of the App's data stored on the device. The encrypted copy of any vault that had iCloud sync switched on does, however, remain in your iCloud after uninstalling, so that it can be restored when you reinstall and sign in with the same Apple ID. Section 6 explains how to delete it.
- The purchase-related information in 2.2 is retained by Apple and RevenueCat for as long as is necessary to manage and restore purchases.
- The retention period for the advertising-related information in 2.3 is determined by Google.

On protection: the current version of the App does not encrypt files on the device with its own encryption. It stores them in a dedicated area, behind the App's passcode and biometric lock, and relies on the standard device protection iOS provides, such as protection by the device passcode. For stronger protection, set a passcode on the device itself.

Copies uploaded to iCloud, on the other hand, are always encrypted. This is a measure to avoid placing unencrypted files in the cloud; it is not a guarantee that the contents are concealed from anyone able to access your iCloud account.

## 6. Your rights and choices

- Viewing and taking your data out: what you have stored can be exported at any time through the App's export feature and the OS share sheet.
- Deleting data: items can be deleted individually in the App, and deleting the App from your device removes all of the App's data on that device.
- Deleting the copy in iCloud: the encrypted copy of a vault with iCloud sync switched on can be erased under iOS Settings > (your name) > iCloud > Manage Account Storage, by selecting Veiler and deleting its data. Uninstalling the App alone does not erase it. If anything is unclear, contact us at the address in section 1.
- Usage records: the records described in 2.4 can be switched off at any time in the App's settings ("Share usage data", under About).
- Advertising: you can limit the use of information for advertising by the means described in 2.3 — changing the iOS tracking setting, your choice at the consent screen in covered regions, or purchasing Veiler Pro.
- How the bin behaves: deleted items are held in the bin for a period that depends on your plan (up to 30 days on Veiler Pro) before being permanently deleted. On the free plan, deletion takes effect immediately. Data in the bin is also lost if you delete the App.
- Purchase information: you can review and manage your billing and purchase history through your Apple App Store account settings and, where needed, via the contact address in section 1.

## 7. Biometrics (Face ID and similar)

The App can use your device's biometrics (Face ID, Touch ID and similar) to unlock. Biometric matching is completed entirely within the device's OS; the App never obtains, stores or transmits the biometric information itself — no face and no fingerprint. The App receives only the result of whether authentication succeeded.

## 8. Use by minors

Minors should use the App with the consent of a parent or guardian. We do not collect identification documents, photographs or anything similar for the purpose of age verification.

## 9. Changes to this Policy

We may revise this Policy in response to changes in law or in the App's features. Where a change is significant, we will announce it in the App or where this Policy is published. Continuing to use the App after a revision constitutes agreement to the revised Policy.

## 10. Governing law

The interpretation and application of this Policy are governed by the law of Japan.

## 11. Contact

For questions about this Policy or about how the App handles information, please contact:

- Hiroki Kataoka
- kyataoka.deve@gmail.com
