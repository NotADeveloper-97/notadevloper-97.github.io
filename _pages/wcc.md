---
layout: page-w-banner
title: World Crypto Con
bannerTitle: World Crypto Con Hackathon
permalink: /wcc/
---

<style>
  .rvn-wcc-doc {
    font-family: 'Inter', sans-serif;
    color: #111827;
    max-width: 900px;
    margin: 0 auto;
    padding: 60px 24px;
  }
  .rvn-wcc-doc h2, .rvn-wcc-doc h3 {
    font-family: 'Space Grotesk', sans-serif;
    color: #090B11;
  }
  .rvn-wcc-doc h2 { font-size: 28px; margin-top: 48px; border-bottom: 2px solid rgba(59, 82, 198, 0.08); padding-bottom: 8px; }
  .rvn-wcc-doc h2:first-of-type { margin-top: 0; }
  .rvn-wcc-doc h3 { font-size: 18px; line-height: 1.5; color: #4B5563; font-weight: 400; }
  .rvn-wcc-doc h3 p { margin-top: 12px; color: #FF5A1F; font-weight: 600; }
  
  .rvn-wcc-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(260px, 1fr));
    gap: 16px;
    margin-top: 20px;
  }
  .rvn-wcc-link-card {
    background: #FFFFFF;
    border: 1px solid rgba(17, 24, 39, 0.05);
    border-radius: 12px;
    padding: 16px 20px;
    font-weight: 600;
    color: #3B52C6;
    text-decoration: none;
    box-shadow: 0 2px 4px rgba(0,0,0,0.01);
    transition: all 0.2s ease;
  }
  .rvn-wcc-link-card:hover {
    border-color: #FF5A1F;
    color: #FF5A1F;
    transform: translateY(-2px);
  }

  .rvn-wcc-ol {
    list-style: none;
    padding: 0;
    margin: 24px 0;
  }
  .rvn-wcc-ol > li {
    background: #FAFBFC;
    border: 1px solid #ECEEF1;
    border-radius: 16px;
    padding: 24px;
    margin-bottom: 20px;
  }
  .rvn-wcc-ol strong {
    font-family: 'Space Grotesk', sans-serif;
    display: block;
    font-size: 16px;
    color: #090B11;
    margin-bottom: 8px;
  }
  .rvn-wcc-ol ul {
    margin-top: 12px;
    padding-left: 20px;
  }
  .rvn-wcc-ol li ul li {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 13px;
    color: #3B52C6;
    margin-bottom: 4px;
  }
</style>

<div class="rvn-wcc-doc">
  <h2>What is Ravencoin?</h2>
  <h3>
    Ravencoin is a protocol based on a fork of the Bitcoin code which adds features specifically focused on allowing tokens to be issued on the Ravencoin blockchain[cite: 16]. These tokens can have whatever properties the issuer of the token decides - so they can be limited in quantity, named and be issued as securities or as collectibles[cite: 16].
    <p>Make your own security token within minutes and have it trade worldwide[cite: 16].</p>
  </h3>

  <h2>Hackathon Development References</h2>
  <div class="rvn-wcc-grid">
    <a class="rvn-wcc-link-card" href="https://github.com/RavenProject/Ravencoin" target="_blank">Public GitHub Project</a>
    <a class="rvn-wcc-link-card" href="https://raven-nightly-builds.ravencoin.org" target="_blank">Download Core Daemon / Qt</a>
    <a class="rvn-wcc-link-card" href="https://github.com/RavenDevKit/insight-api" target="_blank">Insight API Documentation</a>
    <a class="rvn-wcc-link-card" href="https://testnet.ravencoin.network/" target="_blank">Testnet Faucet Node</a>
    <a class="rvn-wcc-link-card" href="https://testnet-api.ravencoin.org/api/" target="_blank">Testnet REST API Endpoint</a>
    <a class="rvn-wcc-link-card" href="https://testnet-api.ravencoin.org/" target="_blank">Testnet Block Explorer</a>
    <a class="rvn-wcc-link-card" href="https://github.com/underdarkskies/ravencore-lib" target="_blank">JavaScript Core Library</a>
    <a class="rvn-wcc-link-card" href="https://github.com/standard-error/python-ravencoinlib" target="_blank">Python Library Asset Engine</a>
    <a class="rvn-wcc-link-card" href="https://github.com/JonPizza/ravenrpc" target="_blank">Secondary Python RPC Wrapper</a>
  </div>

  <h2>Environment Compilation Guidelines</h2>
  <div class="rvn-wcc-grid">
    <a class="rvn-wcc-link-card" href="https://github.com/RavenProject/Ravencoin/blob/master/doc/build-osx.md" target="_blank">macOS Build Environment Setups</a>
    <a class="rvn-wcc-link-card" href="https://github.com/RavenProject/Ravencoin/blob/master/doc/build-unix.md" target="_blank">Unix / Linux Compilation Matrix</a>
  </div>

  <h2>How to use Testnet Snapshot Data?</h2>
  <h3>To accelerate regional nodes, download the pre-synchronized chain dataset directly from the WCC folder repositories[cite: 16]:</h3>
  
  <ol class="rvn-wcc-ol">
    <li>
      <strong>Step 1: Extract block structures directly into target system data paths:</strong>
      <ul>
        <li>macOS Platform Target — ~/Library/Application Support/Raven/testnet7</li>
        <li>Linux OS Target Ecosystem — ~/.raven/testnet7</li>
        <li>Windows Workspace Target Path — $(User)/AppData/Roaming/Raven/testnet7</li>
      </ul>
    </li>
    <li>
      <strong>Step 2: Place the base configurations (<code>ravencoin.conf</code>) one tier above the testnet folder root:</strong>
      <ul>
        <li>macOS Execution Target — ~/Library/Application Support/Raven</li>
        <li>Linux Execution Target Systems — ~/.raven</li>
        <li>Windows Execution File Structures — $(User)/AppData/Roaming/Raven</li>
      </ul>
    </li>
  </ol>

  <h2>How to claim testing coins from the Faucet?</h2>
  <h3>Provide your address target within the <a href="https://testnet.ravencoin.network/" target="_blank" style="color:#3B52C6; font-weight:600;">Testnet Faucet Portal</a> to instantly distribute diagnostic assets[cite: 16].</h3>
</div>