---
layout: default
title: Introduction
---

# Credeau: Integration Flow

Follow the steps below to securely collect device intelligence and access real-time insights via Credeau.

## Credeau SDK Integration Summary

1. ### User Permissions & Consent
   - Request user permissions to enable anonymized device data collection.
   - Ensure compliance with all applicable privacy laws and regulatory guidelines.
   - Clearly communicate the purpose of data collection to foster user trust.

2. ### SDK Initialization & User Creation
   - Initialize the SDK early in the app’s lifecycle (e.g., splash screen or main activity).
   - Assign a unique, custom-generated user hash. **Do not use or store PII.**
   - Enable periodic syncing to transmit data to Credeau servers securely.

3. ### Intelligent Data Synchronization
   - Once syncing is enabled, anonymized device data is automatically sent every 8 hours.

   #### Advanced Features
   - **Fraud Detection:** Identify risky behavior using device-level intelligence in near real time.
   - **On-Demand Sync:** Trigger data syncs manually to fetch the most recent behavioral signals — even when the app is inactive.

4. ### Real-Time Decisioning via Insights API
   - Leverage the **Insights API** to retrieve processed data and actionable insights.
   - Integrate insights into your models for:
     - Credit underwriting
     - Fraud risk checks
     - Customer segmentation & personalization
