---
layout: page-w-banner
title: About
description: "Ravencoin is a digital peer to peer network that aims to implement a use case specific blockchain, designed to efficiently handle one specific function: the transfer of assets from one party to another."
bannerTitle: About the Ravencoin Project
bannerImage: /assets/img/pages/about/about-banner.jpg
permalink: /about/
---

<style>
  .rvn-about-container {
    font-family: 'Inter', sans-serif;
    color: #111827;
    max-width: 900px;
    margin: 0 auto;
    padding: 60px 24px;
  }
  .rvn-about-container h2, .rvn-about-container h3 {
    font-family: 'Space Grotesk', sans-serif;
    letter-spacing: -0.02em;
    color: #090B11;
    margin-top: 40px;
    margin-bottom: 20px;
  }
  .rvn-about-container h2 { font-size: 36px; border-bottom: 2px solid rgba(255, 90, 31, 0.1); padding-bottom: 12px; }
  .rvn-about-container h3 { font-size: 24px; }
  .rvn-about-container p { font-size: 16px; line-height: 1.7; color: #4B5563; margin-bottom: 24px; }
  
  .rvn-blockquote {
    border-left: 4px solid #FF5A1F;
    background: #F8F9FA;
    padding: 24px;
    margin: 32px 0;
    border-radius: 0 12px 12px 0;
  }
  .rvn-blockquote p {
    font-style: italic;
    color: #1E293B;
    font-size: 18px;
    margin: 0;
  }

  .rvn-spec-list {
    list-style: none;
    padding: 0;
    display: grid;
    grid-template-columns: repeat(auto-fit, minmax(200px, 1fr));
    gap: 16px;
    margin: 32px 0;
  }
  .rvn-spec-list li {
    background: #FFFFFF;
    border: 1px solid rgba(17, 24, 39, 0.05);
    border-radius: 12px;
    padding: 16px 20px;
    font-weight: 600;
    font-size: 15px;
    color: #3B52C6;
    box-shadow: 0 4px 6px -1px rgba(0, 0, 0, 0.02);
    display: flex;
    align-items: center;
    gap: 10px;
  }
  .rvn-spec-list li::before {
    content: "";
    width: 8px;
    height: 8px;
    background: #FF5A1F;
    border-radius: 50%;
  }

  .rvn-badge-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 20px;
    margin-top: 32px;
  }
  @media (max-width: 640px) {
    .rvn-badge-grid { grid-template-columns: 1fr; }
  }
  .rvn-badge-card {
    background: #090B11;
    color: #FFFFFF;
    padding: 24px;
    border-radius: 16px;
    border: 1px solid rgba(255, 255, 255, 0.08);
  }
  .rvn-badge-card h4 { font-family: 'Space Grotesk', sans-serif; font-size: 18px; margin: 0 0 8px; color: #FF5A1F; }
  .rvn-badge-card p { color: #94A3B8; font-size: 14px; margin: 0; line-height: 1.5; }
</style>

<div class="rvn-about-container">
  <h2>What is Ravencoin?</h2>
  <p>Ravencoin is a digital peer to peer network that aims to implement a use case specific blockchain, designed to efficiently handle one specific function: the transfer of assets from one party to another. Built on a fork of the Bitcoin code, Ravencoin was launched January 3rd, 2018, and is a truly open source project (no ICO or masternodes). It focuses on building a useful technology, with a strong and growing community.</p>

  <h3>How Ravencoin works</h3>
  <p>A Ravencoin post on <em>Medium</em> from November 2017 references Game of Thrones when introducing this experimental currency:</p>
  
  <div class="rvn-blockquote">
    <p>“In the fictional world of Westeros, ravens are used as messengers who carry statements of truth. Ravencoin is a use case specific blockchain designed to carry statements of truth about who owns what assets”</p>
  </div>

  <p>Launched on January 3rd, 2018, the ninth anniversary of bitcoin’s launch, Ravencoin is an open-source project designed to enable instant payments to anyone around the world. The aim of the project is to create a blockchain optimized specifically for the transfer of assets such as tokens from one holder to another.</p>

  <p>A fork of the bitcoin code, Ravencoin features four key core parameters:</p>
  <ul class="rvn-spec-list">
    <li>Issuance Schedule Changes</li>
    <li>1 Minute Block Time</li>
    <li>21 Billion Coin Supply</li>
    <li>KAWPOW Mining Algorithm</li>
  </ul>

  <p>The algorithm is intended to address the centralization of mining caused by ASIC hardware. In the original X16R algorithm paper, the team behind the currency explains that the fixed order of ordinary hashing algorithms lends itself to the construction of ASIC miners.</p>
  <p>The initial X16R algorithm aimed to overcome this problem by constantly disrupting the ordering of the hashing algorithms – it uses the same algorithms used in X15 and SHA512, but the ordering of those algorithms was changed based on the hash of the previous block. Eventually it became economically viable for X16R ASIC's and the community decided to implement new algorithms to mitigate the unfair distribution of Ravencoin. The community has carried out 2 algorithm forks to date to mitigate the potential efficiency improvements of the ASIC miners equipment compared to over the counter consumer grade equipment.</p>
  <p>The current KAWPOW algorithm aims to overcome the problem of centralisation of mining by utilising over the counter graphic processing unit (GPU) memory and compute capabilities. This is intended to allow most consumer grade GPU hardware to mine Ravencoin. The KAWPOW algorithm was derived from ProgPOW and ethhash, with modifications, to improve the distribution of Ravencoin to everyone.</p>
  <p>No additional future algorithm forks are envisaged. Note that this may allow future ASIC development to proceed, albeit as there is a limited potential for ASIC efficiency gains compared to consumer grade hardware, we are resistant to this form of centralisation.</p>

  <h3>Unique Characteristics</h3>
  <div class="rvn-badge-grid">
    <div class="rvn-badge-card">
      <h4>ASIC Resistant</h4>
      <p>Uses the KAWPOW hashing algorithm to utilize consumer GPU memory metrics and discourage corporate centralization.</p>
    </div>
    <div class="rvn-badge-card">
      <h4>Fair Launch</h4>
      <p>Everyone has equal opportunity to mine or purchase RVN since day one with absolute historical parity.</p>
    </div>
    <div class="rvn-badge-card">
      <h4>Zero Allocation</h4>
      <p>No pre-mine, no ICO pools, and absolutely no coins held back for developer allocations or developer foundation rewards.</p>
    </div>
    <div class="rvn-badge-card">
      <h4>Open Source Architecture</h4>
      <p>Entirely community-driven development framework running public cryptographic layers open to all global engineers.</p>
    </div>
  </div>

  <p style="margin-top: 40px; text-align: center;"><a href="https://medium.com/@ravencoin/ravencoin-4683cd00f83c" target="_blank" style="color: #FF5A1F; font-weight: 600; text-decoration: none;">Read the Foundation Announcement on Medium →</a></p>
</div>