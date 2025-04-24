# Gator SDK Integration

This SDK provides device data collection and synchronization capabilities, including support for background sync, device matching, and selective data collection.

## 📦 Installation

Ensure the SDK is added as a dependency in your native Android project. If using React Native, wrap the native module and use it via JS bridge.

---

## ⚙️ SDK Initialization

### Java (Native SDK)
```java
DeviceDataManager dataMgr = new DeviceDataManager(
    context,
    "gator_portal",
    "89c0cbf8-1152-484a-91e7-849ec341175a",
    "https://devdevicesense.credeau.com/api"
);
