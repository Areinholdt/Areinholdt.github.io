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
    font-size:10px; letter-spacing:.35em; text-transform:uppercase; color:var(--teal);
    margin-bottom:1.2rem; display:flex; align-items:center; gap:.8rem;
  }
  .contact-eyebrow::before { content:''; width:20px; height:1px; background:var(--teal); display:block; }
  .contact-top {
    display:grid; grid-template-columns:1.4fr 0.6fr;
    gap:5rem; align-items:start; margin-bottom:4rem;
  }
  .contact-left h1 {
    font-family:var(--serif); font-size:clamp(2.8rem,4vw,4.2rem);
    font-weight:400; line-height:1.08; color:var(--ink); margin-bottom:1.2rem;
  }
  .contact-left h1 em { font-style:italic; color:var(--bright); }
  .contact-intro {
    color:var(--muted); font-size:12.5px; line-height:2.2;
    margin-bottom:2.5rem; max-width:480px;
  }
  .contact-email {
    display:block; font-family:var(--serif);
    font-size:clamp(1.1rem,2vw,1.5rem);
    color:var(--bright); text-decoration:none; font-style:italic;
    padding:1.5rem 0; border-top:1px solid var(--border);
    border-bottom:1px solid var(--border);
    margin-bottom:2.5rem; transition:color .25s; letter-spacing:.02em;
  }
  .contact-email:hover { color:var(--teal); }
  .contact-details { margin-bottom:2.5rem; }
  .cd {
    display:flex; gap:1.2rem; align-items:flex-start;
    padding:.85rem 0; border-bottom:1px solid rgba(80,160,220,0.07);
  }
  .cd:last-child { border-bottom:none; }
  .cd-label {
    font-size:9px; letter-spacing:.2em; text-transform:uppercase;
    color:var(--accent); min-width:90px; padding-top:.15rem; flex-shrink:0;
  }
  .cd-value { font-size:12px; color:var(--muted); line-height:1.8; }
  .cd-value a { color:var(--bright); text-decoration:none; transition:color .2s; }
  .cd-value a:hover { color:var(--teal); }
  .social-title {
    font-size:9px; letter-spacing:.25em; text-transform:uppercase;
    color:var(--faint); margin-bottom:1rem; display:block;
  }
  .social-links { display:flex; flex-wrap:wrap; gap:.7rem; }
  .social-link {
    display:flex; align-items:center; gap:.6rem;
    padding:.65rem 1.1rem; background:var(--card);
    border:1px solid var(--border); text-decoration:none;
    color:var(--muted); font-size:10px; letter-spacing:.14em;
    text-transform:uppercase; transition:all .2s;
  }
  .social-link:hover { border-color:var(--accent); color:var(--bright); }
  .social-link svg { width:14px; height:14px; flex-shrink:0; }
  .contact-photo { position:sticky; top:7rem; width:100%; overflow:hidden; border:1px solid var(--border); }
  .contact-photo img {
    width:100%; display:block; object-fit:cover; aspect-ratio:3/4;
    filter:brightness(1.0) saturate(1.1); transition:filter .4s;
  }
  .contact-photo:hover img { filter:brightness(0.95) saturate(0.9); }
  .open-to {
    padding:2rem 2.5rem; background:var(--bg2);
    border:1px solid var(--border); border-left:2px solid var(--teal);
  }
  .open-to-title {
    font-size:9px; letter-spacing:.25em; text-transform:uppercase;
    color:var(--gold); margin-bottom:1.2rem; display:block;
  }
  .open-to-grid { display:grid; grid-template-columns:1fr 1fr; gap:.5rem; }
  .open-to-item {
    font-size:11.5px; color:var(--muted); padding:.45rem 0;
    border-bottom:1px solid rgba(80,160,220,0.06);
    display:flex; align-items:center; gap:.6rem; line-height:1.5;
  }
  .open-to-item::before {
    content:''; width:3px; height:3px; border-radius:50%;
    background:var(--teal); display:block; flex-shrink:0;
  }
  @media(max-width:768px){
    .contact-wrap { padding:8rem 1.5rem 4rem; }
    .contact-top { grid-template-columns:1fr; gap:3rem; }
    .contact-photo { position:static; }
    .open-to-grid { grid-template-columns:1fr; }
  }
</style>

<div class="contact-wrap">
  <div class="contact-eyebrow">Get in touch</div>
  <div class="contact-top">
    <div class="contact-left">
      <h1>Let's go<br><em>deep</em></h1>
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
          <span class="cd-value">
            Globe Institute, University of Copenhagen<br>
            Danish Marine Mammal Society
          </span>
        </div>
        <div class="cd">
          <span class="cd-label">LinkedIn</span>
          <span class="cd-value">
            <a href="https://www.linkedin.com/in/annikacr/" target="_blank">annikacr</a>
          </span>
        </div>
      </div>
      <span class="social-title">Find me online</span>
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
            <path d="M12 2c2.5 3 4 6.5 4 10s-1.5 7-4 10"/>
          </svg>
          iNaturalist
        </a>
      </div>
      <div style="margin-top:2.5rem;">
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
    <div>
      <div class="contact-photo">
        <img src="/images/shark_annika1.jpg" alt="Annika Reinholdt — fieldwork">
      </div>
    </div>
  </div>
