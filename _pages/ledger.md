---
layout: page-w-banner
title: Ledger
bannerTitle: Using Ledger Nano
bannerImage: /assets/img/pages/wallet/wallet-banner.jpg
permalink: /ledger/
---

<style>
  .rvn-ledger-container {
    font-family: 'Inter', sans-serif;
    color: #111827;
    max-width: 850px;
    margin: 0 auto;
    padding: 60px 24px;
  }
  .rvn-ledger-container h2, .rvn-ledger-container h3 {
    font-family: 'Space Grotesk', sans-serif;
    color: #090B11;
  }
  .rvn-ledger-container h2 { font-size: 32px; border-bottom: 2px solid #ECEEF1; padding-bottom: 8px; margin-bottom: 28px; }
  .rvn-ledger-container h3 { font-size: 22px; margin-top: 40px; color: #3B52C6; }
  .rvn-ledger-container p { line-height: 1.6; color: #4B5563; }
  
  .rvn-step-list {
    list-style: none;
    padding: 0;
    margin: 24px 0;
  }
  .rvn-step-list li {
    position: relative;
    padding-left: 48px;
    margin-bottom: 18px;
    line-height: 1.6;
    color: #4B5563;
  }
  .rvn-step-list li::before {
    content: "✓";
    position: absolute;
    left: 0;
    top: 2px;
    width: 24px;
    height: 24px;
    background: rgba(255, 90, 31, 0.1);
    color: #FF5A1F;
    border-radius: 50%;
    display: flex;
    align-items: center;
    justify-content: center;
    font-weight: 700;
    font-size: 12px;
  }
  .rvn-kbd {
    font-family: 'IBM Plex Mono', monospace;
    background: #F3F4F6;
    border: 1px solid #E5E7EB;
    border-radius: 4px;
    padding: 2px 6px;
    font-size: 13px;
    color: #1F2937;
  }
</style>

<div class="rvn-ledger-container">
  <h2>How to use Ledger Nano S and Ledger Nano X</h2>
  <p>The Ledger Nano S and Ledger Nano X are hardware wallets designed to securely lock private key access inside offline physical storage elements. Installing the Ravencoin application allows you to monitor and signatures regular transactions safely. <em>Note: Native internal management of Ravencoin custom asset layers is currently unsupported on ledger firmware interfaces at this time.</em></p>

  <h3>Before you begin</h3>
  <ul class="rvn-step-list">
    <li>Download and deploy the official desktop version of <a href="https://support.ledger.com/hc/en-us/articles/360006395553" target="_blank">Ledger Live</a>.</li>
    <li>Initialize and secure your basic Ledger hardware key configuration profile.</li>
    <li>Verify that your physical device is running the latest baseline core firmware modules.</li>
    <li>Ensure the official <strong>Bitcoin App</strong> is installed first, as the Ravencoin engine shares base library files.</li>
  </ul>

  <h3>Installing the Ravencoin Ledger Module</h3>
  <ul class="rvn-step-list">
    <li>Connect your physical hardware device via USB and input your custom access PIN.</li>
    <li>Open Ledger Live and navigate directly into the <span class="rvn-kbd">Manager</span> tab menu interface.</li>
    <li>Confirm and allow device connection permissions on your hardware screen if requested.</li>
    <li>Locate the Ravencoin entry listing within the App Catalog selection tree.</li>
    <li>Click <span class="rvn-kbd">Install</span>. If an error block requests dependency profiles, update your Bitcoin client application framework first.</li>
  </ul>

  <h3>Setting Up Electrum-Ravencoin</h3>
  <p>To orchestrate external transfers alongside cold-storage device protections, download the specialized desktop utility suite: <a href="https://github.com/Electrum-RVN-SIG/electrum-ravencoin" target="_blank" style="font-weight:600; color:#FF5A1F;">Electrum-Ravencoin Wallet Client →</a></p>

  <ul class="rvn-step-list">
    <li>Attach your Ledger device, enter your lock PIN, and access the native on-device <span class="rvn-kbd">Ravencoin</span> dashboard.</li>
    <li>Launch the Electrum-Ravencoin application on your workstation while closing default Ledger Live scripts.</li>
    <li>Select your workspace file path profile name and advance past the wallet profile naming confirmation block.</li>
    <li>When presented with construction parameters, explicitly mark <span class="rvn-kbd">Standard Wallet</span> as your choice.</li>
    <li>On keys source allocation steps, click <span class="rvn-kbd">Use a hardware device</span> and advance.</li>
    <li>Select the scanned hardware identity label: <span class="rvn-kbd">an unnamed ledger [ledger, initialized]</span>.</li>
    <li>Confirm the standard derivation path configurations without manual string overrides.</li>
    <li>Choose whether to encrypt configuration metadata file caches locally on your computer to finish setup.</li>
  </ul>
</div>