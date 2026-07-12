---
layout: page-w-banner
title: Wallets
bannerTitle: Ravencoin Wallets
bannerImage: /assets/img/pages/wallet/wallet-banner.jpg
permalink: /wallet/
---

<style>
  /* ---------------------------------------------------
      Modern Refined Web3 Design System Tokens
  --------------------------------------------------- */
  .rvn-wallet-wrap {
    font-family: 'Inter', sans-serif;
    max-width: 1200px;
    margin: 0 auto;
    padding: 60px 24px;
  }

  .rvn-wallet-wrap h2 {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 28px;
    font-weight: 700;
    color: #090B11;
    margin-top: 56px;
    margin-bottom: 24px;
    border-left: 4px solid #FF5A1F;
    padding-left: 14px;
  }

  .rvn-wallet-wrap h2:first-of-type {
    margin-top: 0;
  }

  .rvn-sublede {
    color: #4B5563;
    font-size: 15px;
    line-height: 1.6;
    margin-bottom: 32px;
  }

  /* ---------- Core Download Cards System ---------- */
  .dl-grid {
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(300px, 1fr));
    gap: 24px;
    margin-bottom: 32px;
  }

  .dl-card {
    background: #FFFFFF;
    border: 1px solid rgba(17, 24, 39, 0.05);
    border-radius: 20px;
    padding: 36px 32px;
    display: flex;
    flex-direction: column;
    align-items: center;
    box-shadow: 0 4px 20px -4px rgba(15, 23, 42, 0.04);
    transition: transform 0.2s ease, box-shadow 0.2s ease;
  }

  .dl-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 20px 32px -8px rgba(15, 23, 42, 0.08);
  }

  .dl-icon-box {
    height: 80px;
    width: 80px;
    border-radius: 50%;
    background: #FAFBFC;
    border: 1px solid #ECEEF1;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 24px;
    color: #3B52C6;
  }

  .dl-icon-box i {
    font-size: 40px;
  }

  .dl-card-title {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 20px;
    font-weight: 700;
    color: #090B11;
    margin-bottom: 20px;
  }

  .dl-btn {
    width: 100%;
    display: inline-flex;
    align-items: center;
    justify-content: center;
    gap: 10px;
    background: #3B52C6;
    color: #FFFFFF !important;
    font-weight: 600;
    font-size: 15px;
    text-decoration: none !important;
    padding: 14px 24px;
    border-radius: 10px;
    transition: background 0.15s ease;
  }

  .dl-btn:hover {
    background: #2A3B9F;
  }

  .dl-btn-orange { background: #FF5A1F; }
  .dl-btn-orange:hover { background: #E04810; }
  
  .dl-btn-dark { background: #090B11; }
  .dl-btn-dark:hover { background: #1E293B; }

  /* ---------- Platform Badges & Labels ---------- */
  .platform-icon-strip {
    display: flex;
    justify-content: center;
    align-items: center;
    flex-wrap: wrap;
    gap: 6px;
    margin: 4px 0 20px 0;
    min-height: 26px;
  }

  .os-tag {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    font-weight: 600;
    color: #4B5563;
    background: #F3F4F6;
    padding: 3px 8px;
    border-radius: 6px;
    display: inline-flex;
    align-items: center;
    gap: 4px;
  }

  .os-tag i {
    font-size: 13px;
  }

  .asset-support-tag {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    font-weight: 700;
    color: #FF5A1F;
    background: rgba(255, 90, 31, 0.08);
    border: 1px solid rgba(255, 90, 31, 0.15);
    padding: 4px 12px;
    border-radius: 6px;
    margin-top: 16px;
  }

  .no-asset-tag {
    height: 23px;
    margin-top: 16px;
  }

  /* ---------- Mobile Native Grid Section ---------- */
  .mobile-badges {
    display: flex;
    justify-content: center;
    gap: 16px;
    flex-wrap: wrap;
    margin: 8px 0 48px 0;
  }

  .mobile-badges img {
    height: 50px;
    transition: transform 0.15s ease;
  }

  .mobile-badges img:hover {
    transform: scale(1.03);
  }

  .center-actions {
    max-width: 500px;
    margin: 24px auto 56px auto;
    display: flex;
    flex-direction: column;
    gap: 16px;
  }
</style>

<div class="rvn-wallet-wrap">
  
  <!-- ============ DESKTOP NODE DOWNLOADS ============ -->
  <h2>Desktop Download Nodes</h2>
  <div class="dl-grid">
    <!-- Windows -->
    <div class="dl-card">
      <div class="dl-icon-box" style="color: #0078D4;"><i class="zmdi zmdi-windows"></i></div>
      <div class="dl-card-title">Windows Node</div>
      <a class="dl-btn" href="https://github.com/RavenProject/Ravencoin/releases/download/v4.6.2snapshot/raven-4.7.0-0b91b62a2-win64-setup-unsigned.exe" download>
        <i class="zmdi zmdi-download"></i><span>Download .exe Setup</span>
      </a>
    </div>

    <!-- MacOS -->
    <div class="dl-card">
      <div class="dl-icon-box" style="color: #A3AAAE;"><i class="zmdi zmdi-apple"></i></div>
      <div class="dl-card-title">macOS Node</div>
      <a class="dl-btn" href="https://github.com/RavenProject/Ravencoin/releases/download/v4.6.2snapshot/raven-4.7.0-0b91b62a2-osx-unsigned.dmg" download>
        <i class="zmdi zmdi-download"></i><span>Download .dmg Package</span>
      </a>
    </div>

    <!-- Linux -->
    <div class="dl-card">
      <div class="dl-icon-box" style="color: #FCC737;"><i class="zmdi zmdi-desktop-mac"></i></div>
      <div class="dl-card-title">Linux Node</div>
      <a class="dl-btn" href="https://github.com/RavenProject/Ravencoin/releases/download/v4.6.2snapshot/raven-4.7.0-0b91b62a2-x86_64-linux-gnu.tar.gz" download>
        <i class="zmdi zmdi-download"></i><span>Download binaries (.tar.gz)</span>
      </a>
    </div>
  </div>

  <div class="center-actions">
    <p class="rvn-sublede" style="text-align: center; margin-bottom: 0;">For binary verification hashes and secure cryptographic checksum signatures, pull directly from our core repository source:</p>
    <a class="dl-btn dl-btn-dark" href="https://github.com/RavenProject/Ravencoin/releases" target="_blank" rel="noopener">
      <i class="zmdi zmdi-github-alt"></i><span>Official GitHub Releases</span>
    </a>
  </div>

  <!-- ============ ADVANCED/ELECTRUM MODULES ============ -->
  <h2>Electrum Framework Node Options</h2>
  <p class="rvn-sublede">Lightweight desktop interface focusing on speed and optional hardware wallet compatibility layers.</p>
  <div class="center-actions" style="margin-top: 0;">
    <a class="dl-btn dl-btn-orange" href="https://github.com/Electrum-RVN-SIG/Electrum-Ravencoin/releases" target="_blank" rel="noopener">
      <i class="zmdi zmdi-github-alt"></i><span>Electrum-Ravencoin Releases</span>
    </a>
  </div>

  <!-- ============ NATIVE MOBILE APPS ============ -->
  <h2>Mobile Application Frameworks (Native Core)</h2>
  <p class="rvn-sublede" style="text-align: center;">Official mobile applications compiled directly with native Ravencoin asset layer validation mechanics:</p>
  <div class="mobile-badges">
    <a href="https://itunes.apple.com/us/app/rvn-wallet/id1371751946?mt=8" target="_blank" rel="noopener"><img src="/assets/img/pages/wallet/app-store-badge.svg" alt="App Store"></a>
    <a href="https://play.google.com/store/apps/details?id=com.ravenwallet" target="_blank" rel="noopener"><img src="/assets/img/pages/wallet/google-play-badge.svg" alt="Google Play"></a>
  </div>

  <!-- ============ INTEGRATIONS & THIRD PARTY ============ -->
  <h2>Famous &amp; Widely-Used 3rd Party Integrations</h2>
  <div class="dl-grid">
    <!-- Trust Wallet -->
    <div class="dl-card">
      <div class="dl-icon-box" style="color: #3375BB;"><i class="zmdi zmdi-shield-check"></i></div>
      <div class="dl-card-title">Trust Wallet</div>
      <div class="platform-icon-strip">
        <span class="os-tag"><i class="zmdi zmdi-apple"></i> iOS</span>
        <span class="os-tag"><i class="zmdi zmdi-android"></i> Android</span>
      </div>
      <a class="dl-btn" href="https://trustwallet.com/" target="_blank" rel="noopener nofollow">Get Trust Wallet</a>
      <div class="no-asset-tag"></div>
    </div>

    <!-- Exodus Wallet -->
    <div class="dl-card">
      <div class="dl-icon-box" style="color: #1F1F3D;"><i class="zmdi zmdi-case"></i></div>
      <div class="dl-card-title">Exodus Wallet</div>
      <div class="platform-icon-strip">
        <span class="os-tag"><i class="zmdi zmdi-desktop-mac"></i> Desktop</span>
        <span class="os-tag"><i class="zmdi zmdi-smartphone"></i> Mobile</span>
      </div>
      <a class="dl-btn" href="https://www.exodus.com/" target="_blank" rel="noopener nofollow">Get Exodus Wallet</a>
      <div class="no-asset-tag"></div>
    </div>

    <!-- Guarda Wallet -->
    <div class="dl-card">
      <div class="dl-icon-box" style="color: #00A651;"><i class="zmdi zmdi-balance-wallet"></i></div>
      <div class="dl-card-title">Guarda Wallet</div>
      <div class="platform-icon-strip">
        <span class="os-tag"><i class="zmdi zmdi-desktop-mac"></i> Desktop</span>
        <span class="os-tag"><i class="zmdi zmdi-smartphone"></i> Mobile</span>
      </div>
      <a class="dl-btn" href="https://guarda.com/" target="_blank" rel="noopener nofollow">Get Guarda Wallet</a>
      <div class="asset-support-tag">Asset Layer Support</div>
    </div>

    <!-- Atomic Wallet -->
    <div class="dl-card">
      <div class="dl-icon-box" style="color: #00A2E8;"><i class="zmdi zmdi-flash"></i></div>
      <div class="dl-card-title">Atomic Wallet</div>
      <div class="platform-icon-strip">
        <span class="os-tag"><i class="zmdi zmdi-desktop-mac"></i> Desktop</span>
        <span class="os-tag"><i class="zmdi zmdi-smartphone"></i> Mobile</span>
      </div>
      <a class="dl-btn" href="https://atomicwallet.io/" target="_blank" rel="noopener nofollow">Get Atomic Wallet</a>
      <div class="no-asset-tag"></div>
    </div>

    <!-- D'CENT Wallet -->
    <div class="dl-card">
      <div class="dl-icon-box" style="color: #E9573F;"><i class="zmdi zmdi-fingerprint"></i></div>
      <div class="dl-card-title">D'CENT Hardware</div>
      <div class="platform-icon-strip">
        <span class="os-tag"><i class="zmdi zmdi-usb"></i> Hardware</span>
        <span class="os-tag"><i class="zmdi zmdi-smartphone"></i> App</span>
      </div>
      <a class="dl-btn" href="https://dcentwallet.com/" target="_blank" rel="noopener nofollow">Get D'CENT Wallet</a>
      <div class="asset-support-tag">Asset Layer Support</div>
    </div>

    <!-- Trezor Wallet -->
    <div class="dl-card">
      <div class="dl-icon-box" style="color: #00B074;"><i class="zmdi zmdi-key"></i></div>
      <div class="dl-card-title">Trezor Hardware</div>
      <div class="platform-icon-strip">
        <span class="os-tag"><i class="zmdi zmdi-usb"></i> Cold Storage</span>
      </div>
      <a class="dl-btn" href="https://trezor.io/" target="_blank" rel="noopener nofollow">Get Trezor Wallet</a>
      <div class="no-asset-tag"></div>
    </div>
  </div>

  <!-- ============ PAPER WALLETS ============ -->
  <h2>Deterministic Paper Storage Engines</h2>
  <div class="dl-grid">
    <div class="dl-card">
      <a class="dl-btn dl-btn-dark" href="https://github.com/todd1251/WalletGenerator.net/tree/ravencoin" target="_blank" rel="noopener nofollow">
        <i class="zmdi zmdi-print"></i><span>Paper Engine (Penfold Build)</span>
      </a>
    </div>
    <div class="dl-card">
      <a class="dl-btn dl-btn-dark" href="https://paper.pocketraven.com/" target="_blank" rel="noopener nofollow">
        <i class="zmdi zmdi-print"></i><span>Paper Engine (Traysi Build)</span>
      </a>
    </div>
  </div>

</div>