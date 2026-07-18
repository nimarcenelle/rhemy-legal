# STACK Privacy Policy

**Effective date: July 18, 2026**

This Privacy Policy describes how STACK ("the app," "we," "us") handles your information. STACK is designed around a simple principle: **your data lives on your phone.** There are no accounts, no sign-ups, no cloud database of users, and no advertising or analytics SDKs.

Please read this policy together with our [Terms of Service](./terms-of-service).

## The short version

- Everything the app knows about you — your quiz answers, priorities, scanned products, grades, scores, and check-ins — is stored **only on your device**.
- Photos you take (your face, your shelf, a product) are sent **once** to a vision API to read appearance signals or label text, then discarded. They are never saved by us, never used to identify you, and never used to train models by us.
- We never see your name, email, or identity. Purchases are tied to an **anonymous identifier**, not to you.
- You can erase everything the app stores with one tap (Settings → Delete everything).
- We do not sell, rent, or share your personal information for advertising. We have no advertising relationships.

## Information the app handles

### 1. Information stored only on your device

The following never leaves your phone. It is stored in the app's local database and is deleted when you use "Delete everything" or uninstall the app:

- **Quiz answers** (goal, commitment, training, sleep, energy, diet, caffeine, weakest link)
- **Face appearance signals** — seven numeric scores (e.g., dark circles, dullness) derived from your face photo. The *numbers* are stored; the *photo* is not.
- **Your priority profile** (the ranked priorities computed from quiz + face signals)
- **Scanned products, ingredients, grades, reasons, and Stack Scores**
- **Quick-scan history, score snapshots, and weekly check-ins**
- **Monthly cost figures you enter**
- **Local usage counters** (e.g., session count, whether you've seen certain screens) kept in app storage
- **Local diagnostics** — the app keeps a small on-device log of feature events (e.g., "scan completed") to aid debugging. This log never leaves your device and is not connected to any analytics service.

### 2. Photos — processed, not stored

STACK uses your camera (with your permission) for three features: the face scan, the shelf scan, and Scan Anywhere. You can also pick a screenshot from your photo library for Scan Anywhere.

When you capture or select a photo:

- The photo is transmitted over an encrypted connection (HTTPS) to **Google's Gemini API**, which returns either appearance-signal numbers (face scan) or structured label text (product scans).
- The photo is held in memory only for the duration of that request and is then discarded by the app. The app never writes your photos to disk and never uploads them anywhere else.
- Photos are sent without your name, contact details, or any account identifier — we don't have any.
- Google processes the image as our service provider to provide the extraction result. Google's handling of API data is described in Google's own terms and privacy documentation for the Gemini API. We have configured nothing that links these requests to your identity.

If you deny camera access, you can still use the app by entering products manually.

### 3. Purchases

Payments are processed entirely by **Apple** through your App Store account. We never see or store your payment details, card numbers, or billing address.

To deliver and restore purchases, the app uses **RevenueCat**, a purchase-infrastructure service. RevenueCat receives:

- An **anonymous, randomly generated app identifier** (not your name, email, or Apple ID)
- Your purchase receipts and subscription status
- Basic device information necessary to validate purchases (e.g., device model, OS version, app version)

We never attach your identity to this anonymous ID, and we do not use it to track you across other companies' apps or websites. RevenueCat acts as our service provider and processes this data per its own privacy policy.

### 4. Notifications

All reminders (report reminders, rescan nudges, weekly check-ins) are **local notifications scheduled on your device**. There is no push-notification server and nothing is transmitted to schedule them. You can disable them at any time in iOS Settings → Notifications → STACK.

### 5. Photo library saving

If you tap "Save image" on your Stack Facts share card, the app asks for permission to **add** the image to your photo library. The app cannot read, browse, or view your existing photos through this permission.

## What we do NOT collect

- No name, email address, phone number, or contact information
- No account credentials (there are no accounts)
- No precise or approximate location
- No advertising identifiers; no cross-app or cross-site tracking
- No third-party analytics (no Mixpanel, Firebase, Meta, Google Analytics, or similar SDKs)
- No health records, and no data from HealthKit or any health platform
- No contacts, messages, browsing history, or files

## How information is used

The information above is used solely to:

1. Grade your products and compute your Stack Score and priority profile (on-device);
2. Extract label text and appearance signals from photos you choose to submit (via the vision API);
3. Deliver, restore, and manage purchases you make;
4. Schedule the local reminders you've enabled;
5. Maintain and debug the app.

We do not use your information for advertising, profiling for advertising, or sale to data brokers. We do not use your photos or data to train machine-learning models.

## Sharing

We share information only with the service providers named above (Google — vision extraction; RevenueCat — purchase management; Apple — payment processing), only to the extent described, and with no one else — except if required by law, or to protect the rights, safety, or property of users or the public. Because we hold no user database, there is very little we *could* disclose: your profile and history exist only on your phone.

If the app's ownership changes, on-device data stays on your device; any successor would be bound by a policy at least as protective for the limited service-provider data described here.

## Data retention

- **On-device data**: retained until you delete it (Settings → Delete everything) or uninstall the app. We have no copy.
- **Photos**: not retained. Discarded after the extraction response.
- **Purchase records**: retained by Apple and RevenueCat per their policies and as required for tax/accounting law. The anonymous purchase identifier persists so your purchases can be restored.

## Your choices and rights

- **Delete everything**: Settings → Delete everything wipes all local data. Uninstalling the app does the same.
- **Camera / photo permissions**: manage anytime in iOS Settings → Privacy.
- **Notifications**: manage anytime in iOS Settings → Notifications.
- **Purchases**: manage or cancel subscriptions in your App Store account settings; request refunds from Apple at reportaproblem.apple.com.

Depending on where you live (e.g., the EEA/UK under GDPR, or California under the CCPA/CPRA), you may have rights to access, correct, delete, or port personal information, and to object to or restrict certain processing. Because we don't maintain user accounts or a server-side profile of you, most of these rights are satisfied directly by the on-device controls above. For anything else — including questions about the anonymous purchase identifier — contact us at the address below and we will respond within the time required by applicable law. We do not discriminate against you for exercising your rights. We do not "sell" or "share" personal information as those terms are defined in the CCPA/CPRA.

For users in the EEA/UK: the legal bases for the limited processing described here are **performance of a contract** (grading the photos and answers you submit; delivering purchases) and **legitimate interests** (app functionality and debugging). Photo processing happens only at your initiative each time you tap scan. Data sent to the vision API and purchase infrastructure may be processed on servers in the United States; these transfers rely on the providers' applicable safeguards (such as standard contractual clauses).

## Security

Data in transit uses TLS (HTTPS). On-device data is protected by iOS's built-in encryption and your device passcode. No method of transmission or storage is 100% secure, but our architecture minimizes risk by keeping your data off servers in the first place.

## Children

STACK is intended for adults and is not directed to children under 13 (or the equivalent minimum age in your jurisdiction). We do not knowingly collect personal information from children. If you believe a child has used the app and submitted a photo, contact us and note that photos are, in any case, not retained.

## Changes to this policy

If we change this policy, we will update the effective date above and, for material changes, present a notice in the app before the change takes effect. Continued use after the effective date constitutes acceptance.

## Contact

Questions or requests about privacy:

**Email:** rhemy.app@gmail.com

---

*Summary of third parties: Apple (payments), Google Gemini API (transient photo extraction), RevenueCat (anonymous purchase management). No others.*
