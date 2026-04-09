---
layout: default
title: Research
permalink: /research/
---
<style>
  .rw { max-width:1000px; margin:0 auto; padding:9rem 3.5rem 6rem; position:relative; z-index:1; }

  .rw-header { margin-bottom:4.5rem; }
  .rw-eyebrow { font-size:13px;letter-spacing:.35em;text-transform:uppercase;color:var(--teal);display:flex;align-items:center;gap:.7rem;margin-bottom:1.2rem; }
  .rw-eyebrow::before { content:'';width:20px;height:1px;background:var(--teal);display:block; }
  .rw-header h1 { font-family:var(--serif);font-size:clamp(2.5rem,4.5vw,4rem);font-weight:400;line-height:1.08;color:var(--ink);margin-bottom:1.2rem; }
  .rw-header h1 em { font-style:italic;color:var(--bright); }
  .rw-header .lead { color:var(--muted);font-size:12.5px;line-height:2.2;max-width:640px; }

  /* GENOME BAR */
  .genome-vis {
    background:var(--card); border:1px solid var(--border);
    padding:2rem; margin-bottom:3rem; display:grid;
    grid-template-columns:1fr 1fr; gap:2rem; align-items:center;
  }
  .gv-left h3 { font-family:var(--serif);font-size:1.3rem;font-weight:400;color:var(--ink);margin-bottom:.8rem;font-style:italic; }
  .gv-left p { color:var(--muted);font-size:12px;line-height:1.9; }
  .gv-bars { display:flex;flex-direction:column;gap:.7rem; }
  .gv-row { display:flex;align-items:center;gap:.8rem; }
  .gv-label { font-size:9px;letter-spacing:.12em;text-transform:uppercase;color:var(--muted);min-width:100px; }
  .gv-track { flex:1;height:6px;background:var(--surface); }
  .gv-fill { height:100%; }
  .gv-pct { font-size:10px;min-width:36px;text-align:right; }

  /* SAMPLES STATUS */
  .samples-box {
    background: var(--card);
    border: 1px solid var(--border);
    padding: 2rem;
    margin: 3rem 0;
  }
  .samples-box h3 {
    font-family: var(--serif);
    font-size: 1.2rem;
    font-weight: 400;
    color: var(--ink);
    margin-bottom: 1.5rem;
  }
  .samples-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 2rem;
  }
  .sample-stat {
    text-align: center;
  }
  .sample-num {
    font-family: var(--serif);
    font-size: 3rem;
    color: var(--teal);
    line-height: 1;
  }
  .sample-label {
    font-size: 11px;
    letter-spacing: 0.1em;
    text-transform: uppercase;
    color: var(--muted);
    margin-top: 0.5rem;
  }

  /* OBJECTIVES */
  .objectives { margin-bottom:3.5rem; }
  .obj-grid { display:grid;grid-template-columns:repeat(3,1fr);gap:1rem;margin-top:1.5rem; }
  .obj-card { background:var(--card);border:1px solid var(--border);padding:1.8rem; }
  .obj-num { font-family:var(--serif);font-size:2.5rem;color:var(--faint);line-height:1;margin-bottom:.5rem;font-weight:400; }
  .obj-title { font-size:10px;letter-spacing:.15em;text-transform:uppercase;color:var(--teal);margin-bottom:.7rem; }
  .obj-p { color:var(--muted);font-size:11.5px;line-height:1.9; }

  /* METHODOLOGY */
  .methodology { margin-bottom:3.5rem; }
  .meth-grid { display:grid;grid-template-columns:1fr 1fr;gap:1.2rem;margin-top:1.5rem; }
  .meth-card { background:var(--surface);border:1px solid var(--border);padding:1.5rem; }
  .meth-card h4 { font-size:9px;letter-spacing:.18em;text-transform:uppercase;color:var(--accent);margin-bottom:.7rem; }
  .meth-card p { color:var(--muted);font-size:11.5px;line-height:1.9; }
  .tags { display:flex;flex-wrap:wrap;gap:.3rem;margin-top:.8rem; }
  .tag { font-size:9px;letter-spacing:.1em;text-transform:uppercase;color:var(--muted);background:rgba(77,166,224,0.06);border:1px solid var(--border);padding:.15rem .45rem; }

  /* COLLABORATORS */
  .collabs { background:var(--bg2);border:1px solid var(--border);padding:2rem;margin-bottom:3.5rem; }
  .collabs h3 { font-size:9px;letter-spacing:.25em;text-transform:uppercase;color:var(--accent);margin-bottom:1.2rem; }
  .collab-row { display:flex;flex-wrap:wrap;gap:1.2rem; }
  .collab { background:var(--card);border:1px solid var(--border);padding:.7rem 1.2rem;font-size:11px;color:var(--muted); }


  @media(max-width:768px){
    .rw { padding:8rem 1.5rem 4rem; }
    .genome-vis { grid-template-columns:1fr; }
    .obj-grid { grid-template-columns:1fr; }
    .meth-grid { grid-template-columns:1fr; }
  }
