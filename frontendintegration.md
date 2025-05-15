<link rel="stylesheet" href="assets/css/style.css" />

<div class="header">
  <img src="assets/images/credeaulogo.png" alt="Credeau Logo" class="logo" />
  <h1 class="title">Credeau Docs</h1>
</div>

<div class="layout"> 
  <div class="sidebar">
    <h2>Overview</h2>
    <ul>
      <li><a href="introduction.html">Introduction</a></li>
      <li><a href="gettingstarted.html">Getting Started</a></li>
      <li><a href="integration.html">Integration</a></li>
    </ul>
     <h2>Data Collection</h2>
    <ul>
      <li><a href="frontendintegration.html">Frontend Integration</a></li>
    </ul>
</div>
</div>

<div class="content">
  <h1 style="color: #f7931e;">DeviceConnect SDK: Frontend Integration Flow</h1>
  <p>
    DeviceConnect empowers businesses with real-time, anonymized intelligence derived directly from mobile devices. It ensures smarter, faster, and more privacy-conscious decision-making through a streamlined SDK integration. Below are the key steps to integrate DeviceConnect in your Android app.
  </p>

  <h2 style="margin-top: 30px; color: #f7931e;">Step-by-Step Integration Guide</h2>

  <h3 style="margin-top: 20px;">Step 1: Request Runtime Permissions</h3>
  <ul>
    <li>Display a consent screen to inform users about the permissions being requested and why they matter.</li>
    <li>Refer to the <strong>Handle Permissions</strong> section for a comprehensive list of required permissions.</li>
    <li>Use the <code>remove</code> node marker to exclude any permission not required for your use case.</li>
  </ul>

  <h3 style="margin-top: 20px;">Step 2: Create a Unique User</h3>
  <ul>
    <li>After permission handling, invoke <code>createUser</code> with a unique <code>CUSTOMER_ID</code>.</li>
    <li>This ID acts as a pseudonymized identifier — avoid using phone numbers, emails, or other personal data.</li>
    <li><code>createUser</code> also validates API credentials to ensure your integration is authorized before proceeding.</li>
    <li>Always call <code>createUser</code> even if some permissions are denied — the SDK syncs only what is available.</li>
  </ul>

  <h3 style="margin-top: 20px;">Step 3: Start Data Synchronization</h3>
  <ul>
    <li>Upon successful <code>createUser</code> response, call <code>startPeriodicSync</code> to begin data collection.</li>
    <li>The SDK continues syncing in the background as per the defined frequency and updates when new permissions are granted.</li>
    <li>Call these functions every time the app opens to ensure continuous background sync and permission adaptation.</li>
  </ul>

  <h2 style="margin-top: 30px; color: #f7931e;">Best Practices & Recommendations</h2>
  <ul>
    <li><strong>Multi-Process Apps:</strong> Ensure manual SDK initialization before invoking <code>createUser</code>.</li>
    <li><strong>Push Notifications:</strong> Forward all notifications to the SDK to avoid background process interruptions. See <em>Forward Notifications to SDK</em>.</li>
  </ul>

  <h2 style="margin-top: 30px; color: #f7931e;">Get Started Today</h2>
  <p>
    Power your fintech platform with anonymized, real-time intelligence from DeviceConnect. Quick to integrate, privacy-respecting by design, and built for scale — DeviceConnect is your gateway to better credit outcomes.
  </p>
</div>

