---
layout: default
title: Contact
permalink: /contact/
---
<style>
  .contact-wrap {
    max-width: 1000px; margin:0 auto; padding:9rem 4rem 6rem;
    position:relative; z-index:1;
  }
  .contact-grid {
    display: grid; grid-template-columns:1fr 1fr; gap:5rem; align-items:start;
  }
  .contact-eyebrow {
    font-size:13px; letter-spacing:.3em; text-transform:uppercase; color:var(--accent);
    margin-bottom:1rem; display:flex; align-items:center; gap:.8rem;
  }
  .contact-eyebrow::before { content:''; width:28px; height:1px; background:var(--accent); display:block; }
  .contact-intro h1 {
    font-family:var(--serif);
    font-size: clamp(2.5rem, 4vw, 3.8rem);
    font-weight:300; line-height:1.1; color:var(--ink); margin-bottom:1.2rem;
  }
  .contact-intro h1 em { font-style:italic; color:var(--accent-bright); }
  .contact-intro p { color:var(--ink-muted); font-size:13px; line-height:2.1; margin-bottom:2rem; }

  .contact-detail {
    display:flex; align-items:flex-start; gap:1rem;
    padding:.9rem 0; border-bottom:1px solid var(--border);
  }
  .contact-detail:last-child { border-bottom:none; }
  .cd-label {
    font-size:13x; letter-spacing:.18em; text-transform:uppercase;
    color:var(--accent); min-width:80px; padding-top:.1rem;
  }
  .cd-value { font-size:13px; color:var(--ink-muted); line-height:1.6; }
  .cd-value a { color:var(--accent-bright); text-decoration:none; }
  .cd-value a:hover { text-decoration:underline; }

  .contact-open {
    margin-top:2rem; padding:1.5rem; background:var(--bg-card); border:1px solid var(--border);
  }
  .contact-open-title {
    font-size:10px; letter-spacing:.18em; text-transform:uppercase; color:var(--gold); margin-bottom:.8rem;
  }
  .contact-open p { font-size:13px; color:var(--ink-muted); line-height:1.9; }

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
    font-size: 13px;
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
        I am open to Research collaborations & data sharing, Genome sequencing partnerships, Fieldwork opportunities,              Media & science communication, Guest lectures, Communication & outreach.
      </p>

      <div class="contact-detail">
        <span class="cd-label">Email</span>
        <span class="cd-value"><a href="mailto:annika.reinholdt@sund.ku.dk">annika.reinholdt@sund.ku.dk</a></span>
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
        <span class="cd-value">Globe Institute, UCPH<br>Danish Marine Mammal Society</span>
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
          Or email directly: <a href="mailto:annika.reinholdt@sund.ku.dk" style="color:var(--accent-bright);">annika.reinholdt@sund.ku.dk</a>
        </p>
      </form>
    </div>
  </div>
</div>
