---
title: Privacy Policy
lang: en
---

> 🇬🇧 **English** · 🇩🇪 [Deutsche Version](../privacy-de/)

# Privacy Policy

**Last updated:** May 18, 2026

This Privacy Policy explains which personal data are processed when you use the iOS app **Crewzilla**, for what purposes, on what legal basis, and what rights you have.

---

## 1. Controller

The controller within the meaning of Art. 4 (7) GDPR is:

**Dominik Schmidt**
Kunigundenstraße 23i
91207 Lauf an der Pegnitz, Germany

E-mail: **domi_schmidt95@icloud.com**
VAT ID: {USTID}

---

## 2. Definitions

The definitions of Art. 4 GDPR apply (in particular "personal data", "processing", "controller", "processor").

---

## 3. Purposes and Legal Bases

Crewzilla is a social planning app for groups of friends. The following processing takes place:

### 3.1 Sign-up and Sign-in

**Data:** e-mail address, hashed password, username.
For "Sign in with Apple": Apple ID token (OIDC), the e-mail address Apple provides (possibly an Apple Private Relay address), and your full name on the first sign-in.

**Purpose:** create and manage your user account, authentication.
**Legal basis:** Art. 6 (1)(b) GDPR (performance of contract).

### 3.2 Profile

**Data:** username, display name, avatar image, onboarding status.
**Purpose:** identification within groups, UI rendering.
**Legal basis:** Art. 6 (1)(b) GDPR.

### 3.3 Groups

**Data:** group name, description, group image, invite code, memberships (including role and join date).
**Purpose:** delivering the core function "planning together in groups of friends".
**Legal basis:** Art. 6 (1)(b) GDPR.

### 3.4 Plans (including location data)

**Data:** title, description, emoji, status, date/time, **place name and GPS coordinates (latitude/longitude)**, budget, currency.
**Purpose:** collaborative activity planning; display of the location on a map (via Apple MapKit).
**Legal basis:** Art. 6 (1)(b) GDPR.

Note: GPS coordinates are derived solely from the place you manually select. Crewzilla does **not** track your current location.

### 3.5 RSVPs, polls, tasks, comments

**Data:** RSVP status (going / maybe / not going) with optional comment; poll questions, options and votes; tasks with assignment and completion state; comment texts with timestamp.
**Purpose:** coordination within plans.
**Legal basis:** Art. 6 (1)(b) GDPR.

### 3.6 Chat messages and images

**Data:** text messages, image attachments.
**Purpose:** group communication.
**Legal basis:** Art. 6 (1)(b) GDPR.

Messages and images are visible only to members of the respective group.

### 3.7 Expenses and settlement

**Data:** amounts, descriptions, category, **receipt photos**, payer, split between participants, date, exchange-rate and original-currency information.
**Purpose:** shared expense tracking and debt settlement within the plan.
**Legal basis:** Art. 6 (1)(b) GDPR.

Receipt photos are visible only to members of the respective plan.

### 3.8 Friendships and user search

**Data:** directed friend requests, status (pending / accepted / declined / blocked); search queries on the username prefix.
**Purpose:** finding and managing friends; inviting them to groups.
**Legal basis:** Art. 6 (1)(b) GDPR; for search additionally Art. 6 (1)(f) GDPR (legitimate interest: providing the "find friends" feature).

Search results are capped at 20 usernames per query.

### 3.9 Calendar synchronisation (opt-in)

**Data:** exclusively **start and end times** of your Apple Calendar events for the next 30 days.
**Not collected:** titles, descriptions, attendees, or locations of your events.

**Purpose:** display your availability to members of your groups.
**Legal basis:** Art. 6 (1)(a) GDPR (consent). You grant consent via the iOS system permission dialog and can revoke it at any time via iOS Settings.

### 3.10 Push notifications (opt-in)

**Data:** APNs device token, your chosen notification preferences per type (e.g. chat, plans, social).
**Purpose:** send notifications about activity in your groups.
**Legal basis:** Art. 6 (1)(a) GDPR (consent).

You may revoke the permission at any time via iOS Settings. Within the app each notification type can be toggled separately.

### 3.11 In-app notifications and activity log

**Data:** notification type, trigger, timestamp; plan-related events.
**Purpose:** transparency within a group (who did what and when).
**Legal basis:** Art. 6 (1)(f) GDPR (legitimate interest in traceability for group members).

### 3.12 In-app purchases / Crewzilla Plus

**Data:** app user ID (Supabase Auth UUID), Apple receipt data, subscription status (active, trial, expired, cancelled), purchase and renewal timestamps, App Store country, iOS version.
**Purpose:** providing the premium feature set (Crewzilla Plus), technical validation of the purchase (receipt validation), management of trial and renewal status, handling of renewal/cancellation/refund events.
**Legal basis:** Art. 6 (1)(b) GDPR (performance of contract).

Payment itself is processed exclusively via your **Apple ID**; Crewzilla does **not** receive any payment or credit-card data from you.

---

## 4. Recipients and Processors

We use the following external service providers:

### Supabase Inc.
- **Seat:** USA. **Data hosting:** Frankfurt am Main, Germany (region `eu-central-1`).
- **Function:** authentication, database (PostgreSQL), file storage, realtime, edge functions.
- **Data processed:** all app data described above.
- **Legal basis for transfer:** data processing agreement under Art. 28 GDPR. Where access from the USA occurs, EU Standard Contractual Clauses pursuant to Implementing Decision (EU) 2021/914 apply.

### Apple Inc.
- **Seat:** USA.
- **Function:**
  - **Sign in with Apple** (OIDC-based authentication),
  - **Apple Push Notification Service (APNs)** (delivering push messages to your device),
  - **MapKit** (rendering maps in the app),
  - **EventKit** (local access to your Apple Calendar, exclusively on your device),
  - **In-app purchases / App Store** (processing and billing of Crewzilla Plus subscriptions via the Apple ID).
