---
layout: default
title: CV
permalink: /cv/
---
<style>
  .cv-wrap {
    max-width: 1000px; margin:0 auto; padding:9rem 4rem 6rem;
    position:relative; z-index:1;
  }
  .cv-top {
    display: flex; justify-content:space-between; align-items:flex-start;
    margin-bottom:3.5rem; flex-wrap:wrap; gap:1.5rem;
  }
  .cv-eyebrow {
    font-size:10px; letter-spacing:.3em; text-transform:uppercase; color:var(--accent);
    margin-bottom:1rem; display:flex; align-items:center; gap:.8rem;
  }
  .cv-eyebrow::before { content:''; width:28px; height:1px; background:var(--accent); display:block; }
  .cv-top h1 {
    font-family:var(--serif);
    font-size: clamp(2.5rem, 4vw, 3.8rem);
    font-weight:300; line-height:1.1; color:var(--ink);
  }
  .cv-top h1 em { font-style:italic; color:var(--accent-bright); }
  .cv-download-area { display:flex; flex-direction:column; align-items:flex-end; gap:1rem; }

  .cv-grid {
    display: grid;
    grid-template-columns: 1fr 1fr;
    gap: 3.5rem 4rem;
  }
  .cv-section h2 {
    font-family:var(--serif);
    font-size:1.3rem; font-weight:400; color:var(--gold);
    margin-bottom:1.5rem; letter-spacing:.04em;
    padding-bottom:.8rem; border-bottom:1px solid var(--border);
  }
  .cv-item { padding:1.1rem 0; border-bottom:1px solid rgba(58,143,196,0.09); }
  .cv-item:last-child { border-bottom:none; }
  .cv-year { font-size:10px; letter-spacing:.15em; color:var(--accent); text-transform:uppercase; margin-bottom:.25rem; }
  .cv-role { font-size:13px; color:var(--ink); margin-bottom:.2rem; line-height:1.5; }
  .cv-place { font-size:11.5px; color:var(--ink-muted); }
  .cv-note { font-size:11px; color:var(--ink-faint); margin-top:.3rem; font-style:italic; }

  /* FULL WIDTH SECTIONS */
  .cv-full { margin-top:3rem; }
  .cv-full h2 {
    font-family:var(--serif);
    font-size:1.3rem; font-weight:400; color:var(--gold);
    margin-bottom:1.5rem; letter-spacing:.04em;
    padding-bottom:.8rem; border-bottom:1px solid var(--border);
  }
  .skills-row {
    display:grid; grid-template-columns:repeat(3,1fr); gap:1rem; margin-bottom:1rem;
  }
  .skill-pill {
    background:var(--bg-card); border:1px solid var(--border);
    padding:.5rem 1rem; font-size:11.5px; color:var(--ink-muted);
  }
  .skill-pill strong { display:block; font-size:9.5px; letter-spacing:.15em; text-transform:uppercase; color:var(--accent); margin-bottom:.25rem; font-weight:400; }

  .pub-row { padding:.9rem 0; border-bottom:1px solid rgba(58,143,196,0.09); display:grid; grid-template-columns:55px 1fr; gap:1rem; }
  .pub-year-sm { font-size:10px; color:var(--accent); letter-spacing:.1em; padding-top:.1rem; }
  .pub-text { font-size:12px; color:var(--ink-muted); line-height:1.8; }
  .pub-text em { color:var(--ink); font-style:italic; }
  .badge {
    display:inline-block; font-size:9px; letter-spacing:.12em; text-transform:uppercase;
    padding:.15rem .45rem; margin-left:.5rem;
  }
  .badge-gold { background:rgba(200,169,110,0.12); color:var(--gold); border:1px solid rgba(200,169,110,0.25); }
  .badge-blue { background:rgba(58,143,196,0.1); color:var(--accent); border:1px solid var(--accent-glow); }

  @media (max-width:768px) {
    .cv-wrap { padding:8rem 1.5rem 4rem; }
    .cv-grid { grid-template-columns:1fr; gap:2rem; }
    .skills-row { grid-template-columns:1fr 1fr; }
    .cv-top { flex-direction:column; }
    .cv-download-area { align-items:flex-start; }
  }
</style>

