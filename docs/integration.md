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
      <li><a href="introduction.html">Introduction</a></li>
      <li><a href="gettingstarted.html">Getting Started</a></li>
      <li><a href="integration.html">Integration</a></li>
    </ul>

  </div>

 <div class="content">
    <h1 style="color: #f7931e;">DeviceConnect: Integration Flow</h1>
    <p>Follow the steps below to securely collect device intelligence and access real-time insights via FinBox.</p>

    <h2 style="margin-top: 30px; color: #f7931e;">DeviceConnect SDK Integration Summary:</h2>

    <ol>
      <li>
        <h3>User Permissions & Consent</h3>
        <ul>
          <li>Request user permissions to enable anonymized device data collection.</li>
          <li>Ensure compliance with all applicable privacy laws and regulatory guidelines.</li>
          <li>Clearly communicate the purpose of data collection to foster user trust.</li>
        </ul>
      </li>

      <li>
        <h3>SDK Initialization & User Creation</h3>
        <ul>
          <li>Initialize the SDK early in the app’s lifecycle (e.g., splash screen or main activity).</li>
          <li>Assign a unique, custom-generated user hash. <strong>Do not use or store PII.</strong></li>
          <li>Enable periodic syncing to transmit data to FinBox servers securely.</li>
        </ul>
      </li>

      <li>
        <h3>Intelligent Data Synchronization</h3>
        <ul>
          <li>Once syncing is enabled, anonymized device data is automatically sent every 8 hours.</li>
        </ul>

        <h4>Advanced Features</h4>
        <ul>
          <li><strong>Fraud Detection:</strong> Identify risky behavior using device-level intelligence in near real time.</li>
          <li><strong>On-Demand Sync:</strong> Trigger data syncs manually to fetch the most recent behavioral signals — even when the app is inactive.</li>
        </ul>
      </li>

      <li>
        <h3>Real-Time Decisioning via Insights API</h3>
        <ul>
          <li>Leverage the <strong>Insights API</strong> to retrieve processed data and actionable insights.</li>
          <li>Integrate insights into your models for:</li>
          <ul>
            <li>Credit underwriting</li>
            <li>Fraud risk checks</li>
            <li>Customer segmentation & personalization</li>
          </ul>
        </ul>
      </li>
    </ol>
  </div>
</div>

</div>
