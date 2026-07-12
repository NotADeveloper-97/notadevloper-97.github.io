---
layout: page-w-banner
title: Community
bannerTitle: Community Resources
bannerImage: /assets/img/pages/community/community-banner.jpg
permalink: /community/
---

<style>
  /* ---------------------------------------------------
      Modern Refined Web3 Design System Tokens
  --------------------------------------------------- */
  .rvn-comm-wrap {
    font-family: 'Inter', sans-serif;
    max-width: 1200px;
    margin: 0 auto;
    padding: 60px 24px;
  }
  
  .rvn-comm-head {
    text-align: center;
    max-width: 700px;
    margin: 0 auto 56px auto;
  }

  .rvn-comm-head h2 {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 36px;
    font-weight: 700;
    color: #090B11;
    margin-bottom: 14px;
    letter-spacing: -0.02em;
  }

  .rvn-comm-head p.subtitle {
    color: #4B5563;
    font-size: 17px;
    line-height: 1.6;
    margin: 0;
  }

  .rvn-section-title {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 22px;
    font-weight: 700;
    color: #090B11;
    margin: 48px 0 24px 0;
    border-left: 4px solid #3B52C6;
    padding-left: 12px;
  }

  /* ---------- Modern Multi-Color Grid ---------- */
  .comm-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(280px, 1fr));
    gap: 20px;
    margin-bottom: 40px;
  }

  .comm-card {
    background: #FFFFFF;
    border: 1px solid rgba(17, 24, 39, 0.05);
    border-radius: 16px;
    padding: 24px;
    text-decoration: none;
    color: inherit;
    display: flex;
    align-items: center;
    gap: 16px;
    transition: transform 0.2s cubic-bezier(0.16, 1, 0.3, 1), box-shadow 0.2s ease, border-color 0.2s ease;
    box-shadow: 0 4px 12px -2px rgba(15, 23, 42, 0.03);
  }

  .comm-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 16px 28px -8px rgba(15, 23, 42, 0.1);
    text-decoration: none;
    color: inherit;
  }

  /* Dynamic Multi-Color Icon Badge Architecture */
  .comm-icon-box {
    flex: 0 0 52px;
    width: 52px;
    height: 52px;
    border-radius: 12px;
    display: flex;
    align-items: center;
    justify-content: center;
    font-size: 24px;
    transition: all 0.2s ease;
  }

  /* Default Faint States matching brand colors */
  .c-btc    { background: rgba(255, 153, 0, 0.08);   color: #FF9900; }
  .c-x      { background: rgba(9, 11, 17, 0.06);     color: #090B11; }
  .c-dis    { background: rgba(88, 101, 242, 0.08);  color: #5865F2; }
  .c-tg     { background: rgba(38, 165, 228, 0.08);  color: #26A5E4; }
  .c-rd     { background: rgba(255, 69, 0, 0.08);    color: #FF4500; }
  .c-git    { background: rgba(36, 41, 46, 0.08);    color: #24292E; }
  .c-wiki   { background: rgba(51, 51, 51, 0.08);    color: #333333; }
  .c-med    { background: rgba(0, 0, 0, 0.06);       color: #000000; }
  .c-tool   { background: rgba(59, 82, 198, 0.08);   color: #3B52C6; }

  /* Premium Full-Color Solid Hover Activations */
  .comm-card:hover .c-btc  { background: #FF9900; color: #FFFFFF; }
  .comm-card:hover .c-x    { background: #090B11; color: #FFFFFF; }
  .comm-card:hover .c-dis  { background: #5865F2; color: #FFFFFF; }
  .comm-card:hover .c-tg   { background: #26A5E4; color: #FFFFFF; }
  .comm-card:hover .c-rd   { background: #FF4500; color: #FFFFFF; }
  .comm-card:hover .c-git  { background: #24292E; color: #FFFFFF; }
  .comm-card:hover .c-wiki { background: #333333; color: #FFFFFF; }
  .comm-card:hover .c-med  { background: #000000; color: #FFFFFF; }
  .comm-card:hover .c-tool { background: #3B52C6; color: #FFFFFF; }

  .comm-meta-block {
    min-width: 0;
  }

  .comm-name {
    font-weight: 600;
    font-size: 15px;
    color: #090B11;
    display: block;
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
  }

  .comm-badge {
    display: inline-block;
    margin-top: 3px;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 10px;
    font-weight: 600;
    color: #6B7280;
    text-transform: uppercase;
    letter-spacing: 0.02em;
  }

  .comm-card:hover .comm-name {
    color: #3B52C6;
  }
</style>

<div class="rvn-comm-wrap">
  
  <div class="rvn-comm-head">
    <h2>Get involved with the Ravencoin community today!</h2>
    <p class="subtitle">We have a number of active and growing communities for you to choose from[cite: 6]:</p>
  </div>

  <!-- ============ PRIMARY SOCIAL HUBS ============ -->
  <div class="rvn-section-title">Primary Communication Hubs</div>
  <div class="comm-grid">
    <!-- Bitcoin Talk -->
    <a class="comm-card" href="https://bitcointalk.org/index.php?topic=3238497" target="_blank" rel="noopener">
      <span class="comm-icon-box c-btc"><i class="zmdi zmdi-comments"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Bitcoin Talk</span>
        <span class="comm-badge">Official Forum Thread[cite: 6]</span>
      </span>
    </a>

    <!-- Twitter -->
    <a class="comm-card" href="https://twitter.com/ravencoin" target="_blank" rel="noopener">
      <span class="comm-icon-box c-x"><i class="zmdi zmdi-twitter"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Official X / Twitter</span>
        <span class="comm-badge">Ecosystem Feed[cite: 6]</span>
      </span>
    </a>

    <!-- Telegram -->
    <a class="comm-card" href="https://t.me/RavencoinDev" target="_blank" rel="noopener">
      <span class="comm-icon-box c-tg"><i class="zmdi zmdi-whatsapp"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Telegram Chat</span>
        <span class="comm-badge">Ecosystem Dev Channel[cite: 6]</span>
      </span>
    </a>

    <!-- Github -->
    <a class="comm-card" href="https://github.com/RavenProject/Ravencoin" target="_blank" rel="noopener">
      <span class="comm-icon-box c-git"><i class="zmdi zmdi-github-alt"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">GitHub Repository</span>
        <span class="comm-badge">Open Source Code[cite: 6]</span>
      </span>
    </a>

    <!-- Wiki -->
    <a class="comm-card" href="https://raven.wiki/wiki/Ravencoin_Wiki" target="_blank" rel="noopener">
      <span class="comm-icon-box c-wiki"><i class="zmdi zmdi-wikipedia"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Ecosystem Wiki</span>
        <span class="comm-badge">Knowledge Base[cite: 6]</span>
      </span>
    </a>
  </div>

  <!-- ============ DISCORD SERVERS ============ -->
  <div class="rvn-section-title">Community Discord Guilds</div>
  <div class="comm-grid">
    <!-- Discord 1 -->
    <a class="comm-card" href="https://discord.gg/jn6uhur" target="_blank" rel="noopener">
      <span class="comm-icon-box c-dis"><i class="zmdi zmdi-input-antenna"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Ravencoin Community</span>
        <span class="comm-badge">Main Discord Server[cite: 6]</span>
      </span>
    </a>

    <!-- Discord 2 -->
    <a class="comm-card" href="https://discord.gg/uh6PrWh" target="_blank" rel="noopener">
      <span class="comm-icon-box c-dis"><i class="zmdi zmdi-accounts"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Discord - Raven</span>
        <span class="comm-badge">Developer Focus Room[cite: 6]</span>
      </span>
    </a>

    <!-- Discord 3 -->
    <a class="comm-card" href="https://discord.gg/fVymYST" target="_blank" rel="noopener">
      <span class="comm-icon-box c-dis"><i class="zmdi zmdi-coffee"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Ecosystem Lounge</span>
        <span class="comm-badge">RVN Trader &amp; Miner Chat[cite: 6]</span>
      </span>
    </a>
  </div>

  <!-- ============ REDDIT COMMUNITIES ============ -->
  <div class="rvn-section-title">Subreddit Forums</div>
  <div class="comm-grid">
    <!-- Reddit 1 -->
    <a class="comm-card" href="https://www.reddit.com/r/Ravencoin/" target="_blank" rel="noopener">
      <span class="comm-icon-box c-rd"><i class="zmdi zmdi-reddit"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">r/Ravencoin</span>
        <span class="comm-badge">Main Subreddit[cite: 6]</span>
      </span>
    </a>

    <!-- Reddit 2 -->
    <a class="comm-card" href="https://www.reddit.com/r/rvn/" target="_blank" rel="noopener">
      <span class="comm-icon-box c-rd"><i class="zmdi zmdi-trending-up"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">r/rvn</span>
        <span class="comm-badge">Discussion Arena[cite: 6]</span>
      </span>
    </a>

    <!-- Reddit 3 -->
    <a class="comm-card" href="https://www.reddit.com/r/RVNMiner/" target="_blank" rel="noopener">
      <span class="comm-icon-box c-rd"><i class="zmdi zmdi-settings"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">r/RVNMiner</span>
        <span class="comm-badge">Hardware &amp; Setup Feed[cite: 6]</span>
      </span>
    </a>

    <!-- Reddit 4 -->
    <a class="comm-card" href="https://www.reddit.com/r/RVNCoin/" target="_blank" rel="noopener">
      <span class="comm-icon-box c-rd"><i class="zmdi zmdi-assignment"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">r/RVNCoin</span>
        <span class="comm-badge">Ecosystem Updates[cite: 6]</span>
      </span>
    </a>

    <!-- Reddit 5 -->
    <a class="comm-card" href="https://www.reddit.com/r/ravencointrader/" target="_blank" rel="noopener">
      <span class="comm-icon-box c-rd"><i class="zmdi zmdi-chart-donut"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">r/ravencointrader</span>
        <span class="comm-badge">Market Dynamics Feed[cite: 6]</span>
      </span>
    </a>
  </div>

  <!-- ============ BLOGS & DEV LOGS ============ -->
  <div class="rvn-section-title">Ecosystem Blog publications</div>
  <div class="comm-grid">
    <!-- Medium 1 -->
    <a class="comm-card" href="https://medium.com/@ravencoin" target="_blank" rel="noopener">
      <span class="comm-icon-box c-med"><i class="zmdi zmdi-file-text"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Ravencoin Medium</span>
        <span class="comm-badge">Core Foundation Blog[cite: 6]</span>
      </span>
    </a>

    <!-- Medium 2 -->
    <a class="comm-card" href="https://medium.com/@tronblack" target="_blank" rel="noopener">
      <span class="comm-icon-box c-med"><i class="zmdi zmdi-account-box"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Tron Black Feed</span>
        <span class="comm-badge">Core Developer Medium[cite: 6]</span>
      </span>
    </a>
  </div>

  <!-- ============ EXPLORERS & TOOLS ============ -->
  <div class="rvn-section-title">Network Monitors &amp; Explorers</div>
  <div class="comm-grid">
    <!-- Node Map -->
    <a class="comm-card" href="http://www.ravennodes.com/" target="_blank" rel="noopener">
      <span class="comm-icon-box c-tool"><i class="zmdi zmdi-map"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Ravencoin Node Map</span>
        <span class="comm-badge">Global Peer Telemetry[cite: 6]</span>
      </span>
    </a>

    <!-- Explorer 1 -->
    <a class="comm-card" href="https://www.assetsexplorer.com/" target="_blank" rel="noopener">
      <span class="comm-icon-box c-tool"><i class="zmdi zmdi-view-list-alt"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Asset Explorer (RealBokito)</span>
        <span class="comm-badge">On-Chain Asset Search[cite: 6]</span>
      </span>
    </a>

    <!-- Explorer 2 -->
    <a class="comm-card" href="https://ravencoin.asset-explorer.net/" target="_blank" rel="noopener">
      <span class="comm-icon-box c-tool"><i class="zmdi zmdi-search"></i></span>
      <span class="comm-meta-block">
        <span class="comm-name">Asset Explorer (Scotty)</span>
        <span class="comm-badge">On-Chain Asset Search[cite: 6]</span>
      </span>
    </a>
  </div>

</div>