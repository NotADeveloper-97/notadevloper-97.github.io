---
layout: page-w-banner
title: Whitepaper
bannerTitle: Whitepaper
bannerImage: /assets/img/pages/whitepaper/whitepaper-banner.jpg
permalink: /whitepaper/
---

<style>
  .rvn-wp-wrap {
    font-family: 'Inter', sans-serif;
    max-width: 900px;
    margin: 0 auto;
    padding: 60px 24px;
    text-align: center;
  }
  .rvn-wp-wrap h2 {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 32px;
    color: #090B11;
    margin-bottom: 8px;
  }
  .rvn-wp-wrap p#pub {
    color: #94A3B8;
    font-size: 14px;
    margin-bottom: 32px;
  }
  .rvn-wp-wrap p#pub a {
    color: #3B52C6;
    text-decoration: none;
    font-weight: 600;
  }
  
  /* Lang Selectors Matrix */
  .lang-bar {
    display: inline-flex;
    background: rgba(9, 11, 17, 0.04);
    border: 1px solid rgba(9, 11, 17, 0.05);
    padding: 6px;
    border-radius: 999px;
    gap: 8px;
    margin-bottom: 56px;
  }
  .lang-bar button {
    background: transparent;
    border: none;
    padding: 8px 18px;
    border-radius: 999px;
    cursor: pointer;
    transition: all 0.2s ease;
    display: flex;
    align-items: center;
  }
  .lang-bar button:hover {
    background: #FFFFFF;
    box-shadow: 0 4px 10px rgba(0,0,0,0.05);
  }
  .lang-bar img {
    height: 20px;
    width: auto;
  }

  /* Document Cards Matrix Grid */
  .wp-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 24px;
    text-align: left;
  }
  @media(max-width: 640px) { .wp-grid { grid-template-columns: 1fr; } }
  
  .wp-card {
    background: #FFFFFF;
    border: 1px solid rgba(17, 24, 39, 0.05);
    border-radius: 20px;
    padding: 32px;
    display: flex;
    flex-direction: column;
    box-shadow: 0 4px 6px -1px rgba(15, 23, 42, 0.02);
    transition: all 0.2s ease;
  }
  .wp-card:hover {
    transform: translateY(-4px);
    box-shadow: 0 12px 24px -8px rgba(15, 23, 42, 0.08);
    border-color: rgba(255, 90, 31, 0.25);
  }
  .wp-icon-shape {
    width: 54px;
    height: 54px;
    border-radius: 12px;
    background: rgba(255, 90, 31, 0.08);
    color: #FF5A1F;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-bottom: 24px;
  }
  .wp-card h3 {
    font-family: 'Space Grotesk', sans-serif;
    font-size: 20px;
    margin: 0 0 10px 0;
  }
  .wp-card h3 a {
    color: #090B11;
    text-decoration: none;
  }
  .wp-card p {
    font-size: 14px;
    color: #4B5563;
    line-height: 1.5;
    margin: 0;
    flex-grow: 1;
  }
</style>

<div class="rvn-wp-wrap">
  <h2 id="intro">Be Informed, Stay Involved</h2>
  <p id="pub">Documents published by <a href="https://www.linkedin.com/in/brucefenton/" target="_blank" rel="noopener">Bruce Fenton</a>, <a href="https://www.linkedin.com/in/tron-black-90287/" target="_blank" rel="noopener">Tron Black</a>, and <a href="https://www.linkedin.com/in/joelweight/" target="_blank" rel="noopener">Joel Weight</a>[cite: 17].</p>
  
  <div class="lang-bar">
    <button id="English" onClick="changeTextEnglish()"><img src="/assets/img/pages/whitepaper/English.png" alt="English selection flag" /></button>
    <button id="German" onClick="changeTextGerman()"><img src="/assets/img/pages/whitepaper/German.png" alt="German selection flag" /></button>
  </div>

  <div class="wp-grid">
    <!-- White Paper -->
    <div class="wp-card">
      <div class="wp-icon-shape"><i class="zmdi zmdi-file-text text-2xl"></i></div>
      <h3><a id="whitePaper1" href="/assets/documents/Ravencoin.pdf" target="_blank">White paper</a></h3>
      <p id="whitePaper2">Ravencoin: A Peer to Peer Electronic System for the Creation and Transfer of Assets[cite: 17]</p>
    </div>

    <!-- X16R Algorithm Paper -->
    <div class="wp-card">
      <div class="wp-icon-shape"><i class="zmdi zmdi-file-text text-2xl"></i></div>
      <h3><a id="x16r1" href="/assets/documents/X16R-Whitepaper.pdf" target="_blank">X16R algorithm paper</a></h3>
      <p id="x16r2">X16R: ASIC Resistant by Design[cite: 17]</p>
    </div>

    <!-- Development Roadmap -->
    <div class="wp-card">
      <div class="wp-icon-shape"><i class="zmdi zmdi-map text-2xl"></i></div>
      <h3><a id="roadMap1" href="https://github.com/RavenProject/Ravencoin/tree/master/roadmap" target="_blank">Development roadmap</a></h3>
      <p id="roadMap2">Development roadmap[cite: 17]</p>
    </div>

    <!-- Markdown Target -->
    <div id="roadMapMD" class="wp-card">
      <div class="wp-icon-shape"><i class="zmdi zmdi-github text-2xl"></i></div>
      <h3><a href="https://github.com/RavenProject/Ravencoin/tree/master/whitepaper" target="_blank">Markdown Version</a></h3>
      <p id="roadMapMD4">Markdown version of the Ravencoin white papers[cite: 17].</p>
    </div>
  </div>
