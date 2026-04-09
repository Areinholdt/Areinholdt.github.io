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
  

  /* PHOTO GALLERY */
  .gallery-label {
    font-size: 13px; letter-spacing:.3em; text-transform:uppercase; color:var(--accent);
    margin-bottom:2rem; display:flex; align-items:center; gap:.8rem;
  }
  .gallery-label::after { content:''; flex:1; height:1px; background:var(--border); max-width:160px; }
  .gallery {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    grid-auto-rows: 220px;
    gap: 0.8rem;
    margin-bottom: 5rem;
  }
  .gallery-item {
    background: var(--bg-card);
    border: 1px solid var(--border);
    overflow: hidden;
    position: relative;
  }
  .gallery-item.wide { grid-column: span 2; }
  .gallery-item img { width:100%; height:100%; object-fit:cover; display:block; filter: brightness(0.85) saturate(0.85); transition: filter 0.3s; }
  .gallery-item:hover img { filter: brightness(0.95) saturate(0.95); }
  .gallery-item-label {
    position: absolute; bottom:.6rem; left:.8rem;
    font-size: 10px; letter-spacing:.12em; color:var(--ink-muted);
    text-transform: uppercase; background: rgba(5,13,24,0.65); padding:.15rem .4rem;
  }
  .img-empty {
    width:100%;height:100%;display:flex;align-items:center;justify-content:center;
    flex-direction:column;gap:.5rem;color:var(--ink-faint);font-size:10px;letter-spacing:.1em;
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
        I am a bioinformatics scientist with a passion for Arctic marine biology and genomics.
        My research focuses on how Arctic and deep-sea fish, whales and elasmobranchs survive extreme cold, darkness,
        and high pressure --- by studying not just the genes that code for proteins,
        but the 98% of the genome that most studies ignore entirely.
      </p>

      <blockquote>
        <p>"During an Arctic research expedition, I held a rare deep-sea anglerfish in my hands.
        Its bizarre appearance and intact light organ left me fascinated me deeply. That encounter sparked
        my ambition to understand how species survive and adapt to extreme environments."</p>
      </blockquote>

      <p>
        With a background spanning fieldwork at sea, clean-lab DNA work, and large-scale
        computational analysis, I bridge the ocean and the terminal. I have participated in
        Arctic fish and marine mammal surveys, led seal-handling expeditions, and worked 
        extensively with marine mammals in both field and post-mortem settings.
        My experience includes whale necropsies, biopsy sampling, and photo-identification of beaked whales.
        In addition, I am proficient in identifying Arctic fish and shark taxa,
        combining hands-on field expertise with genomic research to better
        understand adaptation in extreme environments.
      </p>
      <p>
        My bioinformatics background covers population genomics, variant calling, phylogenetics,
        and AI-driven analyses. I previously worked as an IT consultant, where I
        applied data engineering and workflow automation to industrial problems --- skills I now
        bring back to evolutionary biology.
      </p>

      <div class="stat-row">
        <div><span class="stat-num">12+</span><span class="stat-label">Months Sea & Expedition time</span></div>
        <div><span class="stat-num">3</span><span class="stat-label">Research vessels</span></div>
        <div><span class="stat-num">1</span><span class="stat-label">Best poster award</span></div>
      </div>
    </div>
  </div>

  <!-- PHOTO GALLERY -->
  <div class="gallery-label">Field &amp; lab</div>
  <div class="gallery">
    <div class="gallery-item wide">
      <!-- <img src="/images/TVA-kaskelothvalen.jpg" alt="Sperm whale stranding"> -->
      <div class="img-empty">
        <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="0.8" opacity="0.4"><path d="M3 12c0 0 2-6 9-6s9 6 9 6-2 6-9 6-9-6-9-6z"/><circle cx="12" cy="12" r="2"/></svg>
        <span>TVA-kaskelothvalen.jpg — paste image path here</span>
      </div>
      <span class="gallery-item-label">Sperm whale · Danish waters · Feb 2026</span>
    </div>
    <div class="gallery-item">
      <div class="img-empty">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="0.8" opacity="0.4"><path d="M22 16.92v3a2 2 0 0 1-2.18 2 19.79 19.79 0 0 1-8.63-3.07A19.5 19.5 0 0 1 4.69 12 19.79 19.79 0 0 1 1.61 3.41 2 2 0 0 1 3.6 1.22h3a2 2 0 0 1 2 1.72c.127.96.361 1.903.7 2.81a2 2 0 0 1-.45 2.11L7.91 8.6A16 16 0 0 0 12 12.69a16 16 0 0 0 4.09 3.91l.94-.94a2 2 0 0 1 2.11-.45c.907.339 1.85.573 2.81.7A2 2 0 0 1 24 18z"/></svg>
        <span>R/V Tarajoq · Arctic survey</span>
      </div>
      <span class="gallery-item-label">GINR · Davis Strait</span>
    </div>
    <div class="gallery-item">
      <div class="img-empty">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="0.8" opacity="0.4"><path d="M3 9l9-7 9 7v11a2 2 0 0 1-2 2H5a2 2 0 0 1-2-2z"/><polyline points="9 22 9 12 15 12 15 22"/></svg>
        <span>Whitehead Lab · Gully MPA</span>
      </div>
      <span class="gallery-item-label">Dalhousie · Jul 2024</span>
    </div>
    <div class="gallery-item">
      <div class="img-empty">
        <svg width="24" height="24" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="0.8" opacity="0.4"><circle cx="12" cy="12" r="10"/><polyline points="12 6 12 12 16 14"/></svg>
        <span>Anholt Island · Seal expedition</span>
      </div>
      <span class="gallery-item-label">Field leadership · Jul 2023</span>
    </div>
    <div class="gallery-item wide">
      <div class="img-empty">
        <svg width="28" height="28" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="0.8" opacity="0.4"><rect x="2" y="3" width="20" height="14" rx="2"/><path d="M8 21h8M12 17v4"/></svg>
        <span>Lab work · Globe Institute, UCPH</span>
      </div>
      <span class="gallery-item-label">Copenhagen · 2022–2025</span>
    </div>
  </div>

  <!-- SKILLS -->
  <div class="gallery-label">Skills &amp; tools</div>
  <div class="skills-grid">
    <div class="skill-card">
      <h4>Programming</h4>
      <p>Python · R · SQL · JavaScript · Bash · AWS · Workflow automation</p>
    </div>
    <div class="skill-card">
      <h4>Bioinformatics</h4>
      <p>Population genomics · Variant calling · Phylogenetics · dN/dS · AlphaFold3 · FoldSeek</p>
    </div>
    <div class="skill-card">
      <h4>Machine learning</h4>
      <p>Deep learning for non-coding DNA · PhastCons · phyloHMM · AI-based fisheries tools</p>
    </div>
    <div class="skill-card">
      <h4>Laboratory</h4>
      <p>DNA extraction · Sequencing prep · Clean-lab procedures · PacBio / Hi-C pipelines</p>
    </div>
    <div class="skill-card">
      <h4>Fieldwork</h4>
      <p>Biopsy collection · Marine mammal handling · Trawl surveys · Expedition leadership</p>
    </div>
    <div class="skill-card">
      <h4>Communication</h4>
      <p>Conference speaker · Guest lecturer · Science journalist · Board member DMMS</p>
    </div>
  </div>

</div>
