---
layout: default
title: Frontend Integration
---

# <span style="color: #f7931e;">DeviceConnect SDK: Frontend Integration Flow</span>

DeviceConnect empowers businesses with real-time, anonymized intelligence derived directly from mobile devices. It ensures smarter, faster, and more privacy-conscious decision-making through a streamlined SDK integration. Below are the key steps to integrate DeviceConnect in your Android app.

## <span style="color: #f7931e;">Step-by-Step Integration Guide</span>

### Step 1: Request Runtime Permissions

- Display a consent screen to inform users about the permissions being requested and why they matter.
- Refer to the **Handle Permissions** section for a comprehensive list of required permissions.
- Use the `remove` node marker to exclude any permission not required for your use case.

### Step 2: Create a Unique User

- After permission handling, invoke `createUser` with a unique `CUSTOMER_ID`.
- This ID acts as a pseudonymized identifier — avoid using phone numbers, emails, or other personal data.
- `createUser` also validates API credentials to ensure your integration is authorized before proceeding.
- Always call `createUser` even if some permissions are denied — the SDK syncs only what is available.

### Step 3: Start Data Synchronization

- Upon successful `createUser` response, call `startPeriodicSync` to begin data collection.
- The SDK continues syncing in the background as per the defined frequency and updates when new permissions are granted.
- Call these functions every time the app opens to ensure continuous background sync and permission adaptation.

## <span style="color: #f7931e;">Best Practices & Recommendations</span>

- **Multi-Process Apps:** Ensure manual SDK initialization before invoking `createUser`.
- **Push Notifications:** Forward all notifications to the SDK to avoid background process interruptions. See *Forward Notifications to SDK*.

## <span style="color: #f7931e;">Get Started Today</span>

Power your fintech platform with anonymized, real-time intelligence from DeviceConnect. Quick to integrate, privacy-respecting by design, and built for scale — DeviceConnect is your gateway to better credit outcomes.
