<!-- <link rel="stylesheet" href="assets/css/style.css" />

<div class="container">
  <div class="sidebar">
    <h2>Sidebar</h2>
    <ul>
      <li><a href="index.html">Home</a></li>
      <li><a href="page2.html">Page 2</a></li>
      <li><a href="page3.html">Page 3</a></li>
    </ul>
  </div>

  <div class="content">
    <h1>Hello, GitHub Pages!</h1>
    <p>This is my homepage with a left-aligned sidebar layout.</p>
  </div>
</div> -->

---
home: true
heroImage: logo.svg
footer: Copyright © 2023 Moshpit Technologies Pvt. Ltd.
---
<style>
.home .feature {
  flex-basis: 45% !important;
  max-width: 45% !important;
}
@media (max-width: 719px){
  .home .feature {
    max-width: 100% !important;
    padding: 0 2.5rem !important;
  }
}

.home .doc_link:hover {
    border-bottom-width: 10px;
    border-bottom-style: solid;
    padding-bottom: 3px;
}

</style>
<div class="features">
  <div class="feature">
    <h2>DeviceConnect</h2>
    <p>
      Lets businesses get access to enriched Android mobile device data of customers to build lending and wealth management apps.
    </p>
    <p>
      <a href="device-connect/" class="doc_link">See Documentation →</a>
    </p>
  </div>
  <div class="feature">
    <h2>BankConnect</h2>
    <p>
      Lets businesses get access to enriched transaction data of customers using bank statements uploaded manually or via Net Banking.
    </p>
    <p>
      <a href="session-flow/" class="doc_link">See Documentation →</a>
    </p>
  </div>
</div>
