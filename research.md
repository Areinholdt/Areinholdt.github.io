---
layout: default
title: Research
permalink: /research/
---
<style>
  .research-wrap {
    max-width: 1000px;
    margin: 0 auto;
    padding: 9rem 4rem 6rem;
    position: relative; z-index: 1;
  }
  .research-header { margin-bottom: 4rem; }
  .research-eyebrow {
    font-size: 10px; letter-spacing:.3em; text-transform:uppercase; color:var(--accent);
    margin-bottom:1rem; display:flex; align-items:center; gap:.8rem;
  }
  .research-eyebrow::before { content:''; width:28px; height:1px; background:var(--accent); display:block; }
  .research-header h1 {
    font-family: var(--font-serif);
    font-size: clamp(2.5rem, 4vw, 3.8rem);
    font-weight: 300; line-height:1.1; color:var(--ink); margin-bottom:1.2rem;
  }
  .research-header h1 em { font-style:italic; color:var(--accent-bright); }
  .research-header p { color:var(--ink-muted); font-size:12.5px; line-height:2.1; max-width:620px; }

  /* PROJECT CARDS */
  .project-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    padding: 2.8rem;
    margin-bottom: 1.5rem;
    display: grid;
    grid-template-columns: 70px 1fr;
    gap: 2rem;
    align-items: start;
    transition: border-color 0.25s;
  }
  .project-card:hover { border-color: var(--accent); }
  .project-num {
    font-family: var(--font-serif);
    font-size: 4rem; color:var(--ink-faint); line-height:1; font-weight:300;
  }
  .project-tag {
    font-size: 9px; letter-spacing:.18em; text-transform:uppercase;
    color: var(--accent); border: 1px solid var(--accent-glow);
    padding: .2rem .6rem; display:inline-block; margin-bottom:.8rem;
  }
  .project-card h2 {
    font-family: var(--font-serif);
    font-size: 1.7rem; font-weight:400; color:var(--ink); margin-bottom:.8rem; line-height:1.2;
  }
  .project-card p { color:var(--ink-muted); font-size:12.5px; line-height:2.1; margin-bottom:1rem; }
  .project-methods {
    display: flex; flex-wrap:wrap; gap:.5rem; margin-top:1rem;
  }
  .method-tag {
    font-size: 9.5px; letter-spacing:.1em; text-transform:uppercase;
    background: rgba(58,143,196,0.08); color:var(--ink-muted);
    border: 1px solid var(--border); padding:.2rem .55rem;
  }
  .project-collab {
    margin-top: 1.2rem; padding-top:1rem; border-top:1px solid var(--border);
    font-size: 11px; color:var(--ink-faint); letter-spacing:.05em;
  }
  .project-collab strong { color:var(--ink-muted); font-weight:400; }

  /* PUBLICATIONS */
  .pubs-section { margin-top: 5rem; }
  .pubs-label {
    font-size:10px; letter-spacing:.3em; text-transform:uppercase; color:var(--accent);
    margin-bottom:2rem; display:flex; align-items:center; gap:.8rem;
  }
  .pubs-label::after { content:''; flex:1; height:1px; background:var(--border); max-width:160px; }
  .pub-item {
    padding: 1.5rem 0; border-bottom: 1px solid var(--border);
    display: grid; grid-template-columns: 60px 1fr; gap: 1.5rem; align-items:start;
  }
  .pub-year { font-size:11px; color:var(--accent); letter-spacing:.1em; }
  .pub-title { font-family:var(--font-serif); font-size:1.1rem; font-weight:400; color:var(--ink); margin-bottom:.3rem; }
  .pub-journal { font-size:11.5px; color:var(--ink-muted); }
  .pub-status {
    display:inline-block; font-size:9px; letter-spacing:.15em; text-transform:uppercase;
    background: rgba(200,169,110,0.12); color:var(--gold);
    border:1px solid rgba(200,169,110,0.25); padding:.2rem .5rem; margin-left:.6rem;
  }

  @media (max-width:768px) {
    .research-wrap { padding:8rem 1.5rem 4rem; }
    .project-card { grid-template-columns:1fr; gap:1rem; padding:2rem; }
    .project-num { font-size:2.5rem; }
  }
</style>

