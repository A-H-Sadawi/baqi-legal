# Privacy Policy — Baqi (باقي)

**Last updated:** October 2026

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
On Android, Baqi can read the messages on your phone, but it only processes messages from bank and financial-service senders it recognizes. Anything that does not look like a bank transaction is discarded.

The text of each bank transaction message is saved in your Baqi account together with the transaction, so Baqi can show you how each transaction was detected. Other users cannot see it.

Baqi is not connected to your bank and never asks for your online banking login.

### 2.4 iPhone
Baqi does not read your messages on iPhone. On iPhone you add your accounts and transactions manually. There is no service that forwards messages from iPhone to Baqi.

### 2.5 Usage and Technical Data
- App version and device operating system (for crash reporting and support)
- We do not use advertising identifiers or third-party analytics trackers

### 2.6 In-App Guide
If you use the in-app guide, Baqi records which guide steps you started, skipped or finished, and when. These records contain no message text and no amounts, and they are deleted with your account.

### 2.7 Bank Requests
If you ask Baqi to add a bank, it stores the bank name you type, along with your app version and language. This data contains no message text and is deleted with your account.

---

## 3. How We Use Your Data

| Purpose | Data Used |
|---|---|
| Display your balance and transaction history | Account and transaction data |
| Send payment reminders and budget alerts | Loan, subscription, and budget data |
| Detect transactions automatically | Bank message text (Android) |
| Process in-app purchases | Handled by Apple App Store / Google Play — we do not store payment card details |
| Provide premium features | Subscription status via RevenueCat (linked to your Baqi user ID) |

---

## 4. Data Storage and Security

- All data is stored in Supabase (PostgreSQL), hosted in the **UAE region** (closest available to KSA).
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
| Anthropic (AI service) | Reading bank messages Baqi cannot read itself | When Baqi cannot read a bank message itself, the text of that message may be sent to extract the amount and the merchant. Names, shop names and numbers in the message may be included. This happens automatically during a scan. |
| RevenueCat | Subscription management | Your Baqi user ID and purchase status |
| Sentry | Crash reports | Your user ID, app version, device type and technical details of an error. Baqi's code does not attach message text to error reports. |
| Clearbit | Merchant and service logos | The website domain of a merchant or service, so its logo can be shown |
| Apple App Store / Google Play | In-app purchases | Handled entirely by Apple/Google |

---

## 6. Bank Message Text (Special Category)

We treat bank message text with extra care:

- **Android**: messages are read on your phone. The text of each bank transaction message is saved in your account with the transaction, so Baqi can show how it was detected.
- **AI service**: a bank message Baqi cannot read itself may be sent to an AI service (Anthropic) to extract the amount and merchant. Names and shop names in the message may still be included.
- Baqi only processes messages from bank and financial-service senders it recognizes.
- **iPhone**: Baqi does not read your messages on iPhone (see Section 2.4).
- You can stop SMS reading at any time in your phone's settings.

---

## 7. Data Retention

- Your data is retained for as long as your account is active.
- Delete Account in Settings deactivates your account. To permanently delete your account and data, email abdulrahmansadawi@gmail.com from your registered address; we delete it within 30 days. The steps are in Section 13 below.
- If your premium subscription expires, your data is preserved — only premium features are restricted. A 14-day grace period applies.

---

## 8. Your Rights

You have the right to:

- **Access** your data — all data is visible within the app
- **Correct** your data — edit any transaction, account, or profile field at any time
- **Delete** your account and all associated data — Settings → Account → Delete Account deactivates your account; to delete it permanently, see Section 7 and Section 13
- **Export** your data — contact us and we will provide a JSON export within 30 days
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

**Email:** abdulrahmansadawi@gmail.com  
**App:** Settings → Help & Support

---

## 12. Governing Law

This policy is governed by the laws of the **Kingdom of Saudi Arabia** and applicable data protection regulations including the **Personal Data Protection Law (PDPL)**.

---

## 13. How to Delete Your Account

### In the app

Open **Settings → Account → Delete Account**. In the version of Baqi installed today this **deactivates** your account; it does not remove your data. To delete your account and data permanently, request it by email (below).

### Request deletion by email

1. Send an email to **abdulrahmansadawi@gmail.com** from the email address you registered with in Baqi. We cannot act on a request sent from a different address.
2. Use the subject line: **Delete my Baqi account**.
3. We confirm that the request comes from the registered address, delete your account, and reply to confirm.

### What is deleted

Your Baqi account and sign-in record, and everything saved under it: accounts, transactions including the saved text of bank messages, loans, goals, budgets, obligations, receivables, notifications, reports and requests you sent, and your settings. We delete it within 30 days of your request.

Crash reports are held by our error-reporting service under its own retention period and are not part of your Baqi account data.

### Your Google Play subscription

Deleting your account does **not** cancel a Google Play subscription. Cancel it yourself in Google Play (Play Store → profile → Payments & subscriptions → Subscriptions).
