# Chrome Web Store Privacy Policy

## Single Purpose Description

**One-sentence summary:**
WhatsApp integration for energy business operations, enabling authorized users to send business messages for alerts, approvals, and customer communications through the EnergyNow management platform.

**Detailed description (for store listing):**
EnergyNow Bridge integrates WhatsApp Web with the EnergyNow business management platform. It enables authorized business users to send WhatsApp messages for energy transaction alerts, inventory management, overhead tracking, and operational approvals. The extension provides a message queue system for bulk messaging campaigns and real-time notifications for business events.



## Permission Justifications

### activeTab
Required to detect when WhatsApp Web is open and verify connection status without accessing all browser tabs.

### storage
Stores JWT authentication tokens, user session data, message queues, campaign templates, and extension settings locally.

### background
Maintains persistent service worker for connection monitoring, message queue processing, and coordinating message delivery.

### scripting
Injects content scripts into WhatsApp Web to access messaging APIs and enable programmatic message sending.

### tabs
Detects WhatsApp Web tabs, opens WhatsApp Web when needed, and sends messages to the correct tab.

### alarms
Schedules periodic tasks: connection checks, queue processing, message retries, and token refresh.

### Host: web.whatsapp.com
**CORE FUNCTIONALITY** - Required to inject scripts and access WhatsApp's messaging APIs for sending business messages.

### Host: api.energynow.in
Communicates with EnergyNow backend to fetch business data (alerts, approvals, transactions, overhead tasks).

### Host: energynow.in
User authentication, OAuth callbacks, and session management.

### Host: ipapi.co
One-time country detection to auto-select country code for phone number formatting (UX improvement only).



## Remote Code

**Does your extension execute remote code?** NO

**Justification:** All code is bundled with the extension package. Only JSON data is fetched from APIs, never executable JavaScript. Content Security Policy prevents remote code execution.



## Data Usage Certification

### Personally Identifiable Information (PII)
**Collected:** YES
- User email (for login)
- User name and role (from EnergyNow account)
- Organization code (company ID)
- WhatsApp phone number (auto-detected from WhatsApp Web)

**Use:** Authentication, authorization, display in UI, verify authorized messaging accounts
**Shared with:** EnergyNow API only (first-party service)
**Transmission:** HTTPS only
**Storage:** Chrome storage API (encrypted)



### Health Information
**Collected:** NO


### Financial and Payment Information
**Collected:** NO

**Note:** Extension displays read-only transaction records for approval workflows but does NOT collect payment details, process transactions, or handle financial data.



### Authentication Information
**Collected:** YES
- JWT tokens (from EnergyNow API)
- Session timestamps

**Use:** API authentication
**Security:** Stored encrypted in Chrome storage, transmitted via HTTPS only, auto-expire
**Shared with:** EnergyNow API only



### Personal Communications
**Collected:** YES
- Outbound message content (user-typed business messages)
- Recipient phone numbers (customers, vendors)
- Campaign templates

**Use:** Sending business communications via WhatsApp Web
**Important:** Extension does NOT access:
- Incoming WhatsApp messages
- Personal conversations
- Chat history
- Contact lists (except numbers explicitly entered)

**Transmission:** Through WhatsApp's infrastructure (subject to WhatsApp's privacy policy)
**Retention:** Stored locally until delivery, then optionally cleared



### Location
**Collected:** NO

**Note:** Uses ipapi.co once to detect country code (e.g., "IN") for phone formatting UX. Does NOT track GPS, precise location, or IP addresses.


### Web History
**Collected:** NO

Extension only detects if web.whatsapp.com is open. Does not monitor, track, or access other websites, URLs, bookmarks, or browsing history.



### User Activity
**Collected:** YES (local only)
- Message sending statistics (count, status)
- Extension usage (which tabs viewed)
- Queue status (pending, sent, failed)

**Use:** Display stats in UI, retry failed messages, show activity logs
**Storage:** Local only (Chrome storage)
**Analytics:** NO analytics services used
**Sharing:** NOT transmitted to any server



### Website Content
**Accessed:** YES
- WhatsApp Web page (to inject messaging scripts)
- EnergyNow API responses (business data)

**Not Accessed:**
- WhatsApp chat history
- Received messages
- Media files
- Other websites

**Modifications:** Scripts injected into web.whatsapp.com only for messaging functionality


## Data Handling Practices Summary

| Data Type | Collected | Use | Encrypted | Shared | Retention |
|-----------|-----------|-----|-----------|--------|-----------|
| Email/Name | Yes | Authentication | Yes | EnergyNow API only | Until logout |
| WhatsApp # | Yes | Authorization check | Yes | EnergyNow API only | Until logout |
| Message content | Yes | Send via WhatsApp | Yes | WhatsApp only | Until delivered |
| Auth tokens | Yes | API access | Yes | EnergyNow API only | 24 hours |
| Health info | No | - | - | - | - |
| Financial info | No | - | - | - | - |
| Location | No | - | - | - | - |
| Web history | No | - | - | - | - |



## Certification Statements

✅ This extension complies with Chrome Web Store policies
✅ This extension complies with Google's Limited Use requirements
✅ Data use is limited to providing core functionality
✅ No data is sold to third parties
✅ No data is used for advertising or profiling
✅ All data transfers are encrypted (HTTPS)
✅ Users can delete data via logout/uninstall
✅ Privacy policy is publicly accessible



## Privacy Policy URL

**For Chrome Web Store listing:**
https://github.com/[your-repo]/energynow-extension/blob/main/PRIVACY.md

*(Update with actual GitHub URL or host PRIVACY.md on energynow.in)*



## Support Contact

**Email:** support@energynow.in
**Website:** https://energynow.in

---

**Prepared for:** Chrome Web Store Submission
**Extension Version:** 1.0.0
**Date:** October 4, 2025
