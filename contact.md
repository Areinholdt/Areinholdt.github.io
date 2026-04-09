---
layout: default
title: Contact
permalink: /contact/
---
<style>
  .contact-wrap {
    max-width: 1000px; margin:0 auto; padding:9rem 3.5rem 6rem;
    position:relative; z-index:1;
  }
  .contact-eyebrow {
    font-size:13px; letter-spacing:.3em; text-transform:uppercase; color:var(--teal);
    margin-bottom:1rem; display:flex; align-items:center; gap:.8rem;
  }
  .contact-eyebrow::before { content:''; width:20px; height:1px; background:var(--teal); display:block; }
  .contact-top {
    display:grid; grid-template-columns:1fr 1fr; gap:4rem;
    align-items:start; margin-bottom:3rem;
  }
  .contact-photo {
    width:100%; aspect-ratio:3/4; overflow:hidden;
    border:1px solid var(--border);
  }
  .contact-photo img {
    width:100%; height:100%; object-fit:cover; display:block;
    filter:brightness(0.9) saturate(0.85);
  }
  .contact-right h1 {
    font-family:var(--serif); font-size:clamp(2.5rem,4vw,4rem);
    font-weight:400; line-height:1.1; color:var(--ink); margin-bottom:1rem;
  }
  .contact-right h1 em { font-style:italic; color:var(--bright); }
  .contact-intro {
    color:var(--muted); font-size:13px; line-height:2.1;
    margin-bottom:2rem;
  }
  .contact-email {
    display:block; font-family:var(--serif); font-size:1.3rem;
    color:var(--bright); text-decoration:none; font-style:italic;
    padding:1.5rem 0; border-top:1px solid var(--border);
    border-bottom:1px solid var(--border);
    margin-bottom:2rem; transition:color .2s;
  }
  .contact-email:hover { color:var(--teal); }

  .contact-details {
    display:flex; flex-direction:column; gap:.5rem; margin-bottom:2rem;
  }
  .cd {
    padding:.9rem 0; border-bottom:1px solid rgba(80,160,220,0.08);
    display:flex; gap:1rem; align-items:flex-start;
  }
  .cd-label {
    font-size:9px; letter-spacing:.2em; text-transform:uppercase;
    color:var(--accent); min-width:80px; padding-top:.2rem;
  }
  .cd-value { font-size:12px; color:var(--muted); line-height:1.7; }
  .cd-value a { color:var(--bright); text-decoration:none; }
  .cd-value a:hover { color:var(--teal); }

  .social-links {
    display:flex; flex-wrap:wrap; gap:.7rem; margin-bottom:2.5rem;
  }
  .social-link {
    display:flex; align-items:center; gap:.7rem;
    padding:.7rem 1.2rem; background:var(--card);
    border:1px solid var(--border); text-decoration:none;
    color:var(--muted); font-size:11px; letter-spacing:.12em;
    text-transform:uppercase; transition:all .2s;
  }
  .social-link:hover { border-color:var(--accent); color:var(--bright); }
  .social-link svg { width:16px; height:16px; flex-shrink:0; }

  .open-to {
    padding:2rem; background:var(--bg2); border:1px solid var(--border);
  }
  .open-to-title {
    font-size:9px; letter-spacing:.25em; text-transform:uppercase;
    color:var(--gold); margin-bottom:1.2rem; display:block;
  }
  .open-to-grid {
    display:grid; grid-template-columns:1fr 1fr; gap:.6rem;
  }
  .open-to-item {
    font-size:12px; color:var(--muted); padding:.5rem 0;
    border-bottom:1px solid rgba(80,160,220,0.08);
    display:flex; align-items:center; gap:.6rem;
  }
  .open-to-item::before {
    content:''; width:4px; height:4px; border-radius:50%;
    background:var(--teal); display:block; flex-shrink:0;
  }

  @media(max-width:768px){
    .contact-wrap { padding:8rem 1.5rem 4rem; }
    .contact-top { grid-template-columns:1fr; gap:2rem; }
    .open-to-grid { grid-template-columns:1fr; }
    .social-links { flex-direction:column; }
  }
</style>

<div class="contact-wrap">
  <div class="contact-eyebrow">Get in touch</div>

  <div class="contact-top">
    <div class="contact-photo">
      <img src="/images/shark_annika1.jpg" alt="Annika Reinholdt fieldwork">
    </div>

    <div class="contact-right">
      <h1>Let's go <em>deep</em></h1>
      <p class="contact-intro">
        Whether you are a researcher, a funder, a journalist, 
        or simply someone fascinated by what lives at the bottom 
        of the ocean — I would love to hear from you.
      </p>

      <a href="mailto:annika.reinholdt@sund.ku.dk" class="contact-email">
        annika.reinholdt@sund.ku.dk
      </a>

      <div class="contact-details">
        <div class="cd">
          <span class="cd-label">Location</span>
          <span class="cd-value">Copenhagen, Denmark</span>
        </div>
        <div class="cd">
          <span class="cd-label">Affiliation</span>
          <span class="cd-value">Globe Institute, UCPH<br>Danish Marine Mammal Society</span>
        </div>
      </div>

      <div class="social-links">
        <a href="https://www.instagram.com/annikareinholdt/" target="_blank" class="social-link">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5">
            <rect x="2" y="2" width="20" height="20" rx="5"/>
            <circle cx="12" cy="12" r="5"/>
            <circle cx="17.5" cy="6.5" r="1" fill="currentColor" stroke="none"/>
          </svg>
          Instagram
        </a>
        <a href="https://www.linkedin.com/in/annikacr/" target="_blank" class="social-link">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5">
            <rect x="2" y="2" width="20" height="20" rx="3"/>
            <path d="M7 10v7M7 7v.01M12 17v-4a2 2 0 0 1 4 0v4M12 10v7"/>
          </svg>
          LinkedIn
        </a>
        <a href="https://www.inaturalist.org/people/areinholdt" target="_blank" class="social-link">
          <svg viewBox="0 0 24 24" fill="none" stroke="currentColor" stroke-width="1.5">
            <circle cx="12" cy="12" r="10"/>
            <path d="M12 2a10 10 0 0 1 0 20M2 12h20"/>
          </svg>
          iNaturalist
        </a>
      </div>

      <div class="open-to">
        <span class="open-to-title">Open to</span>
        <div class="open-to-grid">
          <div class="open-to-item">Research collaborations</div>
          <div class="open-to-item">Funding partnerships</div>
          <div class="open-to-item">Genome sequencing projects</div>
          <div class="open-to-item">Fieldwork opportunities</div>
          <div class="open-to-item">Media &amp; science communication</div>
          <div class="open-to-item">Guest lectures &amp; outreach</div>
        </div>
      </div>

    </div>
  </div>
</div>
