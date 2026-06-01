---
layout: default
title: About
permalink: /about/
---
<style>
  .about-wrap {
    max-width: 1100px;
    margin: 0 auto;
    padding: 9rem 4rem 6rem;
    position: relative;
    z-index: 1;
  }
  .about-top {
    display: grid;
    grid-template-columns: 1fr 1.6fr;
    gap: 5rem;
    align-items: start;
    margin-bottom: 5rem;
  }
  .photo-stack { position: relative; padding-bottom: 2rem; }
  .photo-main {
    width: 100%;
    aspect-ratio: 3/4;
    background: var(--bg-card);
    border: 1px solid var(--border);
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 0.6rem;
    color: var(--ink-faint);
    font-size: 11px;
    letter-spacing: 0.1em;
  }
  .photo-main img { width:100%; height:100%; object-fit:cover; display:block; filter: brightness(0.9) saturate(0.85); }
  .photo-accent {
    position: absolute;
    bottom: 0; right: -1.8rem;
    width: 52%;
    aspect-ratio: 1;
    background: var(--bg-surface);
    border: 1px solid var(--border);
    overflow: hidden;
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
    gap: 0.5rem;
    color: var(--ink-faint);
    font-size: 10px;
    letter-spacing: 0.1em;
  }
  .photo-accent img { width:100%; height:100%; object-fit:cover; display:block; filter: brightness(0.9); }
  .about-intro-label {
    font-size: 13px;
    letter-spacing: 0.3em;
    text-transform: uppercase;
    color: var(--accent);
    margin-bottom: 1.2rem;
    display: flex; align-items: center; gap: 0.7rem;
  }
  
  .about-intro-label::before { content:''; width:28px; height:1px; background:var(--accent); display:block; }
  .about-intro h1 {
    font-family: var(--serif);
    font-size: clamp(2.5rem, 4vw, 3.8rem);
    font-weight: 300;
    line-height: 1.1;
    color: var(--ink);
    margin-bottom: 1.8rem;
  }
  .about-intro h1 em { font-style: italic; color: var(--accent-bright); }
  .about-intro p {
    color: var(--ink-muted);
    font-size: 12.5px;
    line-height: 2.1;
    margin-bottom: 1.2rem;
  }
  blockquote {
    border-left: 2px solid var(--accent);
    padding: 1rem 1.5rem;
    margin: 2rem 0;
    background: var(--bg-card);
  }
  blockquote p {
    font-family: var(--serif);
    font-size: 1.1rem;
    font-style: italic;
    color: var(--ink);
    line-height: 1.7;
    margin: 0;
  }
  .stat-row {
    display: flex; gap: 2.5rem;
    margin-top: 2.5rem; padding-top: 2rem;
    border-top: 1px solid var(--border);
  }
  .stat-num { font-family: var(--serif); font-size: 2.2rem; color: var(--accent-bright); display:block; line-height:1; }
  .stat-label { font-size: 10px; letter-spacing: .15em; color: var(--ink-faint); text-transform: uppercase; margin-top: .4rem; display:block; }
  

  /* PHOTO GALLERY — REFINED */
  .gallery-label {
    font-size: 13px; letter-spacing:.3em; text-transform:uppercase; color:var(--accent);
    margin-bottom: 2.5rem; display:flex; align-items:center; gap:.8rem;
  }
  .gallery-label::after { content:''; flex:1; height:1px; background:var(--border); max-width:160px; }
  
  .gallery {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-rows: 260px;
    gap: 0.5rem;
    margin-bottom: 5rem;
  }
  
  .gallery-item {
    background: var(--bg-card);
    border: 1px solid var(--border);
    overflow: hidden;
    position: relative;
    transition: all 0.3s ease;
  }
  
  .gallery-item.wide { grid-column: span 2; }
  
  .gallery-item img {
    width: 100%;
    height: 100%;
    object-fit: cover;
    display: block;
    filter: brightness(0.82) saturate(0.9) contrast(1.05);
    transition: filter 0.4s ease;
  }
  
  .gallery-item:hover img {
    filter: brightness(0.9) saturate(1) contrast(1.08);
  }
  
  .gallery-item-label {
    position: absolute;
    bottom: 0;
    left: 0;
    right: 0;
    font-size: 11px;
    letter-spacing: 0.12em;
    color: var(--ink-faint);
    text-transform: uppercase;
    background: linear-gradient(to top, rgba(5,13,24,0.85), transparent);
    padding: 1.2rem 1rem 0.8rem 1rem;
    text-align: left;
  }
  /* SKILLS */
  .skills-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.2rem;
    margin-bottom: 5rem;
  }
  .skill-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    padding: 1.5rem;
  }
  .skill-card h4 {
    font-size: 10px; letter-spacing:.18em; text-transform:uppercase;
    color: var(--gold); margin-bottom:.8rem;
  }
  .skill-card p { font-size:11.5px; color:var(--ink-muted); line-height:1.9; }

  @media (max-width: 900px) {
    .about-wrap { padding: 8rem 1.5rem 4rem; }
    .about-top { grid-template-columns: 1fr; gap: 3rem; }
    .photo-accent { display: none; }
    .gallery { grid-template-columns: 1fr 1fr; }
    .gallery-item.wide { grid-column: span 2; }
    .skills-grid { grid-template-columns: 1fr 1fr; }
  }