- **Data processed:** Apple ID token, APNs device token, map requests, receipt data for Crewzilla Plus purchases.
- **Legal basis for transfer:** Apple Developer Program License Agreement, Apple Data Processing Addendum, EU Standard Contractual Clauses; Apple is certified under the EU-US Data Privacy Framework.

### RevenueCat, Inc.
- **Seat:** USA (San Francisco, CA).
- **Function:** management of Crewzilla Plus in-app purchases: server-side validation of Apple receipts, synchronisation of subscription and entitlement status, processing of server notifications for renewals, cancellations and refunds.
- **Data processed:** app user ID (Supabase Auth UUID), Apple receipt data, subscription and entitlement status, App Store country, iOS version, timestamps of purchase events.
- **Legal basis for transfer:** data processing agreement under Art. 28 GDPR (RevenueCat Data Processing Addendum), EU Standard Contractual Clauses pursuant to Implementing Decision (EU) 2021/914. RevenueCat is certified under the EU-US Data Privacy Framework.

### We expressly do NOT use

- Advertising networks or advertising IDs (IDFA is not requested)
- Tracking SDKs (Crewzilla does not use `AppTrackingTransparency`)
- Analytics tools (Firebase Analytics, PostHog, Mixpanel etc.)
- Crash-reporting SDKs (Sentry, Crashlytics etc.)
- Third-party cookies (Crewzilla is a native app, not a website)

---

## 5. International Transfers

Database and storage content is hosted in the EU (Frankfurt). Access by providers (Supabase, Apple) from the USA is possible. For such transfers we rely on:

- **Standard Contractual Clauses** (SCCs, Implementing Decision (EU) 2021/914), and
- **EU-US Data Privacy Framework** (for Apple Inc.).

---

## 6. iOS Permissions

Crewzilla requests only the permissions necessary for a given function. You can revoke each one at any time via iOS Settings.

| Permission | Purpose | If denied |
|---|---|---|
| Calendar | Calendar sync (availability) | Calendar sync disabled |
| Photo Library (write) | Save chat images to your Photos | Saving not possible |
| Notifications (push) | Push notifications | No push; in-app notifications still work |

---

## 7. Storage Duration

- **Account data** is stored as long as your account exists.
- **Content (plans, chats, expenses)** is stored as long as the respective group exists or you remain a member.
- **On account deletion** your profile, avatar, memberships and personal records (own RSVPs, votes, tasks, expenses, settlements) are deleted without undue delay. Content you contributed to shared contexts (chat messages, comments) remains there with anonymised sender, so the remaining group members can still read the conversation.
- **Calendar busy times** are overwritten on each sync and fully deleted when the function is disabled.
- **APNs device tokens** are removed on sign-out and on account deletion.

Data is deleted unless statutory retention obligations apply. In encrypted backup systems, data may remain for a limited period for technical reasons until it is automatically overwritten.

---

## 8. Your Rights

Under the GDPR you have the right to:

- **Access** the personal data we hold about you (Art. 15)
- **Rectification** of inaccurate data (Art. 16)
- **Erasure** ("right to be forgotten", Art. 17)
- **Restriction** of processing (Art. 18)
- **Data portability** (Art. 20)
- **Object** to processing based on legitimate interests (Art. 21)
- **Withdraw consent** (e.g. calendar, push) with effect for the future (Art. 7 (3))
- **Lodge a complaint** with a data-protection supervisory authority (Art. 77), in particular the competent authority of your place of residence or the German Federal Commissioner for Data Protection (BfDI).

Requests should be sent to: **domi_schmidt95@icloud.com**

---

## 9. In-App Account Deletion

You can permanently delete your account at any time:

**Settings → Delete account → Confirm**

Deletion is carried out without undue delay; see Section 7 for content in shared contexts.

---

## 10. Note on "Sign in with Apple"

When signing in with Apple, Apple lets you decide whether to share your real e-mail address or an **Apple Private Relay address** (`@privaterelay.appleid.com`) with Crewzilla. Crewzilla stores only what Apple provides. If you choose Private Relay, Apple forwards e-mails to your real address without disclosing it to us.

Your **full name** is provided by Apple to Crewzilla only on the **first** sign-in; subsequent sign-ins return no name.

---

## 11. Data Security

- **Transport encryption:** communication between the app and the server is exclusively over TLS 1.2 or higher.
- **Encryption at rest:** data and files at Supabase are stored encrypted (AES-256).
- **Row-Level Security:** record-level access is database-enforced and restricted to authorised users (members of the respective group).
- **Passwords** are stored only as hashes (bcrypt, Supabase standard).
- **Apple Sign-In** uses nonce-based OIDC validation.
- **Non-public storage buckets** for chat images and receipts; access only for group or plan members.

---

## 12. No Advertising, No Tracking

Crewzilla operates **entirely without advertising, tracking, or marketing profiling**. **No data is shared with third parties for advertising purposes.** No advertising IDs are collected and no tracking SDKs are used.

---

## 13. Minimum Age

The use of Crewzilla is permitted only for persons aged **18 years or older**. If you are younger, please do not create an account. If we learn that an account is operated by a person under 18, we will suspend or delete it.

---

## 14. Changes to this Policy

We may adjust this Privacy Policy to reflect changes in the legal situation or in the app's functions. The most recent version, dated at the top, is always available at this URL and in the app under **Settings → Privacy**. For material changes we will notify you on the next app launch or by e-mail.

---

## 15. Contact

For questions about data processing:

**Dominik Schmidt**
Kunigundenstraße 23i
91207 Lauf an der Pegnitz, Germany
E-mail: **domi_schmidt95@icloud.com**