<div class="cv-wrap">
  <div class="cv-top">
    <div>
      <div class="cv-eyebrow">Curriculum vitae</div>
      <h1>Annika Caroline<br><em>Reinholdt</em></h1>
    </div>
    <div class="cv-download-area">
      <a href="/assets/CV_Reinholdt.pdf" class="btn btn-ghost">Download PDF</a>
      <div style="font-size:10px;color:var(--ink-faint);letter-spacing:.1em;">ozreinholdt@gmail.com</div>
      <div style="font-size:10px;color:var(--ink-faint);letter-spacing:.1em;">Copenhagen, Denmark</div>
    </div>
  </div>

  <div class="cv-grid">

    <div class="cv-section">
      <h2>Education</h2>
      <div class="cv-item">
        <div class="cv-year">Feb 2025</div>
        <div class="cv-role">MSc Bioinformatics, Computational Biology</div>
        <div class="cv-place">University of Copenhagen</div>
        <div class="cv-note">GPA 11.06 · Thesis grade: 12</div>
      </div>
      <div class="cv-item">
        <div class="cv-year">Jun 2022</div>
        <div class="cv-role">BSc Biology (specialisation in Bioinformatics)</div>
        <div class="cv-place">University of Copenhagen</div>
        <div class="cv-note">GPA 9.17 · Thesis grade: 12</div>
      </div>
    </div>

    <div class="cv-section">
      <h2>Work experience</h2>
      <div class="cv-item">
        <div class="cv-year">Mar 2025 – Oct 2025</div>
        <div class="cv-role">IT Consultant</div>
        <div class="cv-place">Netcompany, Copenhagen</div>
        <div class="cv-note">Automated test pipelines · SQL/AWS · Workshop delivery</div>
      </div>
      <div class="cv-item">
        <div class="cv-year">Jun 2022 – Feb 2025</div>
        <div class="cv-role">Research Group Member</div>
        <div class="cv-place">Olsen Group, Globe Institute, UCPH</div>
        <div class="cv-note">Population genomics · DNA extraction · Fieldwork</div>
      </div>
      <div class="cv-item">
        <div class="cv-year">Aug 2022 – present</div>
        <div class="cv-role">Student Assistant</div>
        <div class="cv-place">Greenland Institute of Natural Resources (GINR)</div>
        <div class="cv-note">Arctic surveys · R/V Tarajoq · R/V Sanna</div>
      </div>
      <div class="cv-item">
        <div class="cv-year">Oct 2021 – Dec 2021</div>
        <div class="cv-role">Communications Assistant</div>
        <div class="cv-place">Dept. of Science Education, UCPH</div>
      </div>
    </div>

    <div class="cv-section">
      <h2>Fieldwork</h2>
      <div class="cv-item">
        <div class="cv-year">Jul 2024</div>
        <div class="cv-role">Field Researcher — Gully MPA</div>
        <div class="cv-place">Whitehead Lab, Dalhousie University</div>
        <div class="cv-note">3-week sailboat expedition · Beaked whale biopsies &amp; drone survey</div>
      </div>
      <div class="cv-item">
        <div class="cv-year">Jul 2023</div>
        <div class="cv-role">Field Leader — Anholt Island Seal Expedition</div>
        <div class="cv-place">Aarhus University / Globe Institute</div>
        <div class="cv-note">Led team in seal handling, genomic sampling, and safety</div>
      </div>
      <div class="cv-item">
        <div class="cv-year">2022 – present</div>
        <div class="cv-role">Arctic Surveys — Davis Strait</div>
        <div class="cv-place">Greenland Institute of Natural Resources</div>
        <div class="cv-note">Fish, shrimp, crab stock assessments · By-catch management · DFO collaboration</div>
      </div>
    </div>

    <div class="cv-section">
      <h2>Awards &amp; service</h2>
      <div class="cv-item">
        <div class="cv-year">2023</div>
        <div class="cv-role">Best Poster Award <span class="badge badge-gold">Award</span></div>
        <div class="cv-place">European Cetacean Society Conference (ECS)</div>
      </div>
      <div class="cv-item">
        <div class="cv-year">2024 – present</div>
        <div class="cv-role">Board Member</div>
        <div class="cv-place">Danish Marine Mammal Society (DMMS)</div>
      </div>
      <div class="cv-item">
        <div class="cv-year">Feb &amp; May 2026</div>
        <div class="cv-role">Media expert — Sperm whale stranding</div>
        <div class="cv-place">DR1 TV Avisen · DR1 TVA live · Blue Voices exhibition</div>
      </div>
    </div>

  </div><!-- end grid -->

  <!-- SKILLS -->
  <div class="cv-full">
    <h2>Skills</h2>
    <div class="skills-row">
      <div class="skill-pill"><strong>Programming</strong>Python · R · SQL · JavaScript · Bash · AWS</div>
      <div class="skill-pill"><strong>Bioinformatics</strong>Population genomics · Variant calling · Phylogenetics · AlphaFold3 · FoldSeek</div>
      <div class="skill-pill"><strong>Machine learning</strong>Deep learning · PhastCons · AI fisheries tools · Workflow automation</div>
      <div class="skill-pill"><strong>Laboratory</strong>DNA extraction · Sequencing prep · PacBio · Hi-C · Clean-lab procedures</div>
      <div class="skill-pill"><strong>Fieldwork</strong>Biopsy collection · Marine mammal handling · Trawl surveys · Expedition leadership</div>
      <div class="skill-pill"><strong>Languages</strong>Danish (native) · English (fluent)</div>
    </div>
  </div>

  <!-- PUBLICATIONS -->
  <div class="cv-full">
    <h2>Publications &amp; presentations</h2>
    <div class="pub-row">
      <div class="pub-year-sm">2026</div>
      <div class="pub-text"><em>First record of Chimaera lusitanicus in Greenland waters</em> <span class="badge badge-blue">In review</span><br>Reinholdt, A.C. et al. · Cybium, International Journal of Ichthyology</div>
    </div>
    <div class="pub-row">
      <div class="pub-year-sm">2024</div>
      <div class="pub-text"><em>The Genomics of Kalmarsund Harbour Seals</em> — Talk<br>Danish Marine Mammal Symposium</div>
    </div>
    <div class="pub-row">
      <div class="pub-year-sm">2023</div>
      <div class="pub-text"><em>Uncovering the Genetic Structure of the Kalmarsund Harbour Seals</em> — Talk<br>EPIC Population Genetics Conference</div>
    </div>
    <div class="pub-row">
      <div class="pub-year-sm">2023</div>
      <div class="pub-text"><em>New research platform for studying Northern bottlenose whales in the Arctic</em> — Poster <span class="badge badge-gold">Best poster</span><br>European Cetacean Society Conference</div>
    </div>
  </div>

</div>
