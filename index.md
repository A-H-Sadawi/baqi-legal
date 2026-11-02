# Privacy Policy — Baqi (باقي)

**Last updated:** November 2026

---

## 1. Introduction

Baqi ("we", "our", "the app") is a personal finance tracking application for individuals in the Kingdom of Saudi Arabia. This Privacy Policy explains what data we collect, how we use it, and your rights as a user.

Baqi is not a licensed financial institution. All financial summaries and insights shown in the app are informational only and do not constitute financial advice.

---

## 2. Data We Collect

### 2.1 Account Data
- Email address (used for login and account recovery)
- First name (used for personalised greetings)
- Language preference

### 2.2 Financial Data You Enter
- Bank account names and opening balances (you enter these manually — we never connect directly to any bank)
- Transactions you add manually or via SMS parsing
- Loans, subscriptions, goals, and budgets you create

### 2.3 Bank Message Text (Android)
On Android, Baqi can read the messages on your phone, but it only processes messages that look like bank transaction messages. Other messages are not saved.

The text of each bank transaction message is saved in your Baqi account together with the transaction, so Baqi can show you how each transaction was detected. Other users cannot see it.

A message that looks like a bank message but that Baqi cannot read is left out of your transactions. It may first be sent to an AI service (see Section 5), and only if you agree can it be sent to the Baqi team (see Section 2.9).

Baqi is not connected to your bank and never asks for your online banking login.

### 2.4 iPhone
Baqi does not read your messages on iPhone. On iPhone you add your accounts and transactions manually. There is no service that forwards messages from iPhone to Baqi.

### 2.5 Usage and Technical Data
- Crash reports (see Section 5, Sentry)
- When you run a message scan during setup, Baqi records your phone's model and manufacturer, the Android version, the app version, whether SMS permission was granted, whether the scan finished or failed, and the error text if it failed
- Baqi records the build number and platform of the app you have installed, and roughly when you last opened it
- We do not use advertising identifiers or third-party analytics trackers

### 2.6 In-App Guide
If you use the in-app guide, Baqi records which guide steps you started, skipped or finished, and when. These records contain no message text and no amounts, and they are deleted with your account.

### 2.7 Bank Requests
If you ask Baqi to add a bank, it stores the bank name you type, along with your app version and language. This data contains no message text and is deleted with your account.

### 2.8 Reports You Send
If you report a transaction as wrong, Baqi saves your report: the saved message text of that transaction, its merchant, amount and type, the problem types you picked, and any note you typed. You choose to send it. It is used to find and fix mistakes in how Baqi reads bank messages. It is deleted with your account.

### 2.9 Helping Improve Baqi
On Android, when Baqi finds a message that looks like it comes from a bank but cannot read it, it asks whether you want to help. If you agree:
- Baqi sends the message to the Baqi team: the full, unchanged text and the sender name or number it came from. The text can contain amounts, balances, names and parts of account or card numbers.
- It is used only to teach Baqi to read that bank's messages.
- Your choice is saved in your account. After you agree, Baqi sends such messages automatically each time it finds one.

If you say no, nothing is sent automatically. Baqi may ask about a single message and sends it only if you tap to share it.

To withdraw your agreement, email baqi.app.sup@gmail.com from your registered address. We turn sharing off for your account and delete the messages you have already shared.

---

## 3. How We Use Your Data

| Purpose | Data Used |
|---|---|
| Display your balance and transaction history | Account and transaction data |
| Send payment reminders and budget alerts | Loan, subscription, and budget data |
| Detect transactions automatically | Bank message text (Android) |
| Help improve how Baqi reads bank messages | Messages you agree to share, and reports you send |
| Process in-app purchases | Handled by Apple App Store / Google Play — we do not store payment card details |
| Provide premium features | Subscription status via RevenueCat (linked to your Baqi user ID) |

---

## 4. Data Storage and Security

- All data is stored in Supabase (PostgreSQL), hosted in Seoul, South Korea. This is outside Saudi Arabia.
- All data in transit is encrypted using TLS.
- All data at rest is encrypted by the hosting provider.
- Row-Level Security (RLS) is enforced on every database table — your data is never accessible to other users.
- We never store raw bank credentials. Balances are described as "Tracked" or "Estimated" — never as live bank data.
- The Baqi team may access account data, including saved message text, to provide support, fix problems and improve how Baqi reads bank messages.

---

## 5. Data Sharing

We do not sell your data. We share data only with the following service providers, strictly to operate the app:

| Provider | Purpose | Data Shared |
|---|---|---|
| Supabase | Database hosting | All app data (encrypted at rest by the hosting provider), including the saved text of your bank transaction messages |
| Anthropic (AI service) | Reading bank messages Baqi cannot read itself | When Baqi cannot read a bank message itself, the text of that message may be sent to extract the amount and the merchant. Names, shop names and numbers in the message may be included. This happens automatically during a scan. Long digit runs (5 digits or more, such as account and card numbers) are hidden before sending, keeping only the last 4. |
| RevenueCat | Subscription management | Your Baqi user ID and purchase status |
| Sentry | Crash reports | Your user ID, app version, device type and technical details of an error. Baqi's code does not attach message text to error reports. |
| Clearbit | Merchant and service logos | The website domain of a merchant or service, so its logo can be shown |
| Apple App Store / Google Play | In-app purchases | Handled entirely by Apple/Google |

---

## 6. Bank Message Text (Special Category)

We treat bank message text with extra care:

- **Android**: messages are read on your phone. The text of each bank transaction message is saved in your account with the transaction, so Baqi can show how it was detected.
- **AI service**: a bank message Baqi cannot read itself may be sent to an AI service (Anthropic) to extract the amount and merchant. Long digit runs (5 digits or more, such as account and card numbers) are hidden before sending, keeping only the last 4. Names and shop names in the message may still be included.
- **Sharing with the Baqi team**: only if you agree (Section 2.9), a bank-style message Baqi cannot read is sent, unchanged, to the Baqi team so support for that bank can be added. You can also send a report about a single transaction (Section 2.8).
- Baqi only processes messages that look like bank transaction messages.
- **iPhone**: Baqi does not read your messages on iPhone (see Section 2.4).
- You can stop SMS reading at any time in your phone's settings.

---

## 7. Data Retention

- Your data is retained for as long as your account is active.
- Delete Account in Settings permanently deletes your account, your data and your sign-in record immediately. You can also request deletion by email or from the [account deletion page](#13-how-to-delete-your-account).
- If your premium subscription expires, your data is preserved — only premium features are restricted. A 14-day grace period applies.

---

## 8. Your Rights

You have the right to:

- **Access** your data — all data is visible within the app
- **Correct** your data — edit any transaction, account, or profile field at any time
- **Delete** your account and all associated data — Settings → Account → Delete Account, or see the account deletion page
- **Export** your data — contact us and we will provide a JSON export within 30 days
- **Withdraw consent** for sharing unrecognized messages (Section 2.9) — email baqi.app.sup@gmail.com from your registered address
- **Withdraw consent** for SMS reading — disable in device settings at any time

---

## 9. Children

Baqi is not intended for users under the age of 18. We do not knowingly collect data from minors.

---

## 10. Changes to This Policy

We will notify you of material changes to this policy via a notification in the app. The "Last updated" date at the top of this page will always reflect the most recent revision.

---

## 11. Contact

For privacy questions, data export requests, or account deletion assistance:

**Email:** baqi.app.sup@gmail.com

**App:** Settings → Help & Legal → Send Feedback

---

## 12. Governing Law

This policy is governed by the laws of the **Kingdom of Saudi Arabia** and applicable data protection regulations including the **Personal Data Protection Law (PDPL)**.

---

## 13. How to Delete Your Account

### In the app

Open Settings → Account → Delete Account and type your email to confirm. Your account, your data and your sign-in record are permanently deleted immediately. This cannot be undone.

### Request deletion by email

1. Send an email to **baqi.app.sup@gmail.com** from the email address you registered with in Baqi. We cannot act on a request sent from a different address.
2. Use the subject line: **Delete my Baqi account**.
3. We confirm that the request comes from the registered address, delete your account, and reply to confirm.

### What is deleted

Your Baqi account and sign-in record, and everything saved under it: accounts, transactions including the saved text of bank messages, loans, goals, budgets, obligations, receivables, notifications, reports and requests you sent, and your settings. For email requests, we delete it within 30 days of your request.

Crash reports are held by our error-reporting service under its own retention period and are not part of your Baqi account data.

### Your Google Play subscription

After your account is deleted, Baqi also asks RevenueCat, the service that manages subscriptions, to delete your customer record. This step is best-effort and does not affect whether your account is deleted.

Deleting your account does **not** cancel a Google Play subscription. Cancel it yourself in Google Play (Play Store → profile → Payments & subscriptions → Subscriptions).