</style>

<div class="rw">

  <div class="rw-header">
    <div class="rw-eyebrow">Research Project</div>
    <h1>Deep, Dark<br>and <em>Cold</em></h1>
    <p class="lead">
      Convergent Genomics of Arctic Marine Taxa — investigating how Arctic and deep-sea fish
      survive extreme pressure, cold, and darkness by exploring the 98% of the genome
      that most science has never looked at.
    </p>
  </div>

  <!-- GENOME VISUALISATION -->
  <div class="genome-vis">
    <div class="gv-left">
      <h3>The unexplored 98%</h3>
      <p>
        Most genomic studies focus on protein-coding genes — only ~2% of the genome.
        The other 98%, non-coding regulatory DNA, controls when and where genes are
        expressed. This project is one of the first to study this "dark genome"
        in Arctic deep-sea species.
      </p>
    </div>
    <div class="gv-bars">
      <div class="gv-row">
        <span class="gv-label">Coding DNA</span>
        <div class="gv-track"><div class="gv-fill" style="width:2%;background:var(--teal);"></div></div>
        <span class="gv-pct" style="color:var(--teal);">~2%</span>
      </div>
      <div class="gv-row">
        <span class="gv-label">Dark genome</span>
        <div class="gv-track"><div class="gv-fill" style="width:98%;background:var(--accent);opacity:.5;"></div></div>
        <span class="gv-pct" style="color:var(--accent);">~98%</span>
      </div>
      <div style="font-size:9px;color:var(--faint);margin-top:.3rem;letter-spacing:.08em;">This project's focus — largely unmapped from an evolutionary perspective</div>
    </div>
  </div>

  <!-- SAMPLES STATUS -->
  <div class="samples-box">
    <h3>Samples collected & sequenced</h3>
    
    <div class="samples-grid">
      <div class="sample-stat">
        <div class="sample-num">100+</div>
        <div class="sample-label">Tissue samples collected</div>
      </div>
      
      <div class="sample-stat">
        <div class="sample-num">2</div>
        <div class="sample-label">Species sequenced</div>
      </div>
    </div>
  </div>

  <!-- BACKGROUND -->
  <div style="margin-bottom:3.5rem;">
    <div class="section-label">Background</div>
    <p style="color:var(--muted);font-size:12.5px;line-height:2.2;max-width:760px;margin-bottom:1rem;">
      The Arctic is changing fast. Boreal species are moving north, and endemic Arctic taxa
      are under growing pressure — many hypothesised to seek refuge in the deep ocean,
      a relatively stable environment of high pressure, low oxygen, and total darkness.
    </p>
    <p style="color:var(--muted);font-size:12.5px;line-height:2.2;max-width:760px;margin-bottom:1rem;">
      While physiological adaptations to these conditions have been explored, the genomic
      mechanisms — particularly within non-coding DNA — remain largely unknown.
      A key open question is whether the same genomic solutions evolved independently
      across unrelated deep-sea lineages: <em style="color:var(--bright);">convergent evolution at the molecular level.</em>
    </p>
    <p style="color:var(--muted);font-size:12.5px;line-height:2.2;max-width:760px;">
      This project addresses that gap by combining coding and non-coding genomic regions,
      protein structure modelling, and phylogenetic diversification analyses —
      applied specifically to Arctic taxa, an understudied group with direct relevance
      to climate change prediction and conservation.
    </p>
  </div>

  <!-- RESEARCH OBJECTIVES -->
  <div class="objectives">
    <div class="section-label">Research objectives</div>
    <div class="obj-grid">
      <div class="obj-card">
        <div class="obj-num">01</div>
        <div class="obj-title">Genomic drivers of adaptation</div>
        <p class="obj-p">
          Identify coding genes under selection and conserved or accelerated non-coding
          regions across Arctic deep-sea species. Reveal the genetic and regulatory
          factors enabling survival at high pressure, low temperature, and in darkness.
        </p>
      </div>
      <div class="obj-card">
        <div class="obj-num">02</div>
        <div class="obj-title">Protein structure &amp; novelty</div>
        <p class="obj-p">
          Explore whether adaptation is driven by large evolutionary leaps or
          subtle shifts in protein structure. Link DNA changes to their biological
          effects using AlphaFold3 and FoldSeek structural comparison.
        </p>
      </div>
      <div class="obj-card">
        <div class="obj-num">03</div>
        <div class="obj-title">Genomics &amp; diversification</div>
        <p class="obj-p">
          Discover why some Arctic deep-sea lineages are more successful than others.
          Combine evolutionary trees and fossil records to test which genomic
          and environmental factors help lineages thrive in extreme conditions.
        </p>
      </div>
    </div>
  </div>

  <!-- METHODOLOGY -->
  <div class="methodology">
    <div class="section-label">Methodology</div>
    <div class="meth-grid">
      <div class="meth-card">
        <h4>Genome dataset</h4>
        <p>15–20 deep-sea species genomes alongside shallow-water relatives. New chromosome-level assemblies generated using PacBio/Hi-C pipelines at Yggdrasil laboratory. Contributed to the Vertebrate Genomes Project and Darwin Tree of Life.</p>
      </div>
      <div class="meth-card">
        <h4>Coding region analysis</h4>
        <p>Selection tested using dN/dS ratios and site-specific models to detect accelerated or conserved genes. Gene ontology and pathway analyses link genes to biological functions relevant to deep-sea adaptation.</p>
      </div>
      <div class="meth-card">
        <h4>Non-coding DNA</h4>
        <p>Deep learning models including PhastCons, phyloHMM, and DeepCons identify conserved and accelerated elements in the regulatory "dark genome" — a major unexplored frontier in Arctic evolutionary biology.</p>
      </div>
       <div class="meth-card">
        <h4>Protein structure</h4>
        <p>3D structures predicted with AlphaFold3 and compared across species using FoldSeek. Structural metrics — stability, domain rearrangements, interface changes — quantify whether molecular changes are subtle or represent major evolutionary leaps.</p>
      </div>
  
    </div>
  </div>

  <!-- COLLABORATORS -->
  <div class="collabs">
    <h3>Collaborators &amp; institutions</h3>
    <div class="collab-row">
      <span class="collab">who who who</span>
      <span class="collab">Natural History Museum of Denmark</span>
      <span class="collab">who who who</span>
      <span class="collab">who who who</span>
      <span class="collab">who who who</span>
      <span class="collab">who who who</span>
    </div>
  </div>

  <div style="text-align:center;padding-top:1rem;">
    <a href="/contact" class="btn btn-primary">Get in touch about collaborating</a>
  </div>

</div>