</style>

<div class="about-wrap">
  <div class="about-top">
    <div class="photo-stack">
  <div class="photo-main">
    <img src="/images/portrait.jpg" alt="Annika Reinholdt">
  </div>
  <div style="margin-top:3.0rem; width:100%; overflow:hidden; border:1px solid var(--border);">
  <img src="/images/angler_annika.jpg" alt="Fieldwork" 
       style="width:100%; height:400px; object-fit:cover; object-position:center 20%;
              filter:brightness(1.1) saturate(1.1); display:block;">
</div>
</div>

    <div class="about-intro">
      <div class="about-intro-label">About me</div>
      <h1>Decoding life<br>in the <em>dark</em></h1>
      <p>
        I go to places most people will never see - and I bring 
        back the molecular secrets of the animals that live there.
      </p>
      
      <p>
       We have robots on Mars yet we barely have eyes on the deep sea - 
        the largest habitat on Earth, home to fish, sharks, skates 
        and whales living under crushing pressure, freezing cold, 
        and complete darkness. I am a scientist who goes there 
        to find out how.
      </p>

      <p>
        My name is Annika Reinholdt. I read the DNA of deep-sea 
        animals, combining ocean expeditions with computational 
        biology to understand how life thrives at the very 
        extremes of existence on Earth.
      </p>
      
      <blockquote>
          <p>"On a night shift during an Arctic expedition, a deep-sea 
              anglerfish came up in the trawl net. Its bioluminescent lure 
              was still glowing, from a world 1500 metres below. I held it 
              in my hands. I took a tissue sample. And I thought: whatever 
              survival looks like at that depth, it is written somewhere 
              in here. I am going to find it."</p>
      </blockquote>

      <p>
        Most genomic research has explored only 2% of the genome, 
        the part that codes for proteins. The other 98% acts like 
        a control panel, switching genes on and off and shaping 
        how animals survive. In deep-sea animals, that control panel 
        has been shaped by millions of years of evolution under 
        the most extreme conditions on Earth. Those adaptations 
        are written in the genome, waiting to be read. 
        Almost no one has looked there yet. 
        That is where my research begins.
      </p>
     
      <p>
        I have held the answers in my hands. 
        Now I am going to read them.
      </p>

      <div class="stat-row">
        <div><span class="stat-num">12+</span><span class="stat-label">Months Sea & Expedition time</span></div>
        <div><span class="stat-num">4</span><span class="stat-label">Collaborating institutions</span></div>
        <div><span class="stat-num">100+</span><span class="stat-label">Collected tissue samples</span></div>
      </div>
    </div>
  </div>

<!-- PHOTO GALLERY -->
  <div class="gallery-label">Deep Sea Species</div>
  <div class="gallery">
    <div class="gallery-item wide">
      <img src="/images/whale1.JPG" alt="Northern Bottlnose Whale"> 
      <span class="gallery-item-label">Photo 1</span>
    </div>
    <div class="gallery-item">
      <img src="/images/fish.jpg" alt="Photo 2"> 
      <span class="gallery-item-label">Large-eye snaggletooth</span>
    </div>
    <div class="gallery-item">
      <img src="/images/fish2.jpg" alt="Photo 3"> 
      <span class="gallery-item-label">Deep sea perch</span>
    </div>
    <div class="gallery-item">
      <img src="/images/whale1.JPG" alt="Northern Bottlnose Whale"> 
      <span class="gallery-item-label">Northern Bottlnose Whale</span>
    </div>
    <div class="gallery-item">
      <img src="/images/shark2.jpg" alt="Photo 5"> 
      <span class="gallery-item-label">Greenland shark</span>
    </div>
    <div class="gallery-item wide">
      <img src="/images/seal.jpg" alt="Photo 6"> 
      <span class="gallery-item-label">Harp seal</span>
    </div>
    <div class="gallery-item">
      <img src="/images/fish4.jpg" alt="Photo 7"> 
      <span class="gallery-item-label">Photo 7</span>
    </div>
  </div>

</div>