<div class="research-wrap">
  <div class="research-header">
    <div class="research-eyebrow">Research</div>
    <h1>Deep, Dark<br>and <em>Cold</em></h1>
    <p>
      My work focuses on the genomic mechanisms that enable Arctic and deep-sea fish
      to survive extreme environments — combining comparative genomics, AI-based protein
      modelling, and deep learning on non-coding DNA to uncover adaptations invisible
      to conventional analysis.
    </p>
  </div>

  <!-- PROJECT 1 -->
  <div class="project-card">
    <div class="project-num">01</div>
    <div>
      <span class="project-tag">PhD Research · 2025–2028 · Active</span>
      <h2>Convergent Genomics of Arctic Marine Taxa</h2>
      <p>
        This project investigates how Arctic and deep-sea fish survive in extreme environments
        characterised by high pressure, near-zero temperatures, and complete darkness.
        A central question is whether unrelated species independently evolve the same
        genomic solutions — <em>convergent evolution</em> at the molecular level.
      </p>
      <p>
        Most genomic studies focus on protein-coding regions, which represent only ~2%
        of the genome. This project goes further by exploring the 98% "dark genome"
        — non-coding regulatory DNA that controls how and when genes are expressed.
        By integrating coding genes, non-coding elements, and protein structures,
        the project builds a comprehensive picture of adaptation to one of Earth's
        most extreme environments.
      </p>
      <p>
        The dataset will include 15–20 deep-sea species genomes alongside shallow-water
        relatives, combining existing high-quality assemblies with newly sequenced Arctic
        taxa generated using PacBio/Hi-C pipelines at the Yggdrasil laboratory.
        New assemblies will be contributed to open-access initiatives including the
        Vertebrate Genomes Project and Darwin Tree of Life.
      </p>
      <div class="project-methods">
        <span class="method-tag">Comparative genomics</span>
        <span class="method-tag">AlphaFold3</span>
        <span class="method-tag">FoldSeek</span>
        <span class="method-tag">dN/dS selection tests</span>
        <span class="method-tag">PhastCons</span>
        <span class="method-tag">phyloHMM</span>
        <span class="method-tag">Deep learning</span>
        <span class="method-tag">PacBio / Hi-C</span>
        <span class="method-tag">Phylogenomics</span>
      </div>
      <div class="project-collab">
        <strong>Collaborators:</strong> Globe Institute, UCPH · Natural History Museum of Denmark ·
        Greenland Institute of Natural Resources · Yggdrasil Genome Centre
      </div>
    </div>
  </div>

  <!-- PROJECT 2 -->
  <div class="project-card">
    <div class="project-num">02</div>
    <div>
      <span class="project-tag">MSc Thesis · 2024–2025 · Completed</span>
      <h2>Population Genomics of Kalmarsund Harbour Seals</h2>
      <p>
        My master's thesis investigated the population structure and conservation genetics
        of harbour seals (<em>Phoca vitulina</em>) in the Kalmarsund strait — a population
        geographically isolated from neighbouring Baltic and North Sea populations.
        Using whole-genome data, I characterised levels of genetic diversity, inbreeding,
        and connectivity, with direct implications for conservation management.
      </p>
      <div class="project-methods">
        <span class="method-tag">Population genomics</span>
        <span class="method-tag">Variant calling</span>
        <span class="method-tag">Admixture analysis</span>
        <span class="method-tag">ROH analysis</span>
        <span class="method-tag">Python · R</span>
      </div>
      <div class="project-collab">
        <strong>Supervisor:</strong> Morten Tange Olsen Group, Globe Institute, UCPH ·
        Grade: 12
      </div>
    </div>
  </div>

  <!-- PROJECT 3 -->
  <div class="project-card">
    <div class="project-num">03</div>
    <div>
      <span class="project-tag">Pilot Project · 2023 · Completed</span>
      <h2>AI-Based By-Catch Assessment on R/V Tarajoq</h2>
      <p>
        An independent pilot project applying machine learning and computer vision to
        automate by-catch assessment during Arctic trawl surveys aboard the
        Greenland Institute of Natural Resources research vessel R/V Tarajoq.
        Integrated image data with fisheries databases to test ML workflows for
        species identification and count estimation in real field conditions.
      </p>
      <div class="project-methods">
        <span class="method-tag">Machine learning</span>
        <span class="method-tag">Computer vision</span>
        <span class="method-tag">Python</span>
        <span class="method-tag">Fisheries databases</span>
      </div>
      <div class="project-collab">
        <strong>Institution:</strong> Greenland Institute of Natural Resources (GINR) · Grade: 12
      </div>
    </div>
  </div>

  <!-- PROJECT 4 -->
  <div class="project-card">
    <div class="project-num">04</div>
    <div>
      <span class="project-tag">BSc Thesis · 2022 · Completed</span>
      <h2>Genetic Structure in the Common Warthog</h2>
      <p>
        Bachelor's thesis investigating population genetic structure across the range of
        the common warthog (<em>Phacochoerus africanus</em>) using genomic data.
        The study explored how geography and ecology shape genetic differentiation
        across African populations.
      </p>
      <div class="project-methods">
        <span class="method-tag">Population genetics</span>
        <span class="method-tag">Phylogenetics</span>
        <span class="method-tag">R · Python</span>
      </div>
      <div class="project-collab">
        <strong>Institution:</strong> University of Copenhagen · Grade: 12
      </div>
    </div>
  </div>

  <!-- PUBLICATIONS -->
  <div class="pubs-section">
    <div class="pubs-label">Publications &amp; presentations</div>

    <div class="pub-item">
      <span class="pub-year">2026</span>
      <div>
        <div class="pub-title">
          First record of the Portuguese rabbitfish <em>Chimaera lusitanicus</em>
          (Chimaeridae) in Greenland waters
          <span class="pub-status">In review</span>
        </div>
        <div class="pub-journal">Reinholdt, A.C. et al. · Cybium, International Journal of Ichthyology</div>
      </div>
    </div>

    <div class="pub-item">
      <span class="pub-year">2024</span>
      <div>
        <div class="pub-title">The Genomics of Kalmarsund Harbour Seals</div>
        <div class="pub-journal">Talk · Danish Marine Mammal Symposium (DMMS)</div>
      </div>
    </div>

    <div class="pub-item">
      <span class="pub-year">2023</span>
      <div>
        <div class="pub-title">Uncovering the Genetic Structure of the Kalmarsund Harbour Seals</div>
        <div class="pub-journal">Talk · Evolution and Population Genetics in Denmark (EPIC) Conference</div>
      </div>
    </div>

    <div class="pub-item">
      <span class="pub-year">2023</span>
      <div>
        <div class="pub-title">
          New research platform offers unprecedented opportunities for studying
          Northern bottlenose whales in the Arctic
          <span class="pub-status">Best poster award</span>
        </div>
        <div class="pub-journal">Poster · European Cetacean Society Conference (ECS)</div>
      </div>
    </div>
  </div>
</div>