</div>

<script type="text/javascript">
  function changeTextEnglish()
  {
    document.getElementById('intro').innerHTML = 'Be Informed, Stay Involved';
    document.getElementById('pub').innerHTML = 'Documents published by <a href="https://www.linkedin.com/in/brucefenton/" target="_blank">Bruce Fenton</a>, <a href="https://www.linkedin.com/in/tron-black-90287/" target="_blank">Tron Black</a>, and <a href="https://www.linkedin.com/in/joelweight/" target="_blank">Joel Weight</a>.';
    document.getElementById('whitePaper0').href = "/assets/documents/Ravencoin.pdf";
    document.getElementById('whitePaper1').innerHTML = 'White paper';
    document.getElementById('whitePaper1').href = "/assets/documents/Ravencoin.pdf";
    document.getElementById('whitePaper2').innerHTML = 'Ravencoin: A Peer to Peer Electronic System for the Creation and Transfer of Assets';
    document.getElementById('x16r0').href = "/assets/documents/X16R-Whitepaper.pdf";
    document.getElementById('x16r1').innerHTML = 'X16R algorithm paper';
    document.getElementById('x16r1').href = "/assets/documents/X16R-Whitepaper.pdf";
    document.getElementById('x16r2').innerHTML = 'X16R: ASIC Resistant by Design'; 
    document.getElementById('roadMap0').href = "https://github.com/RavenProject/Ravencoin/tree/master/roadmap";
    document.getElementById('roadMap1').innerHTML = 'Development roadmap';
    document.getElementById('roadMap1').href = "https://github.com/RavenProject/Ravencoin/tree/master/roadmap";
    document.getElementById('roadMap2').innerHTML = 'Development roadmap';
    document.getElementById('roadMapMD').style.display = "flex";
  }
  function changeTextGerman()
  {
    document.getElementById('intro').innerHTML = 'Seien Sie Informiert, Bleiben Sie Dabei';
    document.getElementById('pub').innerHTML = 'Von <a href="https://www.linkedin.com/in/brucefenton/" target="_blank">Bruce Fenton</a>, <a href="https://www.linkedin.com/in/tron-black-90287/" target="_blank">Tron Black</a>, und <a href="https://www.linkedin.com/in/joelweight/" target="_blank">Joel Weight</a> veröffentlichte Dokumente..';
    document.getElementById('whitePaper1').innerHTML = 'Weißbuch';
    document.getElementById('whitePaper1').href = "/assets/documents/Ravencoin.German.pdf";
    document.getElementById('whitePaper2').innerHTML = 'Ravencoin: Ein elektronisches Peer-to-Peer-System für die Erstellung und Übertragung von Assets';
    document.getElementById('x16r1').innerHTML = 'X16R Algorithmusentwurf';
    document.getElementById('x16r1').href = "/assets/documents/X16R-Whitepaper.German.pdf";
    document.getElementById('x16r2').innerHTML = 'X16R: ASIC-beständig durch Design';
    document.getElementById('roadMap1').innerHTML = 'Ravencoin Fahrplan';
    document.getElementById('roadMap1').href = "/assets/documents/Roadmap.German.pdf";
    document.getElementById('roadMap2').innerHTML = 'Ravencoin Fahrplan';
    document.getElementById('roadMapMD').style.display = "none";
  }
</script>