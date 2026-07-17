---
layout: default
title: Home
permalink: /
modalTitle: "Announcement"
modalContent: 'New Wallet Release: Upgrade to Version 4.7.0 <a href="/wallet">Click Here to Upgrade</a>'
modalId: "upgrade-notification"
modalCacheRef: "4.7.0"
---

<link href="/assets/vendors/mediabox/mediabox.css" rel="stylesheet">
<link href="https://fonts.googleapis.com/css2?family=Space+Grotesk:wght@500;600;700&family=Inter:wght@400;500;600;700&family=IBM+Plex+Mono:wght@500;600&display=swap" rel="stylesheet">

<style>
  /* ---------------------------------------------------
      Modern Refined Web3 Design System Tokens
  --------------------------------------------------- */
  .rvn-home {
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
    --glow-ember: rgba(255, 90, 31, 0.15);
    --gold: #F0B429;
    --silver: #A0AEC0;
    --bronze: #C97B3E;

    font-family: 'Inter', -apple-system, sans-serif;
    -webkit-font-smoothing: antialiased;
    background: var(--bg-light);
    color: var(--text-primary-light);
    overflow-x: hidden;
  }

  .rvn-home h1, .rvn-home h2, .rvn-home h3 {
    font-family: 'Space Grotesk', sans-serif;
    letter-spacing: -0.02em;
  }

  .rvn-home .mono {
    font-family: 'IBM Plex Mono', monospace;
  }

  .rvn-home .wrap {
    max-width: 1200px;
    margin: 0 auto !important;
    padding: 0 24px;
    display: block;
  }

  /* ---------- Premium Hero Section ---------- */
  .rvn-hero {
    position: relative;
    display: block;
    width: 100%;
    clear: both;
    background: radial-gradient(circle at 80% 20%, rgba(59, 82, 198, 0.15), transparent 50%),
                radial-gradient(circle at 20% 80%, var(--glow-ember), transparent 50%),
                #090B11;
    color: var(--text-primary-dark);
    padding: 140px 0 80px;
    border-bottom: 1px solid var(--border-dark);
  }

  .rvn-hero::before {
    content: "";
    position: absolute;
    inset: 0;
    background-image: url("/assets/img/home/gplaypattern.png");
    opacity: 0.03;
    mix-blend-mode: overlay;
    pointer-events: none;
  }

  .rvn-hero-inner {
    position: relative;
    z-index: 2;
    text-align: center;
  }

  .rvn-eyebrow {
    display: inline-flex;
    align-items: center;
    gap: 8px;
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    font-weight: 600;
    letter-spacing: 0.14em;
    text-transform: uppercase;
    color: #A5B4FC;
    background: rgba(59, 82, 198, 0.15);
    border: 1px solid rgba(165, 180, 252, 0.3);
    border-radius: 999px;
    padding: 6px 16px;
    margin-bottom: 32px;
  }

  .rvn-eyebrow .dot {
    width: 6px;
    height: 6px;
    border-radius: 50%;
    background: var(--brand-ember);
    box-shadow: 0 0 12px var(--brand-ember);
    animation: pulseGlow 2s infinite;
  }

  @keyframes pulseGlow {
    0% { transform: scale(0.9); opacity: 0.6; }
    50% { transform: scale(1.2); opacity: 1; box-shadow: 0 0 16px var(--brand-ember); }
    100% { transform: scale(0.9); opacity: 0.6; }
  }

  .rvn-hero h1 {
    font-size: 54px;
    font-weight: 700;
    line-height: 1.15;
    max-width: 880px;
    margin: 0 auto 24px;
    background: linear-gradient(180deg, #FFFFFF 0%, #CBD5E1 100%);
    -webkit-background-clip: text;
    -webkit-text-fill-color: transparent;
  }

  .rvn-hero p.lede {
    max-width: 640px;
    margin: 0 auto 44px;
    color: var(--text-secondary-dark);
    font-size: 18px;
    line-height: 1.6;
  }

  .rvn-hero-buttons {
    display: flex;
    justify-content: center;
    align-items: center;
    gap: 16px;
    flex-wrap: wrap;
    margin-bottom: 48px;
  }

  .rvn-btn {
    display: inline-flex;
    align-items: center;
    gap: 10px;
    padding: 14px 30px;
    border-radius: 10px;
    font-weight: 600;
    font-size: 15px;
    text-decoration: none;
    transition: all 0.2s cubic-bezier(0.16, 1, 0.3, 1);
    border: 1px solid transparent;
  }

  .rvn-btn:hover {
    transform: translateY(-2px);
    box-shadow: 0 12px 20px -6px rgba(0, 0, 0, 0.3);
    text-decoration: none;
  }

  .rvn-btn-primary {
    background: var(--brand-ember);
    color: #FFFFFF;
  }

  .rvn-btn-primary:hover {
    background: var(--brand-ember-hover);
    color: #FFFFFF;
    box-shadow: 0 12px 24px -6px rgba(255, 90, 31, 0.4);
  }

  .rvn-btn-ghost {
    background: rgba(255, 255, 255, 0.03);
    color: #FFFFFF;
    border-color: var(--border-dark);
    backdrop-filter: blur(8px);
  }

  .rvn-btn-ghost:hover {
    background: rgba(255, 255, 255, 0.08);
    border-color: rgba(255, 255, 255, 0.3);
    color: #FFFFFF;
  }

  .rvn-video-icon {
    display: inline-flex;
    align-items: center;
    gap: 12px;
    color: #FFFFFF;
    font-size: 15px;
    font-weight: 600;
    text-decoration: none;
    padding: 10px 20px;
    border-radius: 999px;
    background: rgba(255, 255, 255, 0.05);
    border: 1px solid var(--border-dark);
    transition: all 0.2s ease;
  }

  .rvn-video-icon:hover {
    background: rgba(255, 255, 255, 0.1);
    border-color: rgba(255, 255, 255, 0.2);
    color: var(--brand-ember);
    text-decoration: none;
  }

  .rvn-video-icon svg {
    width: 24px;
    height: 24px;
    transition: transform 0.2s ease;
  }

  .rvn-video-icon:hover svg {
    transform: scale(1.1);
  }

  .rvn-links-row {
    display: flex;
    justify-content: center;
    gap: 32px;
    flex-wrap: wrap;
    margin-top: 56px;
    padding-top: 32px;
    border-top: 1px solid var(--border-dark);
  }

  .rvn-links-row a {
    color: var(--text-secondary-dark);
    font-size: 14px;
    font-weight: 500;
    text-decoration: none;
    transition: color 0.2s ease;
  }

  .rvn-links-row a:hover {
    color: #FFFFFF;
  }

  /* ---------- Modern Live Statistics Strip ---------- */
  .rvn-ledger {
    display: block;
    width: 100%;
    clear: both;
    background: #0B0E17;
    border-top: 1px solid var(--border-dark);
    border-bottom: 1px solid var(--border-dark);
  }

  .rvn-ledger .wrap {
    display: grid;
    grid-template-columns: repeat(4, 1fr);
  }

  .rvn-ledger-cell {
    padding: 26px 24px;
    border-right: 1px solid var(--border-dark);
    text-align: center;
    transition: background 0.2s ease;
  }

  .rvn-ledger-cell:hover {
    background: rgba(255, 255, 255, 0.02);
  }

  .rvn-ledger-cell:last-child {
    border-right: none;
  }

  .rvn-ledger-label {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 11px;
    font-weight: 600;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--text-secondary-dark);
    margin-bottom: 8px;
  }

  .rvn-ledger-value {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 22px;
    font-weight: 700;
    color: #FFFFFF;
  }

  /* ---------- Clean Section Framework ---------- */
  .rvn-section {
    display: block;
    width: 100% !important;
    clear: both !important;
    padding: 100px 0;
    position: relative;
  }

  .rvn-section-head {
    max-width: 700px;
    margin: 0 auto 56px;
    text-align: center;
  }

  .rvn-section-head h2 {
    font-size: 38px;
    font-weight: 700;
    margin-bottom: 16px;
    color: inherit;
  }

  .rvn-section-head p {
    font-size: 17px;
    line-height: 1.6;
    margin: 0;
  }

  /* ---------- Interactive Assets Feature Block ---------- */
  .rvn-assets {
    background: #0D111C;
    color: var(--text-primary-dark);
  }

  .rvn-assets .rvn-section-head p {
    color: var(--text-secondary-dark);
  }

  ul.nav-tabs.rvn-tablist {
    list-style: none;
    display: flex;
    justify-content: center;
    gap: 12px;
    flex-wrap: wrap;
    margin: 0 0 48px;
    padding: 6px;
    background: rgba(255, 255, 255, 0.03);
    border: 1px solid var(--border-dark);
    border-radius: 999px;
    max-width: fit-content;
    margin-left: auto;
    margin-right: auto;
  }

  ul.nav-tabs.rvn-tablist li a {
    display: block;
    padding: 10px 24px;
    border-radius: 999px;
    font-size: 14px;
    font-weight: 600;
    color: var(--text-secondary-dark);
    text-decoration: none;
    transition: all 0.2s cubic-bezier(0.16, 1, 0.3, 1);
    border: 1px solid transparent;
  }

  ul.nav-tabs.rvn-tablist li a:hover {
    color: #FFFFFF;
  }

  ul.nav-tabs.rvn-tablist li.active a {
    background: var(--brand-ember);
    color: #FFFFFF;
    box-shadow: 0 4px 12px rgba(255, 90, 31, 0.25);
  }

  .tab-content .tab-pane {
    display: none;
  }

  .tab-content .tab-pane.active {
    display: block;
    animation: fadeIn 0.4s cubic-bezier(0.16, 1, 0.3, 1);
  }

  @keyframes fadeIn {
    from { opacity: 0; transform: translateY(8px); }
    to { opacity: 1; transform: translateY(0); }
  }

  .rvn-tab-card {
    background: var(--bg-card-dark);
    border: 1px solid var(--border-dark);
    border-radius: 24px;
    padding: 56px;
    display: flex;
    gap: 56px;
    align-items: center;
    flex-wrap: wrap;
    box-shadow: 0 20px 40px -15px rgba(0, 0, 0, 0.5);
  }

  .rvn-tab-icon {
    flex: 0 0 160px;
    text-align: center;
  }

  .rvn-tab-icon img {
    max-width: 130px;
    filter: drop-shadow(0 8px 16px rgba(0,0,0,0.2));
    transition: transform 0.3s ease;
  }

  .rvn-tab-card:hover .rvn-tab-icon img {
    transform: scale(1.05) rotate(2deg);
  }

  .rvn-tab-body {
    flex: 1 1 400px;
  }

  .rvn-tab-body h3 {
    color: #FFFFFF;
    font-size: 24px;
    font-weight: 700;
    margin: 0 0 24px;
  }

  .rvn-tab-body ul {
    list-style: none;
    padding: 0;
    margin: 0;
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 14px 32px;
  }

  .rvn-tab-body ul li {
    color: var(--text-secondary-dark);
    font-size: 15px;
    font-weight: 500;
    padding-left: 24px;
    position: relative;
    line-height: 1.5;
  }

  .rvn-tab-body ul li::before {
    content: "✓";
    position: absolute;
    left: 0;
    top: 0;
    color: var(--brand-ember);
    font-weight: 700;
  }

  /* ---------- Why different (Comparison Section) ---------- */
  .rvn-why {
    background: #FFFFFF;
    color: var(--text-primary-light);
  }

  .rvn-why-grid {
    display: grid !important;
    grid-template-columns: 1.2fr 1fr;
    gap: 64px;
    align-items: start;
  }

  .rvn-why-content {
    display: flex;
    flex-direction: column;
  }

  .rvn-why-title {
    font-size: 32px;
    font-weight: 700;
    margin-top: 0;
    margin-bottom: 24px;
    color: var(--text-primary-light);
  }

  .rvn-compare {
    list-style: none;
    padding: 0;
    margin: 0;
    display: flex;
    flex-direction: column;
    gap: 12px;
  }

  .rvn-compare li {
    display: flex;
    align-items: center;
    justify-content: space-between;
    gap: 20px;
    background: var(--bg-light);
    border: 1px solid var(--border-light);
    border-radius: 12px;
    padding: 18px 24px;
    transition: all 0.2s ease;
  }

  .rvn-compare li:hover {
    transform: translateX(4px);
    border-color: rgba(59, 82, 198, 0.3);
    background: #FFFFFF;
    box-shadow: 0 8px 16px -4px rgba(15, 23, 42, 0.04);
  }

  .rvn-compare .label {
    font-size: 15px;
    color: var(--text-primary-light);
    font-weight: 600;
  }

  .rvn-compare .value {
    font-family: 'IBM Plex Mono', monospace;
    font-size: 14px;
    font-weight: 600;
    color: var(--brand-navy);
    white-space: nowrap;
    background: rgba(59, 82, 198, 0.06);
    padding: 4px 12px;
    border-radius: 6px;
  }

  .rvn-why-art {
    text-align: center;
    display: flex;
    justify-content: center;
    align-items: center;
  }

  .rvn-why-art img {
    max-width: 260px;
    height: auto;
    filter: drop-shadow(0 20px 40px rgba(15, 23, 42, 0.08));
  }

  /* ---------- Conversion Block (CTA) ---------- */
  .rvn-cta {
    background: linear-gradient(135deg, #1E293B 0%, #0F172A 100%);
    color: #FFFFFF;
    padding: 80px 0;
  }

  .rvn-cta-inner {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 32px;
    flex-wrap: wrap;
  }

  .rvn-cta h2 {
    font-size: 32px;
    font-weight: 700;
    margin-bottom: 8px;
  }

  .rvn-cta p {
    margin: 0;
    color: var(--text-secondary-dark);
    font-size: 16px;
    max-width: 520px;
  }

  /* ---------- Exchange Card Grid ---------- */
  .rvn-exchanges {
    background: #FFFFFF;
    border-top: 1px solid var(--border-light);
  }

  .exch-grid {
    display: grid;
    grid-template-columns: repeat(auto-fill, minmax(200px, 1fr));
    gap: 14px;
  }

  .exch-card {
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

  .exch-card:hover {
    transform: translateY(-3px);
    box-shadow: 0 14px 26px -10px rgba(15, 23, 42, 0.14);
    border-color: rgba(59, 82, 198, 0.25);
    color: inherit;
    text-decoration: none;
  }

  .exch-logo {
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

  .exch-logo img {
    width: 100%;
    height: 100%;
    object-fit: contain;
    padding: 6px;
  }

  .exch-name-block { min-width: 0; }

  .exch-name {
    font-weight: 600;
    font-size: 14.5px;
    color: var(--text-primary-light);
    white-space: nowrap;
    overflow: hidden;
    text-overflow: ellipsis;
    display: block;
  }

  .exch-badge {
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

  .cmc-show-more {
    text-align: center;
    margin-top: 40px;
  }

  /* ---------- Modern Social Section ---------- */
  .rvn-social {
    background: #090B11;
    padding: 100px 0;
    text-align: center;
    border-top: 1px solid var(--border-dark);
  }

  .rvn-social h2 {
    color: #FFFFFF;
    margin-bottom: 48px;
    font-size: 34px;
  }

  .rvn-social-row {
    display: flex;
    gap: 32px;
    justify-content: center;
    flex-wrap: wrap;
  }

  .rvn-social-row iframe, .rvn-social-row .twitter-timeline {
    border-radius: 16px !important;
    border: 1px solid var(--border-dark) !important;
    background: var(--bg-card-dark) !important;
    box-shadow: 0 20px 40px -15px rgba(0,0,0,0.3);
  }

  /* ---------- Custom Animation States for Waypoints ---------- */
  .fadeInLeft, .fadeInRight {
    opacity: 0;
    transition: opacity 0.6s ease, transform 0.6s ease;
  }
  .fadeInLeft { transform: translateX(-20px); }
  .fadeInRight { transform: translateX(20px); }
  .rvn-home .active.fadeInLeft, .rvn-home .active.fadeInRight {
    opacity: 1;
    transform: translateX(0);
  }

  /* ---------- Responsive Layout Breakpoints ---------- */
  @media (max-width: 960px) {
    .rvn-hero h1 { font-size: 40px; }
    .rvn-tab-card { padding: 40px; gap: 32px; }
    .rvn-why-grid { grid-template-columns: 1fr !important; gap: 48px; }
    .rvn-why-art { order: -1; }
  }

  @media (max-width: 768px) {
    .rvn-ledger .wrap { grid-template-columns: repeat(2, 1fr); }
    .rvn-ledger-cell { border-bottom: 1px solid var(--border-dark); }
    .rvn-ledger-cell:nth-child(2) { border-right: none; }
    .rvn-ledger-cell:nth-child(3), .rvn-ledger-cell:nth-child(4) { border-bottom: none; }
    .rvn-tab-body ul { grid-template-columns: 1fr; }
    .rvn-cta-inner { text-align: center; justify-content: center; }
    .rvn-section h2 { font-size: 30px; }
    ul.nav-tabs.rvn-tablist { border-radius: 16px; padding: 12px; }
    ul.nav-tabs.rvn-tablist li a { padding: 8px 16px; }
    .cmc-name { max-width: 140px; }

    .rvn-compare li { flex-direction: column; align-items: flex-start; gap: 6px; }
    .rvn-compare .value {
      white-space: normal !important;
      word-break: break-word !important;
      max-width: 100% !important;
      display: inline-block !important;
    }
  }

  @media (max-width: 480px) {
    .rvn-hero { padding: 96px 0 56px; }
    .rvn-hero h1 { font-size: 30px; }
    .rvn-hero p.lede { font-size: 15px; }
    .rvn-eyebrow { font-size: 10px; padding: 6px 12px; }

    .rvn-hero-buttons { flex-direction: column; align-items: stretch; gap: 12px; }
    .rvn-btn { width: 100%; justify-content: center; }
    .video-icon { width: 100%; }
    .rvn-video-icon { width: 100%; justify-content: center; }

    .rvn-links-row { flex-direction: column; gap: 14px; margin-top: 40px; padding-top: 24px; }

    .rvn-ledger .wrap { grid-template-columns: 1fr; }
    .rvn-ledger-cell { border-right: none !important; border-bottom: 1px solid var(--border-dark); }
    .rvn-ledger-cell:last-child { border-bottom: none; }

    .rvn-section { padding: 64px 0; }
    .rvn-section-head h2 { font-size: 26px; }

    .rvn-tab-card { padding: 24px; gap: 24px; }
    .rvn-tab-icon { flex-basis: 100%; }
    .rvn-tab-icon img { max-width: 90px; }

    .rvn-why-title { font-size: 26px; }
    .rvn-compare li { flex-direction: column; align-items: flex-start; gap: 6px; }
    .rvn-compare .value {
      white-space: normal !important;
      word-break: break-word !important;
      max-width: 100% !important;
      display: inline-block !important;
    }

    .rvn-cta { padding: 56px 0; }
    .rvn-cta-inner { flex-direction: column; text-align: center; }
    .rvn-cta .rvn-btn { width: 100%; justify-content: center; }

    .exch-grid { grid-template-columns: 1fr; }

    .rvn-social { padding: 64px 0; }
    .rvn-social-row { flex-direction: column; align-items: center; }
    .rvn-social-row iframe,
    .rvn-social-row .twitter-timeline { width: 100% !important; max-width: 360px; }
  }
</style>

<div class="rvn-home">

  <section class="rvn-hero">
    <div class="wrap rvn-hero-inner">
      <span class="rvn-eyebrow"><span class="dot"></span>Live on mainnet since 2018</span>
      <h1>A peer-to-peer blockchain built to move assets, not just coins.</h1>
      <p class="lede">Ravencoin lets anyone issue, transfer, and trade tokenized assets — shares, tickets, credits, or collectibles — directly on-chain.</p>

      <div class="rvn-hero-buttons">
        <a class="rvn-btn rvn-btn-primary" href="/wallet/">Get Your Wallet</a>
        <a class="rvn-btn rvn-btn-ghost" href="/buy-ravencoin/">Buy Ravencoin</a>

        <div class="video-icon" uk-lightbox>
          <a class="rvn-video-icon mediabox" href="https://www.youtube.com/embed/fbfUvkZaw2w?rel=0&amp;showinfo=0">
            <svg xmlns="http://www.w3.org/2000/svg" viewBox="0 0 512 512">
              <path d="M256,0C114.617,0,0,114.615,0,256s114.617,256,256,256,256-114.615,256-256S397.383,0,256,0z M344.48,269.57l-128,80  c-2.59,1.617-5.535,2.43-8.48,2.43c-2.668,0-5.34-0.664-7.758-2.008C195.156,347.172,192,341.82,192,336V176  c0-5.82,3.156-11.172,8.242-13.992c5.086-2.836,11.305-2.664,16.238,0.422l128,80c4.676,2.93,7.52,8.055,7.52,13.57  S349.156,266.641,344.48,269.57z" fill="currentColor"/>
            </svg>
            <span>What is Ravencoin?</span>
          </a>
        </div>
      </div>

      <div class="rvn-links-row">
        <a href="https://github.com/RavenProject/Ravencoin/wiki" target="_blank" rel="noopener">Official Wiki</a>
        <a href="https://github.com/RavenProject/Ravencoin" target="_blank" rel="noopener">Source Code</a>
        <a href="https://discord.gg/fndp4NBGct" target="_blank" rel="noopener">Community Discord</a>
      </div>
    </div>
  </section>

  <div class="rvn-ledger">
    <div class="wrap">
      <div class="rvn-ledger-cell">
        <div class="rvn-ledger-label">Block Reward</div>
        <div class="rvn-ledger-value">1,250 RVN</div>
      </div>
      <div class="rvn-ledger-cell">
        <div class="rvn-ledger-label">Block Time</div>
        <div class="rvn-ledger-value">~60 sec</div>
      </div>
      <div class="rvn-ledger-cell">
        <div class="rvn-ledger-label">Supply Cap</div>
        <div class="rvn-ledger-value">21,000,000,000</div>
      </div>
      <div class="rvn-ledger-cell">
        <div class="rvn-ledger-label">Algorithm</div>
        <div class="rvn-ledger-value">KAWPOW</div>
      </div>
    </div>
  </div>

  <section class="rvn-section rvn-assets">
    <div class="wrap">
      <div class="rvn-section-head">
        <h2>Any asset can live on-chain</h2>
        <p>Issue a tokenized block asset in minutes and configure unique parameters to fit international compliance, volume rules, and transfer mechanics.</p>
      </div>

      <ul class="nav nav-tabs rvn-tablist list-reset">
        <li class="active"><a href="#tab-1">Project Shares</a></li>
        <li class="tab-2"><a href="#tab-2">Virtual Goods</a></li>
        <li class="tab-3"><a href="#tab-3">Physical &amp; Digital Assets</a></li>
        <li class="tab-4"><a href="#tab-4">Credit</a></li>
      </ul>

      <div class="tab-content">
        <div id="tab-1" class="tab-pane active">
          <div class="rvn-tab-card">
            <div class="rvn-tab-icon">
              <img id="tab-token" class="fadeInLeft" src="/assets/img/svg/token.svg" alt="token"/>
            </div>
            <div class="rvn-tab-body">
              <h3>Representing a share of a project</h3>
              <ul>
                <li>On-chain Security Tokens</li>
                <li>RVN Dividend Partnership shares</li>
                <li>Limited royalty pools</li>
                <li>Crowd-funded corporate assets</li>
              </ul>
            </div>
          </div>
        </div>

        <div id="tab-2" class="tab-pane">
          <div class="rvn-tab-card">
            <div class="rvn-tab-icon">
              <img id="tab-tickets" class="fadeInLeft" src="/assets/img/svg/tickets.svg" alt="tickets"/>
            </div>
            <div class="rvn-tab-body">
              <h3>Representing virtual goods</h3>
              <ul>
                <li>Resellable Event Tickets</li>
                <li>Activity & Operational Licenses</li>
                <li>Service Access Tokens</li>
                <li>In-game Currencies &amp; Items</li>
              </ul>
            </div>
          </div>
        </div>

        <div id="tab-3" class="tab-pane">
          <div class="rvn-tab-card">
            <div class="rvn-tab-icon">
              <img id="tab-gold" class="fadeInLeft" src="/assets/img/svg/gold.svg" alt="gold"/>
            </div>
            <div class="rvn-tab-body">
              <h3>Real-world custodied physical or digital assets</h3>
              <ul>
                <li>Gold bar backing</li>
                <li>Land Title Deeds</li>
                <li>Silver coins &amp; bullion</li>
                <li>Collectible Comics</li>
                <li>Physical Fiat Reserves</li>
                <li>Energy commodities</li>
              </ul>
            </div>
          </div>
        </div>

        <div id="tab-4" class="tab-pane">
          <div class="rvn-tab-card">
            <div class="rvn-tab-icon">
              <img id="tab-gift-card" class="fadeInLeft" src="/assets/img/svg/gift-card.svg" alt="gift-card"/>
            </div>
            <div class="rvn-tab-body">
              <h3>Representing custom credits</h3>
              <ul>
                <li>Retail Gift Cards</li>
                <li>Airline Frequent Flyer Miles</li>
                <li>Ecosystem Reward Points</li>
              </ul>
            </div>
          </div>
        </div>
      </div>
    </div>
  </section>

  <section class="rvn-section rvn-why">
    <div class="wrap rvn-why-grid">
      <div class="rvn-why-content">
        <h2 class="rvn-why-title">What makes Ravencoin different from Bitcoin?</h2>
        <ul class="rvn-compare">
          <li>
            <span class="label">Core Focus</span>
            <span class="value">Asset Tokenization vs Digital Gold</span>
          </li>
          <li>
            <span class="label">Block Reward</span>
            <span class="value">1,250 RVN vs 3.125 BTC</span>
          </li>
          <li>
            <span class="label">Block Time</span>
            <span class="value">1 min vs 10 min</span>
          </li>
          <li>
            <span class="label">Total Supply</span>
            <span class="value">21 Billion vs 21 Million</span>
          </li>
          <li>
            <span class="label">Mining Algorithm</span>
            <span class="value">KAWPOW (Anti-ASIC) vs SHA-256 (ASIC)</span>
          </li>
          <li>
            <span class="label">Asset Issuance</span>
            <span class="value">Native Layer-1 vs Complex L2 / Protocols</span>
          </li>
          <li>
            <span class="label">Dividend Payments</span>
            <span class="value">Native RVN Distribution vs Not Supported</span>
          </li>
          <li>
            <span class="label">Avg. Transfer Fee</span>
            <span class="value">Sub-Penny vs Variable ($1 - $10+)</span>
          </li>
        </ul>
      </div>
      <div class="rvn-why-art">
        <img id="logo-why" class="fadeInRight" src="/assets/img/home/raven-flock.png" alt="ravencoin logo">
      </div>
    </div>
  </section>

  <section class="rvn-cta">
    <div class="wrap rvn-cta-inner">
      <div>
        <h2>Get involved today</h2>
        <p>Join a global, decentralized network of open-source miners, institutional contributors, traders, and engineers.</p>
      </div>
      <br>
      <a class="rvn-btn rvn-btn-primary" href="/community">Join the Community</a>
    </div>
  </section>

  <section class="rvn-section rvn-exchanges">
    <div class="wrap">
      <div class="rvn-section-head">
        <h2>Top 10 Ravencoin Exchanges</h2>
        <p>The top market platforms trading RVN, parsed directly from major global volume rankings.</p>
      </div>

      <div class="exch-grid">
        <a class="exch-card" href="https://www.binance.com/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/binance.png" alt="Binance"></span>
          <span class="exch-name-block">
            <span class="exch-name">Binance</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>

        <a class="exch-card" href="https://www.bybit.com/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/bybit.png" alt="Bybit"></span>
          <span class="exch-name-block">
            <span class="exch-name">Bybit</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>

        <a class="exch-card" href="https://www.okx.com/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/okx.png" alt="OKX"></span>
          <span class="exch-name-block">
            <span class="exch-name">OKX</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>

        <a class="exch-card" href="https://www.kraken.com/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/kraken.png" alt="Kraken"></span>
          <span class="exch-name-block">
            <span class="exch-name">Kraken</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>

        <a class="exch-card" href="https://www.kucoin.com/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/kucoin.png" alt="KuCoin"></span>
          <span class="exch-name-block">
            <span class="exch-name">KuCoin</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>

        <a class="exch-card" href="https://www.gate.io/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/gateio.png" alt="Gate.io"></span>
          <span class="exch-name-block">
            <span class="exch-name">Gate.io</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>

        <a class="exch-card" href="https://www.mexc.com/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/mexc.png" alt="MEXC"></span>
          <span class="exch-name-block">
            <span class="exch-name">MEXC</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>

        <a class="exch-card" href="https://www.htx.com/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/htx.png" alt="HTX"></span>
          <span class="exch-name-block">
            <span class="exch-name">HTX</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>

        <a class="exch-card" href="https://www.bitget.com/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/bitget.png" alt="Bitget"></span>
          <span class="exch-name-block">
            <span class="exch-name">Bitget</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>

        <a class="exch-card" href="https://www.coinex.com/" target="_blank" rel="noopener nofollow">
          <span class="exch-logo"><img src="/assets/img/pages/exchanges/coinex.png" alt="CoinEx"></span>
          <span class="exch-name-block">
            <span class="exch-name">CoinEx</span>
            <span class="exch-badge">Top 10 Exchange</span>
          </span>
        </a>
      </div>

      <div class="cmc-show-more">
        <a class="rvn-btn rvn-btn-primary" href="/buy-ravencoin/">See All Exchanges</a>
      </div>
    </div>
  </section>

  <section class="rvn-social">
    <div class="wrap">
      <h2>Ecosystem Updates</h2>
      <div class="rvn-social-row">
        <a class="twitter-timeline" data-width="500" data-height="600" data-dnt="true" data-theme="dark" href="https://twitter.com/Ravencoin?ref_src=twsrc%5Etfw">Tweets by Ravencoin</a>
        <a class="twitter-timeline" data-width="500" data-height="600" data-dnt="true" data-theme="dark" href="https://twitter.com/Ravencoin/likes?ref_src=twsrc%5Etfw">Tweets Liked by Ravencoin</a>
      </div>
      <script async src="https://platform.twitter.com/widgets.js" charset="utf-8"></script>
    </div>
  </section>

</div>

<script src="/assets/vendors/mediabox/mediabox.js"></script>
<script>
  MediaBox('.mediabox');
</script>

<script type="text/javascript">
  window.addEventListener("load", function() {

    /* Tab Switcher Logic */
    var myTabs = document.querySelectorAll("ul.nav-tabs > li");
    function myTabClicks(tabClickEvent) {
      for (var i = 0; i < myTabs.length; i++) {
        myTabs[i].classList.remove("active");
      }
      var clickedTab = tabClickEvent.currentTarget;
      clickedTab.classList.add("active");
      tabClickEvent.preventDefault();

      var myContentPanes = document.querySelectorAll(".tab-pane");
      for (i = 0; i < myContentPanes.length; i++) {
        myContentPanes[i].classList.remove("active");
      }
      var anchorReference = tabClickEvent.target;
      var activePaneId = anchorReference.getAttribute("href");
      var activePane = document.querySelector(activePaneId);
      activePane.classList.add("active");
    }
    for (i = 0; i < myTabs.length; i++) {
      myTabs[i].addEventListener("click", myTabClicks);
    }

    /* Waypoints Transitions Trigger Script */
    const targets = ['tab-token', 'tab-tickets', 'tab-gold', 'tab-gift-card', 'logo-why'];
    targets.forEach(function(target) {
      var el = document.getElementById(target);
      if (!el) return;
      var waypoint = new Waypoint({
        element: el,
        handler: function(direction) {
          el.classList.add('active');
        },
        offset: '95%'
      });
    });
  });
</script>