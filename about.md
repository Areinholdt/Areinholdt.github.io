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

  <!-- ANGLERFISH DIVIDER -->
<div style="width:100%;margin:2rem 0 4rem;display:flex;justify-content:center;align-items:center;">
  <svg width="100%" viewBox="0 0 800 300" xmlns="http://www.w3.org/2000/svg">
    <!-- depth atmosphere -->
    <rect width="800" height="300" fill="#020c1e"/>
    <!-- marine snow particles -->
    <circle cx="60" cy="80" r="1.2" fill="#4da6e0" opacity="0.4"><animate attributeName="opacity" values="0.2;0.7;0.2" dur="4s" repeatCount="indefinite"/></circle>
    <circle cx="740" cy="120" r="0.9" fill="#3ecfb0" opacity="0.4"><animate attributeName="opacity" values="0.1;0.6;0.1" dur="3.2s" repeatCount="indefinite"/></circle>
    <circle cx="150" cy="200" r="1.4" fill="#8fd4f5" opacity="0.3"><animate attributeName="opacity" values="0.1;0.5;0.1" dur="5s" repeatCount="indefinite"/></circle>
    <circle cx="650" cy="240" r="1" fill="#4da6e0" opacity="0.35"><animate attributeName="opacity" values="0.2;0.6;0.2" dur="3.8s" repeatCount="indefinite"/></circle>
    <circle cx="400" cy="40" r="0.8" fill="#3ecfb0" opacity="0.3"><animate attributeName="opacity" values="0.1;0.5;0.1" dur="4.5s" repeatCount="indefinite"/></circle>
    <circle cx="200" cy="260" r="1.1" fill="#8fd4f5" opacity="0.25"><animate attributeName="opacity" values="0.1;0.4;0.1" dur="6s" repeatCount="indefinite"/></circle>
    <circle cx="580" cy="60" r="1.3" fill="#4da6e0" opacity="0.3"><animate attributeName="opacity" values="0.2;0.5;0.2" dur="4.2s" repeatCount="indefinite"/></circle>
    <!-- body -->
    <ellipse cx="400" cy="170" rx="140" ry="85" fill="#040f22" stroke="#0d3060" stroke-width="0.8"/>
    <ellipse cx="400" cy="165" rx="112" ry="66" fill="none" stroke="#0a2548" stroke-width="0.5" opacity="0.6"/>
    <!-- jaw -->
    <path d="M275,182 Q310,230 400,222 Q490,230 525,182" fill="#030c1e" stroke="#0d3060" stroke-width="0.8"/>
    <!-- teeth -->
    <line x1="295" y1="183" x2="288" y2="218" stroke="#7ab8d4" stroke-width="1.2" opacity="0.7"/>
    <line x1="316" y1="189" x2="311" y2="224" stroke="#7ab8d4" stroke-width="1.2" opacity="0.7"/>
    <line x1="340" y1="194" x2="337" y2="228" stroke="#7ab8d4" stroke-width="1.2" opacity="0.7"/>
    <line x1="366" y1="197" x2="364" y2="230" stroke="#7ab8d4" stroke-width="1.2" opacity="0.7"/>
    <line x1="400" y1="198" x2="400" y2="231" stroke="#7ab8d4" stroke-width="1.2" opacity="0.7"/>
    <line x1="434" y1="197" x2="436" y2="230" stroke="#7ab8d4" stroke-width="1.2" opacity="0.7"/>
    <line x1="460" y1="194" x2="463" y2="228" stroke="#7ab8d4" stroke-width="1.2" opacity="0.7"/>
    <line x1="484" y1="189" x2="489" y2="223" stroke="#7ab8d4" stroke-width="1.2" opacity="0.7"/>
    <line x1="505" y1="183" x2="512" y2="216" stroke="#7ab8d4" stroke-width="1.2" opacity="0.7"/>
    <!-- eye -->
    <circle cx="318" cy="158" r="22" fill="#020810" stroke="#1a4878" stroke-width="1"/>
    <circle cx="318" cy="158" r="14" fill="#010610"/>
    <circle cx="318" cy="158" r="20" fill="#4da6e0" opacity="0.06"><animate attributeName="opacity" values="0.03;0.12;0.03" dur="3s" repeatCount="indefinite"/></circle>
    <circle cx="323" cy="153" r="4" fill="rgba(143,212,245,0.6)"/>
    <circle cx="325" cy="151" r="1.5" fill="rgba(255,255,255,0.4)"/>
    <!-- fins -->
    <path d="M525,165 Q575,142 592,168 Q578,188 525,178Z" fill="#030e20" stroke="#0d3060" stroke-width="0.6" opacity="0.85"/>
    <path d="M275,165 Q225,145 210,170 Q224,190 275,178Z" fill="#030e20" stroke="#0d3060" stroke-width="0.6" opacity="0.85"/>
    <path d="M370,118 Q388,88 415,118" fill="none" stroke="#0d3060" stroke-width="0.7"/>
    <!-- tail -->
    <path d="M538,168 Q578,142 598,156 Q582,178 538,176Z" fill="#020c1c" stroke="#0d3060" stroke-width="0.5"/>
    <!-- lure stem -->
    <path d="M382,118 Q365,90 372,62 Q376,42 382,22" fill="none" stroke="#2a7ab0" stroke-width="2" opacity="0.9"/>
    <!-- lure glow layers -->
    <circle cx="382" cy="16" r="32" fill="#3ecfb0" opacity="0.06"><animate attributeName="opacity" values="0.03;0.12;0.03" dur="2.2s" repeatCount="indefinite"/></circle>
    <circle cx="382" cy="16" r="20" fill="#3ecfb0" opacity="0.12"><animate attributeName="opacity" values="0.06;0.22;0.06" dur="2.2s" repeatCount="indefinite"/></circle>
    <circle cx="382" cy="16" r="10" fill="#3ecfb0" opacity="0.6"><animate attributeName="opacity" values="0.4;0.9;0.4" dur="2.2s" repeatCount="indefinite"/></circle>
    <circle cx="382" cy="16" r="5" fill="#8ffff0"><animate attributeName="opacity" values="0.7;1;0.7" dur="2.2s" repeatCount="indefinite"/></circle>
    <!-- gill slits -->
    <path d="M355,155 Q349,168 351,180" fill="none" stroke="#0d3060" stroke-width="1.2" opacity="0.6"/>
    <path d="M363,152 Q357,166 359,178" fill="none" stroke="#0d3060" stroke-width="1.2" opacity="0.5"/>
    <!-- depth label -->
    <text x="400" y="285" text-anchor="middle" font-family="'Space Mono', monospace" font-size="9" fill="#2a4a6a" letter-spacing="4">MELANOCETUS JOHNSONII · HADAL ZONE · 1000–4000M</text>
  </svg>
</div>
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
    font-size: 10px;
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
    font-size: 10px; letter-spacing:.3em; text-transform:uppercase; color:var(--accent);
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
        <svg width="32" height="32" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="0.8" opacity="0.3"><path d="M20 21v-2a4 4 0 0 0-4-4H8a4 4 0 0 0-4 4v2"/><circle cx="12" cy="7" r="4"/></svg>
      </div>

    <div class="photo-accent">
        <img src="/images/angler_annika1.jpg" alt="Angler fish">
        <svg width="20" height="20" viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="0.8" opacity="0.3"><path d="M3 12c0 0 2-6 9-6s9 6 9 6-2 6-9 6-9-6-9-6z"/><circle cx="12" cy="12" r="2"/></svg>
        <span>Field photo</span>
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
