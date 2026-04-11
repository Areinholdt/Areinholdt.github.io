---
layout: default
title: Research
permalink: /research/
---
<style>
  .rw { max-width:1000px; margin:0 auto; padding:9rem 3.5rem 6rem; position:relative; z-index:1; }

  .rw-eyebrow { font-size:13px;letter-spacing:.35em;text-transform:uppercase;color:var(--teal);display:flex;align-items:center;gap:.7rem;margin-bottom:1.2rem; }
  .rw-eyebrow::before { content:'';width:20px;height:1px;background:var(--teal);display:block; }

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

  /* SAMPLES */
  .samples-box { background:var(--card);border:1px solid var(--border);padding:2rem;margin:3rem 0; }
  .samples-box h3 { font-family:var(--serif);font-size:1.2rem;font-weight:400;color:var(--ink);margin-bottom:1.5rem; }
  .samples-grid { display:grid;grid-template-columns:1fr 1fr;gap:2rem; }
  .sample-stat { text-align:center; }
  .sample-num { font-family:var(--serif);font-size:3rem;color:var(--teal);line-height:1; }
  .sample-label { font-size:11px;letter-spacing:.1em;text-transform:uppercase;color:var(--muted);margin-top:.5rem; }

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
    .rw-hero { grid-template-columns:1fr !important; }
    .genome-vis { grid-template-columns:1fr; }
    .obj-grid { grid-template-columns:1fr; }
    .meth-grid { grid-template-columns:1fr; }
  }
</style>

<div class="rw">

  <!-- HEADER WITH PHOTO -->
  <div class="rw-hero" style="display:grid;grid-template-columns:1fr 1fr;gap:4rem;align-items:start;margin-bottom:4.5rem;">
    <div>
      <div class="rw-eyebrow">Research Project</div>
      <h1 style="font-family:var(--serif);font-size:clamp(2.5rem,4.5vw,4rem);font-weight:400;line-height:1.08;color:var(--ink);margin-bottom:1.5rem;">Deep, Dark<br>and <em style="font-style:italic;color:var(--bright);">Cold</em></h1>
      <p style="color:var(--muted);font-size:12.5px;line-height:2.2;">
        Most genomic research has explored only 2% of the genome. 
        This project goes into the other 98%, the part that acts 
        like a control panel, switching genes on and off and 
        shaping how animals survive. No one has mapped this in 
        Arctic deep-sea fish, sharks, and whales. 
        That is what this project sets out to do.
      </p>
    </div>
    <div style="overflow:hidden;border:1px solid var(--border);">
      <img src="/images/angler_annika.jpg" alt="Deep-sea fieldwork"
       style="width:100%;height:100%;min-height:0;max-height:400px;object-fit:cover;display:block;
              filter:brightness(0.85) saturate(0.85);object-position:center 20%;">
  </div>
  </div>

  <!-- GENOME VISUALISATION -->
  <div class="genome-vis">
    <div class="gv-left">
      <h3>The unexplored 98%</h3>
      <p>
        Most studies focus on the 2% of the genome that directly 
        codes for proteins. The other 98% acts like a control panel, 
        switching genes on and off and shaping how animals look, 
        behave, and survive. Think of it as the instruction manual 
        for the genes. In Arctic deep-sea species, that instruction 
        manual has never been read. This project is one of the 
        first to try.
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
    <h3>Samples collected &amp; sequenced</h3>
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

  <!-- RESEARCH OBJECTIVES -->
  <div class="objectives">
    <div class="section-label">Research objectives</div>
    <div class="obj-grid">
      <div class="obj-card">
        <div class="obj-num">01</div>
        <div class="obj-title">Genomic drivers of adaptation</div>
        <p class="obj-p">
          Which genes and regulatory regions have changed to allow 
          survival at high pressure, low temperature, and in total 
          darkness? And did different species independently arrive 
          at the same solutions?
        </p>
      </div>
      <div class="obj-card">
        <div class="obj-num">02</div>
        <div class="obj-title">Protein structure &amp; novelty</div>
        <p class="obj-p">
          DNA changes only matter if they change how proteins work. 
          Using AlphaFold3 and FoldSeek we translate genomic changes 
          into 3D protein structures, revealing whether deep-sea 
          adaptation happens through dramatic leaps or subtle 
          molecular fine-tuning.
        </p>
      </div>
      <div class="obj-card">
        <div class="obj-num">03</div>
        <div class="obj-title">Genomics &amp; diversification</div>
        <p class="obj-p">
          Some deep-sea lineages have diversified into dozens of 
          species. Others have barely changed. We combine evolutionary 
          trees and genomic data to find out what makes some lineages 
          winners in the deep.
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
        <p>
          A carefully selected set of Arctic deep-sea species 
          sequenced alongside shallow-water relatives for comparison. 
          New genome assemblies will be generated for key species 
          where no high-quality data exists, and contributed to 
          open-access genomic databases.
        </p>
      </div>
      <div class="meth-card">
        <h4>Coding region analysis</h4>
        <p>
          Selection tested using dN/dS ratios and site-specific 
          models to detect accelerated or conserved genes. Gene 
          ontology and pathway analyses link genes to biological 
          functions relevant to deep-sea adaptation.
        </p>
        <div class="tags">
          <span class="tag">dN/dS</span>
          <span class="tag">Gene ontology</span>
          <span class="tag">Pathway analysis</span>
        </div>
      </div>
      <div class="meth-card">
        <h4>Non-coding DNA</h4>
        <p>
          Deep learning tools identify which parts of the dark 
          genome have been conserved or accelerated across species. 
          Conserved regions are likely critical for survival. 
          Accelerated regions point to rapid adaptation.
        </p>
        <div class="tags">
          <span class="tag">PhastCons</span>
          <span class="tag">phyloHMM</span>
          <span class="tag">Deep learning</span>
        </div>
      </div>
      <div class="meth-card">
        <h4>Protein structure</h4>
        <p>
          3D protein structures predicted with AlphaFold3 and 
          compared across species using FoldSeek. This links 
          DNA changes directly to biological function, showing 
          exactly how molecular evolution happens at depth.
        </p>
        <div class="tags">
          <span class="tag">AlphaFold3</span>
          <span class="tag">FoldSeek</span>
        </div>
      </div>
    </div>
  </div>

  <!-- COLLABORATORS -->
  <div class="collabs">
    <h3>Collaborators &amp; institutions</h3>
    <div class="collab-row">
      <span class="collab">Natural History Museum of Denmark</span>
      <span class="collab">Globe Institute, University of Copenhagen</span>
      <span class="collab">Greenland Institute of Natural Resources</span>
      <span class="collab">Fisheries and Oceans Canada</span>
    </div>
  </div>

  <div style="text-align:center;padding-top:1rem;">
    <a href="/contact" class="btn btn-primary">Get in touch about collaborating</a>
  </div>

</div>
