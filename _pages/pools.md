---
layout: page-w-banner
title: Pools
bannerTitle: Mining Pools
bannerImage: /assets/img/pages/exchanges/exchange-banner.jpg
permalink: /pools/
---

<style>
  /* ---------------------------------------------------
      Modern Refined Web3 Design System Tokens
  --------------------------------------------------- */
  .rvn-pool-container {
    --bg-dark: #090B11;
    --bg-card-dark: #121624;
    --bg-light: #F8F9FA;
    --bg-card-light: #FFFFFF;
    --brand-ember: #FF5A1F;
    --brand-ember-hover: #E04810;
    --brand-navy: #3B52C6;
    --text-primary-dark: #FFFFFF;
    --text-secondary-dark: #94A3B8;
    --text-primary-light: #111827;
    --text-secondary-light: #4B5563;
    --border-dark: rgba(255, 255, 255, 0.08);
    --border-light: rgba(17, 24, 39, 0.05);

    font-family: 'Inter', sans-serif;
    color: var(--text-primary-light);
    max-width: 1200px;
    margin: 0 auto;
    padding: 60px 24px;
  }

  .rvn-pool-container h2 {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 32px;
    font-weight: 700;
    margin-bottom: 16px;
    color: var(--text-primary-light);
  }

  .rvn-pool-container h3 {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 26px;
    font-weight: 700;
    margin-top: 64px;
    margin-bottom: 20px;
    border-left: 4px solid var(--brand-navy);
    padding-left: 14px;
    color: var(--text-primary-light);
  }

  .rvn-pool-container p {
    line-height: 1.6;
    color: var(--text-secondary-light);
    font-size: 16px;
  }

  /* ---------- Grid Architecture ---------- */
  .pool-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(240px, 1fr));
    gap: 16px;
    margin-top: 28px;
  }

  .pool-card {
    position: relative;
    display: flex;
    align-items: center;
    gap: 14px;
    background: #FFFFFF;
    border: 1px solid var(--border-light);
    border-radius: 14px;
    padding: 16px 18px;
    text-decoration: none;
    color: inherit;
    transition: transform 0.18s ease, box-shadow 0.18s ease, border-color 0.18s ease;
  }

  .pool-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 14px 26px -10px rgba(15, 23, 42, 0.14);
    border-color: rgba(255, 90, 31, 0.25);
    color: inherit;
    text-decoration: none;
  }

  .pool-logo-frame {
    flex: 0 0 44px;
    width: 44px;
    height: 44px;
    border-radius: 11px;
    background: #FAFBFC;
    border: 1px solid #ECEEF1;
    display: flex;
    align-items: center;
    justify-content: center;
    overflow: hidden;
  }

  .pool-logo-frame i {
    font-size: 20px;
    color: var(--brand-navy);
  }

  .pool-logo-frame img {
    width: 100%;
    height: 100%;
    object-fit: contain;
    padding: 6px;
  }

  .pool-meta-block { 
    min-width: 0; 
  }

  .pool-name {
    font-weight: 600;
    font-size: 14.5px;
    color: var(--text-primary-light);
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    display: block;
  }

  .pool-badge {
    display: inline-block;
    margin-top: 3px;
    font-size: 10px;
    font-weight: 700;
    letter-spacing: 0.04em;
    text-transform: uppercase;
    color: var(--brand-ember);
    background: rgba(255, 90, 31, 0.08);
    border: 1px solid rgba(255, 90, 31, 0.18);
    border-radius: 5px;
    padding: 2px 6px;
  }

  .pool-badge-platform {
    color: var(--brand-navy);
    background: rgba(59, 82, 198, 0.08);
    border: 1px solid rgba(59, 82, 198, 0.18);
  }

  .pool-badge-top {
    color: #FFFFFF;
    background: var(--brand-ember);
    border: 1px solid var(--brand-ember);
  }
</style>

