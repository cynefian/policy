# Privacy Policy – EnergyNow Bridge Chrome Extension

*Last updated: October 4, 2025*

Cynefian (“we,” “our,” or “us”) is committed to protecting the privacy of users of the **EnergyNow Bridge Chrome Extension** (the “Extension”). This Privacy Policy explains what data we collect, how we use it, and the rights you have as a user.

By installing and using the Extension, you agree to the terms outlined in this Privacy Policy.

---

## 1. Purpose of the Extension

The Extension integrates **WhatsApp Web** with the **EnergyNow business management platform**. It allows authorized business users to:

* Send individual/bulk WhatsApp messages for transaction alerts, inventory updates, approvals, and other custom business-related messages.
* Manage message queues for bulk or campaign-based communication.
* Receive real-time notifications related to business operations.

The Extension does **not** access personal WhatsApp messages, media files, or unrelated browsing activity.

---

## 2. Data We Collect

### Personally Identifiable Information (PII)

* **Email, Name, Role** – collected from your EnergyNow account for authentication and display.
* **Organization Code** – used to verify your company identity.
* **WhatsApp Phone Number** – detected from WhatsApp Web to authorize business messaging.

### Authentication Information

* **JWT Tokens & Session Data** – required to authenticate with EnergyNow APIs.
* Tokens are encrypted, stored locally, and automatically expire.

### Messaging Data

* **Outbound Message Content** – user-typed messages, recipient numbers, and campaign templates.
* Used exclusively to send business communications via WhatsApp.
* Incoming messages, contacts, and chat history are **not collected**.

### Extension Activity

* **Message Logs & Status** – includes sent, pending, and failed message counts.
* Stored locally to enable retries and provide user visibility.

### Location & Device

* **One-time Country Code Detection** – via ipapi.co, to auto-format phone numbers.
* No precise location, GPS, or IP tracking is performed.

---

## 3. Data We Do Not Collect

* **Health Information** – not collected.
* **Financial or Payment Information** – not collected.
* **Browsing History** – not collected, aside from detecting if WhatsApp Web is open.
* **Incoming WhatsApp Messages, Media, or Contacts** – never accessed.

---

## 4. How We Use Data

We use collected data only to:

* Authenticate users and authorize messaging.
* Deliver business messages through WhatsApp.
* Provide transaction alerts, approval workflows, and operational notifications.
* Improve usability (e.g., country code detection, retrying failed messages).

We do **not**:

* Sell or share data with third parties.
* Use data for advertising, profiling, or analytics.

---

## 5. Data Sharing

* **EnergyNow API** – receives authentication details, organization code, and limited business metadata.
* **WhatsApp Infrastructure** – used to deliver outbound messages entered by the user.
* No other third parties receive data.

All data transfers are encrypted using **HTTPS**.

---

## 6. Data Retention

* **Auth Tokens** – valid for 24 hours and refreshed automatically.
* **Message Content** – retained locally until delivery; cleared after successful send or logout.
* **User Info (Email, Role, WhatsApp #)** – retained only during an active session.
* Users may delete all data at any time by logging out or uninstalling the Extension.

---

## 7. Browser Permissions 

The Extension requests the following browser permissions strictly for core functionality:

* **activeTab / tabs** – to detect WhatsApp Web and manage messaging tabs.
* **storage** – to securely store tokens, message queues, and settings.
* **background / alarms** – to process message queues, retries, and session refresh.
* **scripting** – to inject scripts into WhatsApp Web for programmatic messaging.
* **Host permissions** – limited to:

  * `web.whatsapp.com` (messaging integration)
  * `api.energynow.in` (business data & alerts)
  * `energynow.in` (authentication & session management)
  * `ipapi.co` (one-time country detection)

---

## 8. Security Measures

* All communication is encrypted using HTTPS.
* Authentication tokens are encrypted and expire automatically.
* No remote code is executed; only bundled extension code runs.
* Users control their data and may clear it anytime by uninstalling the Extension.

---

## 9. User Rights

As a user, you have the right to:

* Access the data you provide through the Extension.
* Request deletion of data by logging out or uninstalling.

---

## 10. Compliance

This Extension complies with:

* **Chrome Web Store policies**
* **Google’s Limited Use requirements**

We certify that data is used solely for providing the stated business functionality.

---

## 11. Contact Information

If you have questions or concerns about this Privacy Policy, please contact:

**Support Email:** [support@cynefian.com](mailto:support@cynefian.com)
**Website:** [https://energynow.in](https://energynow.in)

---

## 12. Policy Updates

We may update this Privacy Policy from time to time. Updates will be posted on our website and the Chrome Web Store listing. Continued use of the Extension constitutes acceptance of the updated policy.

---

**Prepared for Chrome Web Store Submission – Extension Version 1.0.0**