</div>
<style>
  .contact-wrap {
    max-width: 1000px; margin:0 auto; padding:9rem 4rem 6rem;
    position:relative; z-index:1;
  }
  .contact-grid {
    display: grid; grid-template-columns:1fr 1fr; gap:5rem; align-items:start;
  }
  .contact-eyebrow {
    font-size:10px; letter-spacing:.3em; text-transform:uppercase; color:var(--accent);
    margin-bottom:1rem; display:flex; align-items:center; gap:.8rem;
  }
  .contact-eyebrow::before { content:''; width:28px; height:1px; background:var(--accent); display:block; }
  .contact-intro h1 {
    font-family:var(--serif);
    font-size: clamp(2.5rem, 4vw, 3.8rem);
    font-weight:300; line-height:1.1; color:var(--ink); margin-bottom:1.2rem;
  }
  .contact-intro h1 em { font-style:italic; color:var(--accent-bright); }
  .contact-intro p { color:var(--ink-muted); font-size:12.5px; line-height:2.1; margin-bottom:2rem; }

  .contact-detail {
    display:flex; align-items:flex-start; gap:1rem;
    padding:.9rem 0; border-bottom:1px solid var(--border);
  }
  .contact-detail:last-child { border-bottom:none; }
  .cd-label {
    font-size:10px; letter-spacing:.18em; text-transform:uppercase;
    color:var(--accent); min-width:80px; padding-top:.1rem;
  }
  .cd-value { font-size:12.5px; color:var(--ink-muted); line-height:1.6; }
  .cd-value a { color:var(--accent-bright); text-decoration:none; }
  .cd-value a:hover { text-decoration:underline; }

  .contact-open {
    margin-top:2rem; padding:1.5rem; background:var(--bg-card); border:1px solid var(--border);
  }
  .contact-open-title {
    font-size:10px; letter-spacing:.18em; text-transform:uppercase; color:var(--gold); margin-bottom:.8rem;
  }
  .contact-open p { font-size:12px; color:var(--ink-muted); line-height:1.9; }

  /* FORM */
  .contact-form { display:flex; flex-direction:column; gap:1.2rem; }
  .form-group { display:flex; flex-direction:column; gap:.4rem; }
  .form-group label {
    font-size:10px; letter-spacing:.18em; text-transform:uppercase; color:var(--ink-faint);
  }
  .form-group input,
  .form-group textarea,
  .form-group select {
    background: var(--bg-card);
    border: 1px solid var(--border);
    color: var(--ink);
    padding: .75rem 1rem;
    font-family: var(--mono);
    font-size: 12.5px;
    font-weight: 300;
    outline: none;
    transition: border-color .2s;
    width: 100%;
    resize: vertical;
  }
  .form-group input:focus,
  .form-group textarea:focus,
  .form-group select:focus { border-color: var(--accent); }
  .form-group select option { background: var(--bg-card); }

  @media (max-width:768px) {
    .contact-wrap { padding:8rem 1.5rem 4rem; }
    .contact-grid { grid-template-columns:1fr; gap:3rem; }
  }
</style>

<div class="contact-wrap">
  <div class="contact-grid">
    <div class="contact-intro">
      <div class="contact-eyebrow">Get in touch</div>
      <h1>Let's talk<br>about the <em>deep</em></h1>
      <p>
        I am open to collaborations, research partnerships, media enquiries,
        and conversations about marine genomics, Arctic biology, and ocean conservation.
      </p>

      <div class="contact-detail">
        <span class="cd-label">Email</span>
        <span class="cd-value"><a href="mailto:ozreinholdt@gmail.com">ozreinholdt@gmail.com</a></span>
      </div>
      <div class="contact-detail">
        <span class="cd-label">Location</span>
        <span class="cd-value">Copenhagen, Denmark</span>
      </div>
      <div class="contact-detail">
        <span class="cd-label">LinkedIn</span>
        <span class="cd-value"><a href="https://linkedin.com/in/annikacr" target="_blank">annikacr</a></span>
      </div>
      <div class="contact-detail">
        <span class="cd-label">Affiliations</span>
        <span class="cd-value">Globe Institute, UCPH<br>Greenland Institute of Natural Resources<br>Danish Marine Mammal Society</span>
      </div>

      <div class="contact-open">
        <div class="contact-open-title">Open to</div>
        <p>
          Research collaborations &amp; data sharing ·
          Genome sequencing partnerships ·
          Fieldwork opportunities ·
          Media &amp; science communication ·
          Guest lectures &amp; outreach
        </p>
      </div>
    </div>

    <div>
      <form class="contact-form" action="https://formspree.io/f/YOUR_FORM_ID" method="POST">
        <div class="form-group">
          <label for="name">Name</label>
          <input type="text" id="name" name="name" placeholder="Your full name" required>
        </div>
        <div class="form-group">
          <label for="email">Email</label>
          <input type="email" id="email" name="email" placeholder="your@email.com" required>
        </div>
        <div class="form-group">
          <label for="subject">Subject</label>
          <select id="subject" name="subject">
            <option value="">Select a topic...</option>
            <option value="collaboration">Research collaboration</option>
            <option value="media">Media enquiry</option>
            <option value="data">Data / genome sharing</option>
            <option value="fieldwork">Fieldwork opportunity</option>
            <option value="other">Other</option>
          </select>
        </div>
        <div class="form-group">
          <label for="message">Message</label>
          <textarea id="message" name="message" rows="6" placeholder="What would you like to discuss?" required></textarea>
        </div>
        <button type="submit" class="btn btn-primary" style="align-self:flex-start;">Send message</button>
        <p style="font-size:11px;color:var(--ink-faint);margin-top:.5rem;">
          Or email directly: <a href="mailto:ozreinholdt@gmail.com" style="color:var(--accent-bright);">ozreinholdt@gmail.com</a>
        </p>
      </form>
    </div>
  </div>
</div>