<div class="rvn-pool-container">
  <h2>How can I mine Ravencoin?</h2>
  <p>Designed to be mined on readily available consumer-grade hardware, Ravencoin uses a proof-of-work mining algorithm known as KAWPOW. It’s custom-tailored to be Application Specific Integrated Circuit (ASIC) resistant and is highly efficient on consumer GPU hardware memory profiles.</p>
  <p>To start mining RVN, you will first need to create a wallet and generate a public receiving address that your block payouts can be routed into. Next, connect your hardware config to a verified mining pool.</p>
  <p>To learn the detailed setup commands, visit: <a href="https://raven.wiki/wiki/Mining" target="_blank" rel="noopener" style="color: var(--brand-ember); font-weight: 600; text-decoration: none;">Official Mining Wiki Integration Guide →</a></p>
  
  <h3>Verified Mining Pools (Sorted by Top Network Hashrate)</h3>
  <p>The top operational mining pools hosting the vast majority of Ravencoin's global network hashrate distribution, stripped of dead links and inactive servers:</p>
  
  <div class="pool-grid">
    <!-- 1. 2Miners -->
    <a class="pool-card" href="https://2miners.com/rvn-mining-pool" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><i class="zmdi zmdi-layers"></i></span>
      <span class="pool-meta-block">
        <span class="pool-name">2Miners</span>
        <span class="pool-badge pool-badge-top">#1 Top Hashrate</span>
      </span>
    </a>

    <!-- 2. HeroMiners -->
    <a class="pool-card" href="https://ravencoin.herominers.com/" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><i class="zmdi zmdi-layers"></i></span>
      <span class="pool-meta-block">
        <span class="pool-name">HeroMiners</span>
        <span class="pool-badge pool-badge-top">#2 High Volume</span>
      </span>
    </a>

    <!-- 3. K1Pool -->
    <a class="pool-card" href="https://k1pool.com/pool/rvn" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><i class="zmdi zmdi-layers"></i></span>
      <span class="pool-meta-block">
        <span class="pool-name">K1Pool</span>
        <span class="pool-badge">Dual RVN + ZIL</span>
      </span>
    </a>

    <!-- 4. WoolyPooly -->
    <a class="pool-card" href="https://woolypooly.com/en/coin/rvn" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><i class="zmdi zmdi-layers"></i></span>
      <span class="pool-meta-block">
        <span class="pool-name">WoolyPooly</span>
        <span class="pool-badge">Stable Hash</span>
      </span>
    </a>

    <!-- 5. Cruxpool -->
    <a class="pool-card" href="https://www.cruxpool.com/rvn" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><i class="zmdi zmdi-layers"></i></span>
      <span class="pool-meta-block">
        <span class="pool-name">Cruxpool</span>
        <span class="pool-badge">Low Latency</span>
      </span>
    </a>

    <!-- 6. CoinMinerz -->
    <a class="pool-card" href="https://coinminerz.com/" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><i class="zmdi zmdi-layers"></i></span>
      <span class="pool-meta-block">
        <span class="pool-name">CoinMinerz</span>
        <span class="pool-badge">Active Pool</span>
      </span>
    </a>

    <!-- 7. Blocksmith -->
    <a class="pool-card" href="https://rvn.bsmith.io/" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><i class="zmdi zmdi-layers"></i></span>
      <span class="pool-meta-block">
        <span class="pool-name">Blocksmith</span>
        <span class="pool-badge">Community Pool</span>
      </span>
    </a>
  </div>

  <h3>Automated Mining &amp; Management Platforms</h3>
  <p>While these are not traditional raw mining pools, you can easily use these verified optimization platforms to mine Ravencoin with zero manual batch script configurations.</p>
  <p>Most of the time you don't have to download standalone third-party miner miners or update execution kernels yourself—these platforms include managed mining engines embedded inside their unified client interfaces.</p>

  <div class="pool-grid">
    <a class="pool-card" href="https://www.nicehash.com/" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><img src="/assets/img/pages/pools/nicehash.png" alt="NiceHash"></span>
      <span class="pool-meta-block">
        <span class="pool-name">NiceHash</span>
        <span class="pool-badge pool-badge-platform">Hash Market</span>
      </span>
    </a>

    <a class="pool-card" href="https://www.kryptex.com/" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><img src="/assets/img/pages/pools/kryptex.png" alt="Kryptex"></span>
      <span class="pool-meta-block">
        <span class="pool-name">Kryptex</span>
        <span class="pool-badge pool-badge-platform">1-Click Miner</span>
      </span>
    </a>

    <a class="pool-card" href="https://unmineable.com/" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><img src="/assets/img/pages/pools/unmineable.png" alt="Unmineable"></span>
      <span class="pool-meta-block">
        <span class="pool-name">Unmineable</span>
        <span class="pool-badge pool-badge-platform">Multi-Asset Swap</span>
      </span>
    </a>

    <a class="pool-card" href="https://hiveon.com/os/" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><img src="/assets/img/pages/pools/hiveos.png" alt="HiveOS"></span>
      <span class="pool-meta-block">
        <span class="pool-name">HiveOS</span>
        <span class="pool-badge pool-badge-platform">Rig Management</span>
      </span>
    </a>

    <a class="pool-card" href="https://minerstat.com/" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><img src="/assets/img/pages/pools/minerstat.png" alt="Minerstat"></span>
      <span class="pool-meta-block">
        <span class="pool-name">Minerstat</span>
        <span class="pool-badge pool-badge-platform">OS &amp; Analytics</span>
      </span>
    </a>

    <a class="pool-card" href="https://www.betterhash.net/" target="_blank" rel="noopener nofollow">
      <span class="pool-logo-frame"><img src="/assets/img/pages/pools/betterhash.png" alt="BetterHash"></span>
      <span class="pool-meta-block">
        <span class="pool-name">BetterHash</span>
        <span class="pool-badge pool-badge-platform">Smart Miner</span>
      </span>
    </a>
  </div>

</div>