---
layout: page-w-banner
title: Assets
bannerTitle: A Guide to Ravencoin Assets
bannerImage: /assets/img/pages/about/about-banner.jpg
permalink: /assets/
---

<style>
  .rvn-asset-doc {
    font-family: 'Inter', sans-serif;
    color: #111827;
    max-width: 1000px;
    margin: 0 auto;
    padding: 60px 24px;
  }
  .rvn-asset-doc h2, .rvn-asset-doc h3, .rvn-asset-doc h4 {
    font-family: 'Space Grotesk', sans-serif;
    letter-spacing: -0.01em;
    color: #090B11;
  }
  .rvn-asset-doc h2 { font-size: 32px; margin-top: 50px; border-bottom: 1px solid #ECEEF1; padding-bottom: 8px; }
  .rvn-asset-doc h3 { font-size: 22px; margin-top: 36px; color: #3B52C6; }
  .rvn-asset-doc h4 { font-size: 16px; margin-top: 20px; color: #FF5A1F; }
  .rvn-asset-doc p { line-height: 1.6; color: #4B5563; }
  .rvn-asset-doc ul { padding-left: 20px; line-height: 1.6; }
  
  /* Modern Data Tables Architecture */
  .rvn-matrix {
    width: 100%;
    border-collapse: collapse;
    margin: 20px 0 32px;
    background: #FFFFFF;
    border: 1px solid rgba(17, 24, 39, 0.08);
    border-radius: 8px;
    overflow: hidden;
    box-shadow: 0 4px 6px -1px rgba(15, 23, 42, 0.02);
  }
  .rvn-matrix th, .rvn-matrix td {
    padding: 14px 18px;
    text-align: left;
    font-size: 14px;
  }
  .rvn-matrix th {
    background: #090B11;
    color: #FFFFFF;
    font-family: 'Space Grotesk', sans-serif;
    font-weight: 600;
  }
  .rvn-matrix tr {
    border-bottom: 1px solid rgba(17, 24, 39, 0.05);
  }
  .rvn-matrix tr:last-child {
    border-bottom: none;
  }
  .rvn-matrix td:first-child {
    font-weight: 600;
    color: #111827;
    width: 25%;
    background: #FAFBFC;
  }
  .rvn-matrix td:last-child {
    font-family: 'IBM Plex Mono', monospace;
    color: #3B52C6;
  }
  .rvn-matrix-burn td:last-child {
    font-family: 'IBM Plex Mono', monospace !important;
    color: #111827 !important;
  }
</style>

<div class="rvn-asset-doc">
  <h2>All About Assets</h2>
  <p>This page is a work in progress. While almost all of the information is correct, there may be some nuance that is overlooked. If you come across any problems or believe information needs to be corrected or added, please make a pull request on <a href="https://github.com/RavenProject/ravenproject.github.io">this website's github source</a> or visit us at our <a href="https://discord.com/invite/jn6uhur">discord server</a>.</p>
  <p>This webpage will attempt to cover all aspects of Ravencoin assets from what they are to their on-chain encodings. As you read on, this document will become increasingly technical.</p>

  <h2>Table of Contents</h2>
  <ul>
    <li><a href="#what_is_an_asset">What is an asset?</a></li>
    <li><a href="#where_can_i_trade_assets">Where can I trade assets?</a></li>
    <li><a href="#privacy">Privacy and Access</a></li>
    <li><a href="#the_jargon">The Jargon</a></li>
    <li><a href="#creating_assets">Creating Assets</a></li>
    <li><a href="#what_is_on_chain">What is on the chain?</a></li>
    <li><a href="#burn_addresses">Burn Addresses</a></li>
    <li><a href="#scripts">Standard Asset Scripts</a></li>
    <li><a href="#create_transactions">Building Asset Transactions</a></li>
  </ul>

  <h3 id="what_is_an_asset">What is an asset?</h3>
  <p>A Ravencoin asset (also less commonly referred to as a token) is an on-chain way of creating, storing, and transfering custom end-user generated information. Assets come with a unique, user-chosen name which can allow for assets to be verified by name only and metadata. Ravencoin users have created assets to make their own 'coin', sell digital art, real estate, gem stones, security tokens, wine futures, and even incorporated it as an in-video game currency.</p>

  <h3 id="where_can_i_trade_assets">Where can I trade assets?</h3>
  <p><a href="https://raventrader.net/">Raven Trader</a> is a on-chain peer to peer market which utilises RIP-15 for users to post half-signed atomic swaps. There are also asset markets such as <a href="https://www.rvnft.art/">RVNFT</a> and <a href="https://rvnbay.com/">RVNBay</a>. In addition, one can pay for a listing at <a href="https://cryptosx.io/">Cryptosx</a> for security tokens or OKEX for regular tokens.</p>

  <h3 id="privacy">Privacy and Access</h3>
  <p>A common question about assets is who can see whats on an asset and is there any way to limit viewership of the asset to a recipient. The simple answer is that anyone is able to see the data associated with an asset, however there are protocols (see RIP-10, RIP-11, and RIP-14) that allow for the encryption of IPFS data such that only a recipient of an asset may view it.</p>

  <h2 id="the_jargon">The Jargon</h2>
  <ul>
    <li><h4>Reissuability</h4><p>This is a metadata flag that denotes whether or not an asset can be reissued. Once this flag is set to false it CANNOT be changed back! If you want to change your asset's information in the future, ensure that your asset is reissuable when you create it.</p></li>
    <li><h4>Divisibility (Units)</h4><p>Units is a metadata value from zero to eight that denotes how much an asset can be broken up. Specifically this number is how many digits past the decimal this asset can be divided into (a minimum size of 10<sup>-d</sup> where d is the divisibility). Units=0 means whole tokens only. Units=8 is the most divisible and allows tokens to be transferred in increments of 0.00000001.</p></li>
    <li><h4>Reissuing</h4><p>Reissuing an asset modifies metadata or increases circulating supply. Divisibility updates can only increase, never decrease.</p></li>
    <li><h4>Ownership Assets</h4><p>When creating assets, you receive an ownership token marked with an exclamation point (!). Holding <code>ASSET!</code> grants exclusive structural administrative access over <code>ASSET</code> architectures.</p></li>
  </ul>

  <h2 id="creating_assets">Creating Assets</h2>
  <p>Assets cannot be differentiated against one another except through their names. This means that all asset names must be unique; an asset creation will not be accepted by the chain if the name is not unique. Names are encoded via ASCII constraints using the latin alphabet.</p>

  <h4>Ownership Asset Configurations</h4>
  <table class="rvn-matrix">
    <thead><tr><th>Metadata</th><th>Configuration Requirements</th></tr></thead>
    <tbody>
      <tr><td>Asset Name</td><td>Base asset name + '!'</td></tr>
      <tr><td>Ownership Asset</td><td>No associated ownership asset</td></tr>
      <tr><td>Prerequisites</td><td>Created natively with main base asset</td></tr>
      <tr><td>Asset Amount</td><td>Strictly 1 unit immutable allocation</td></tr>
      <tr><td>Cost</td><td>Generated alongside base generation asset</td></tr>
      <tr><td>Reissuability</td><td>False (Cannot be reissued)</td></tr>
      <tr><td>Divisibility</td><td>0 (Non-divisible structural token)</td></tr>
      <tr><td>Associated Data</td><td>No data strings permitted</td></tr>
    </tbody>
  </table>

  <h3 id="the_big_three">The Big Three</h3>
  
  <h4>Main Assets</h4>
  <table class="rvn-matrix">
    <thead><tr><th>Metadata</th><th>Configuration Requirements</th></tr></thead>
    <tbody>
      <tr><td>Asset Name</td><td>3-30 capital characters. ('.', '_' allowed inline; RVN, RAVEN, RAVENCOIN reserved)</td></tr>
      <tr><td>Ownership Asset</td><td>Generates distinct management token (!)</td></tr>
      <tr><td>Prerequisites</td><td>None</td></tr>
      <tr><td>Asset Amount</td><td>1 to 21,000,000,000 global cap options</td></tr>
      <tr><td>Cost</td><td>500 RVN standard baseline fee</td></tr>
      <tr><td>Reissuability</td><td>Configurable True/False parameters</td></tr>
      <tr><td>Divisibility</td><td>Variable matrix constraints 0 through 8</td></tr>
      <tr><td>Associated Data</td><td>Supports 32-byte cryptographic hashes (IPFS)</td></tr>
    </tbody>
  </table>

  <h4>Sub-Assets</h4>
  <table class="rvn-matrix">
    <thead><tr><th>Metadata</th><th>Configuration Requirements</th></tr></thead>
    <tbody>
      <tr><td>Asset Name</td><td>[main asset]/[sub-portion]. Full length must be <= 30 characters.</td></tr>
      <tr><td>Ownership Asset</td><td>Generates sub-management token (!)</td></tr>
      <tr><td>Prerequisites</td><td>Parent main asset ownership token (!) verification</td></tr>
      <tr><td>Asset Amount</td><td>1 to 21,000,000,000 allocation spans</td></tr>
      <tr><td>Cost</td><td>100 RVN configuration fee</td></tr>
      <tr><td>Reissuability</td><td>Configurable True/False parameters</td></tr>
      <tr><td>Divisibility</td><td>Variable matrix constraints 0 through 8</td></tr>
      <tr><td>Associated Data</td><td>Supports 32-byte cryptographic hashes (IPFS)</td></tr>
    </tbody>
  </table>

  <h4>Unique Assets</h4>
  <table class="rvn-matrix">
    <thead><tr><th>Metadata</th><th>Configuration Requirements</th></tr></thead>
    <tbody>
      <tr><td>Asset Name</td><td>[parent name]#[unique portion]. Full length must be <= 30 characters.</td></tr>
      <tr><td>Ownership Asset</td><td>None</td></tr>
      <tr><td>Prerequisites</td><td>Parent asset ownership token (!) verification</td></tr>
      <tr><td>Asset Amount</td><td>Strictly capped at 1 unique token unit</td></tr>
      <tr><td>Cost</td><td>5 RVN deployment allocation fee</td></tr>
      <tr><td>Reissuability</td><td>False (Permanently immutable)</td></tr>
      <tr><td>Divisibility</td><td>0 (Strict integer unit execution)</td></tr>
      <tr><td>Associated Data</td><td>Supports 32-byte cryptographic hashes (IPFS)</td></tr>
    </tbody>
  </table>

  <h3 id="broadcasts_and_messages">Message Channels</h3>
  <table class="rvn-matrix">
    <thead><tr><th>Metadata</th><th>Configuration Requirements</th></tr></thead>
    <tbody>
      <tr><td>Asset Name</td><td>[parent name]~[channel name]. Sub-portion max 12 characters.</td></tr>
      <tr><td>Ownership Asset</td><td>None</td></tr>
      <tr><td>Prerequisites</td><td>Parent asset ownership token (!) verification</td></tr>
      <tr><td>Asset Amount</td><td>Strictly capped at 1 structural token unit</td></tr>
      <tr><td>Cost</td><td>100 RVN routing deployment fee</td></tr>
      <tr><td>Reissuability</td><td>False (Permanently immutable)</td></tr>
      <tr><td>Divisibility</td><td>0 (Strict integer unit execution)</td></tr>
      <tr><td>Associated Data</td><td>Disabled at baseline creation levels</td></tr>
    </tbody>
  </table>

  <h3 id="qualifiers_restricted_tags">Administrative & Restricted Assets</h3>
  
  <h4>Qualifier Assets</h4>
  <table class="rvn-matrix">
    <thead><tr><th>Metadata</th><th>Configuration Requirements</th></tr></thead>
    <tbody>
      <tr><td>Asset Name</td><td>#[qualifier portion]. Capitalization logic matches main parameters.</td></tr>
      <tr><td>Ownership Asset</td><td>None</td></tr>
      <tr><td>Prerequisites</td><td>None</td></tr>
      <tr><td>Asset Amount</td><td>1 to 10 administrative token ranges</td></tr>
      <tr><td>Cost</td><td>1000 RVN protocol deployment allocation fee</td></tr>
      <tr><td>Reissuability</td><td>False (Permanently immutable)</td></tr>
      <tr><td>Divisibility</td><td>0 (Strict integer unit execution)</td></tr>
      <tr><td>Associated Data</td><td>Supports immutable fixed 32-byte hashes</td></tr>
    </tbody>
  </table>

  <h4>Restricted Assets</h4>
  <table class="rvn-matrix">
    <thead><tr><th>Metadata</th><th>Configuration Requirements</th></tr></thead>
    <tbody>
      <tr><td>Asset Name</td><td>$[restricted portion]. Capitalization logic matches main parameters.</td></tr>
      <tr><td>Ownership Asset</td><td>Generates custom validation ownership tokens (!)</td></tr>
      <tr><td>Prerequisites</td><td>Valid associated administrative layer qualifiers</td></tr>
      <tr><td>Asset Amount</td><td>1 to 21,000,000,000 global cap options</td></tr>
      <tr><td>Cost</td><td>1500 RVN network deployment fee</td></tr>
      <tr><td>Reissuability</td><td>True (Configurable operational structure checks)</td></tr>
      <tr><td>Divisibility</td><td>Variable matrix constraints 0 through 8</td></tr>
      <tr><td>Associated Data</td><td>Supports full updateable 32-byte hashes</td></tr>
    </tbody>
  </table>

  <h2 id="burn_addresses">Network Asset Burning Addresses</h2>
  <table class="rvn-matrix rvn-matrix-burn">
    <thead>
      <tr>
        <th>Operation Type</th>
        <th>Mainnet Operational Address</th>
        <th>Testnet Address</th>
        <th>Burn Fee</th>
      </tr>
    </thead>
    <tbody>
      <tr><td>Issue Main Asset</td><td>RXissueAssetXXXXXXXXXXXXXXXXXhhZGt</td><td>n1issueAssetXXXXXXXXXXXXXXXXWdnemQ</td><td>500 RVN</td></tr>
      <tr><td>Reissue Configuration</td><td>RXReissueAssetXXXXXXXXXXXXXXVEFAWu</td><td>n1ReissueAssetXXXXXXXXXXXXXXWG9NLd</td><td>100 RVN</td></tr>
      <tr><td>Issue Sub-Asset</td><td>RXissueSubAssetXXXXXXXXXXXXXWcwhwL</td><td>n1issueSubAssetXXXXXXXXXXXXXbNiH6v</td><td>100 RVN</td></tr>
      <tr><td>Issue Unique Asset</td><td>RXissueUniqueAssetXXXXXXXXXXWEAe58</td><td>n1issueUniqueAssetXXXXXXXXXXS4695i</td><td>5 RVN</td></tr>
      <tr><td>Issue Message Channel</td><td>RXissueMsgChanneLAssetXXXXXXSjHvAY</td><td>n1issueMsgChanneLAssetXXXXXXT2PBdD</td><td>100 RVN</td></tr>
      <tr><td>Issue Qualifier</td><td>RXissueQuaLifierXXXXXXXXXXXXUgEDbC</td><td>n1issueQuaLifierXXXXXXXXXXXXUysLTj</td><td>1000 RVN</td></tr>
      <tr><td>Issue Restricted Asset</td><td>RXissueRestrictedXXXXXXXXXXXXzJZ1q</td><td>n1issueRestrictedXXXXXXXXXXXXZVT9V</td><td>1500 RVN</td></tr>
      <tr><td>Add Address Tag Check</td><td>RXaddTagBurnXXXXXXXXXXXXXXXXZQm5ya</td><td>n1addTagBurnXXXXXXXXXXXXXXXXX5oLMH</td><td>0.1 RVN</td></tr>
    </tbody>
  </table>
</div>