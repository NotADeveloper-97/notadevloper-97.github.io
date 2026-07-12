---
layout: page-w-banner
title: Projects
bannerTitle: Ravencoin Projects
bannerImage: /assets/img/pages/exchanges/exchange-banner.jpg
permalink: /projects/
---

<style>
  /* ---------------------------------------------------
      Modern Refined Web3 Design System Tokens
  --------------------------------------------------- */
  .rvn-projects-page {
    --bg-dark: #090B11;
    --bg-card-dark: #121624;
    --bg-light: #F8F9FA;
    --bg-card-light: #FFFFFF;
    --brand-ember: #FF5A1F;
    --brand-ember-hover: #E04810;
    --brand-navy: #3B52C6;
    --text-primary-light: #111827;
    --text-secondary-light: #4B5563;
    --border-light: rgba(17, 24, 39, 0.06);

    font-family: 'Inter', sans-serif;
    color: var(--text-primary-light);
    max-width: 900px;
    margin: 0 auto;
    padding: 60px 24px;
    display: block;
    width: 100%;
    clear: both;
  }

  .rvn-projects-page h2, .rvn-projects-page h3, .rvn-projects-page h4 {
    font-family: 'Space Grotesk', sans-serif;
    color: var(--bg-dark);
  }

  .rvn-projects-page h2 { 
    font-size: 32px; 
    border-bottom: 2px solid rgba(17, 24, 39, 0.05); 
    padding-bottom: 12px; 
    margin-bottom: 24px;
  }

  .rvn-projects-page p { 
    line-height: 1.6; 
    color: var(--text-secondary-light); 
    font-size: 16px;
    margin-bottom: 24px;
  }
  
  /* ---------- Table of Contents ---------- */
  .toc-box {
    background: #FAFBFC;
    border: 1px solid #ECEEF1;
    border-radius: 12px;
    padding: 20px 24px;
    margin: 24px 0 48px;
  }

  .toc-box h4 {
    margin-top: 0; 
    color: var(--bg-dark);
    font-size: 16px;
    margin-bottom: 12px;
  }

  .toc-box ul { 
    display: grid; 
    grid-template-columns: 1fr 1fr; 
    gap: 8px 24px; 
    padding-left: 20px; 
    margin: 0;
  }

  @media(max-width:600px){ 
    .toc-box ul { grid-template-columns: 1fr; } 
  }

  .toc-box a { 
    color: var(--brand-navy); 
    font-weight: 600; 
    text-decoration: none; 
    font-size: 14.5px;
  }

  .toc-box a:hover { 
    color: var(--brand-ember); 
    text-decoration: underline; 
  }

  /* ---------- Project Block Container ---------- */
  .project-block {
    background: #FFFFFF;
    border: 1px solid var(--border-light);
    border-radius: 16px;
    padding: 36px;
    margin-bottom: 32px;
    box-shadow: 0 4px 20px -4px rgba(15, 23, 42, 0.04);
    display: block;
    width: 100%;
    clear: both;
  }

  .project-block h3 { 
    font-size: 24px; 
    margin-top: 0; 
    color: var(--bg-dark); 
    margin-bottom: 14px; 
  }

  .project-block h4 { 
    font-size: 13px; 
    text-transform: uppercase; 
    letter-spacing: 0.05em; 
    color: #94A3B8; 
    margin-top: 24px; 
    margin-bottom: 12px; 
  }
  
  /* ---------- Interactive Target Links ---------- */
  .project-links { 
    list-style: none; 
    padding: 0; 
    display: flex; 
    flex-wrap: wrap; 
    gap: 10px; 
    margin: 0;
  }

  .project-links a {
    display: inline-block;
    background: #FAFBFC;
    border: 1px solid #ECEEF1;
    padding: 10px 18px;
    border-radius: 8px;
    font-size: 14px;
    color: var(--brand-navy);
    font-weight: 600;
    text-decoration: none;
    transition: all 0.15s ease;
  }

  .project-links a:hover {
    background: var(--bg-dark);
    color: #FFFFFF;
    border-color: var(--bg-dark);
  }

  .roadmap-list { 
    padding-left: 20px; 
    color: var(--text-secondary-light); 
    font-family: 'IBM Plex Mono', monospace; 
    font-size: 13.5px; 
    line-height: 1.6;
  }
</style>

<div class="rvn-projects-page">
  <h2>Ecosystem Production Projects</h2>
  <p>These verified core infrastructure suites and utility tools are actively maintained, open-source, and fully functional across the global decentralized Ravencoin layer-1 network.</p>

  <div class="toc-box">
    <h4>Active Projects Directory</h4>
    <ul>
      <li><a href="#ravencoin-core">Ravencoin Core Reference Node</a></li>
      <li><a href="#electrum-ravencoin">Electrum-Ravencoin Client</a></li>
      <li><a href="#moontree-wallet">Moontree Wallet Ecosystem</a></li>
      <li><a href="#cryptoscope-indexer">Cryptoscope Asset Explorer</a></li>
    </ul>
  </div>

  <!-- Project 1: Ravencoin Core -->
  <div class="project-block" id="ravencoin-core">
    <h3>Ravencoin Core Reference Node</h3>
    <p>The base software implementation running full-node ledger capabilities. Orchestrates raw peer connections, consensus checks, block distribution rules, and layer-1 asset token minting primitives natively within the client.</p>
    
    <h4>Core Resources &amp; Channels</h4>
    <div class="project-links">
      <a href="https://github.com/RavenProject/Ravencoin" target="_blank" rel="noopener">GitHub Project Source</a>
      <a href="https://github.com/RavenProject/Ravencoin/releases" target="_blank" rel="noopener">Official Client Release Assets</a>
    </div>

    <h4>Ecosystem Target Matrix</h4>
    <ul class="roadmap-list">
      <li><strong>Consensus Engine:</strong> KAWPOW ASIC Resistant PoW Checkpoint</li>
      <li><strong>Deployment Base:</strong> Bitcoin v0.15.x Protocol Hardfork Suite</li>
    </ul>
  </div>

  <!-- Project 2: Electrum-Ravencoin -->
  <div class="project-block" id="electrum-ravencoin">
    <h3>Electrum-Ravencoin Client</h3>
    <p>The standard lightweight desktop wallet application designed for instant network sync and low resource footprint. Maintained explicitly by the Electrum-RVN-SIG development team to provide secure cold-storage hardware tracking integrations.</p>
    
    <h4>Core Resources &amp; Channels</h4>
    <div class="project-links">
      <a href="https://github.com/Electrum-RVN-SIG/electrum-ravencoin" target="_blank" rel="noopener">GitHub Client Source</a>
      <a href="https://github.com/Electrum-RVN-SIG/electrum-ravencoin/releases" target="_blank" rel="noopener">Download Lightweight Binaries</a>
    </div>

    <h4>Ecosystem Target Matrix</h4>
    <ul class="roadmap-list">
      <li><strong>Hardware Verification:</strong> Ledger Nano S/X &amp; Trezor Support Matrix</li>
      <li><strong>Network Layer:</strong> SSL Stratum Electrum Server Infrastructure</li>
    </ul>
  </div>

  <!-- Project 3: Moontree Wallet -->
  <div class="project-block" id="moontree-wallet">
    <h3>Moontree Wallet Ecosystem</h3>
    <p>A mobile open-source wallet designed exclusively around Ravencoin asset token utility mechanics. Built from the ground up to allow frictionless management of main assets, sub-assets, unique tokens, and native IPFS metadata visualization logs.</p>
    
    <h4>Core Resources &amp; Channels</h4>
    <div class="project-links">
      <a href="https://moontree.com/" target="_blank" rel="noopener nofollow">Moontree Project Space</a>
      <a href="https://github.com/moontreewallet" target="_blank" rel="noopener">Open Source Repository</a>
    </div>

    <h4>Ecosystem Target Matrix</h4>
    <ul class="roadmap-list">
      <li><strong>Asset Capabilities:</strong> Send, Receive, and Inspect Layer-1 Unique Tokens</li>
      <li><strong>Storage Profile:</strong> Non-Custodial Mobile Seed Phrase Execution</li>
    </ul>
  </div>

  <!-- Project 4: Cryptoscope -->
  <div class="project-block" id="cryptoscope-indexer">
    <h3>Cryptoscope Asset Explorer</h3>
    <p>A highly reliable block indexing matrix and public database interface built to map network metrics. Features exhaustive tracking logs specifically tailored to asset creation data fields, null address parameter checks, and verifier script metadata records.</p>
    
    <h4>Core Resources &amp; Channels</h4>
    <div class="project-links">
      <a href="https://rvn.cryptoscope.io/" target="_blank" rel="noopener nofollow">Mainnet Chain Explorer</a>
      <a href="https://rvnt.cryptoscope.io/" target="_blank" rel="noopener nofollow">Testnet Chain Explorer</a>
    </div>

    <h4>Ecosystem Target Matrix</h4>
    <ul class="roadmap-list">
      <li><strong>Indexer Features:</strong> Real-Time Block Metrics &amp; Transaction Parsing Logs</li>
      <li><strong>API Infrastructure:</strong> Public JSON-RPC Endpoint Access Pools</li>
    </ul>
  </div>

</div>