---
layout: default
title: Field Notes
permalink: /posts/
---
<style>
  .posts-wrap {
    max-width: 1000px; margin:0 auto; padding:9rem 4rem 6rem;
    position:relative; z-index:1;
  }
  .posts-eyebrow {
    font-size:10px; letter-spacing:.3em; text-transform:uppercase; color:var(--accent);
    margin-bottom:1rem; display:flex; align-items:center; gap:.8rem;
  }
  .posts-eyebrow::before { content:''; width:28px; height:1px; background:var(--accent); display:block; }
  .posts-header h1 {
    font-family: var(--serif);
    font-size: clamp(2.5rem, 4vw, 3.8rem);
    font-weight:300; line-height:1.1; color:var(--ink); margin-bottom:1rem;
  }
  .posts-header h1 em { font-style:italic; color:var(--accent-bright); }
  .posts-header p { color:var(--ink-muted); font-size:12.5px; line-height:2; max-width:560px; margin-bottom:3.5rem; }

  .posts-grid {
    display: grid;
    grid-template-columns: repeat(3, 1fr);
    gap: 1.2rem;
  }
  .post-card {
    background: var(--bg-card);
    border: 1px solid var(--border);
    padding: 2rem;
    text-decoration: none;
    display: block;
    transition: border-color 0.2s;
  }
  .post-card:hover { border-color: var(--accent); }
  .post-date {
    font-size: 10px; letter-spacing:.18em; color:var(--accent);
    text-transform:uppercase; margin-bottom:1rem; display:block;
  }
  .post-title {
    font-family: var(--serif);
    font-size: 1.3rem; font-weight:400; color:var(--ink);
    line-height:1.3; margin-bottom:.7rem;
  }
  .post-cats {
    font-size: 10px; letter-spacing:.1em; text-transform:uppercase;
    color: var(--ink-faint); margin-bottom:.8rem;
  }
  .post-excerpt { color:var(--ink-muted); font-size:12px; line-height:1.9; }
  .post-read {
    display:inline-block; margin-top:1.2rem;
    font-size:10px; letter-spacing:.15em; color:var(--accent-bright);
    text-transform:uppercase;
  }
  .no-posts {
    color: var(--ink-faint); font-size:13px; padding:3rem 0;
    grid-column: 1/-1; text-align:center;
  }

  @media (max-width:900px) {
    .posts-wrap { padding:8rem 1.5rem 4rem; }
    .posts-grid { grid-template-columns:1fr; }
  }
</style>

<div class="posts-wrap">
  <div class="posts-header">
    <div class="posts-eyebrow">Field notes &amp; updates</div>
    <h1>From the <em>deep</em></h1>
    <p>
      Dispatches from the lab, the ship, and the ocean floor.
      Updates on research, fieldwork, conferences, and marine science.
    </p>
  </div>

  <div class="posts-grid">
    {% if site.posts.size > 0 %}
      {% for post in site.posts %}
        <a href="{{ post.url }}" class="post-card">
          <span class="post-date">{{ post.date | date: "%d %b %Y" }}</span>
          <div class="post-title">{{ post.title }}</div>
          {% if post.categories %}
            <div class="post-cats">{{ post.categories | join: " · " }}</div>
          {% endif %}
          {% if post.excerpt %}
            <div class="post-excerpt">{{ post.excerpt | strip_html | truncatewords: 28 }}</div>
          {% endif %}
          <span class="post-read">Read more →</span>
        </a>
      {% endfor %}
    {% else %}
      <div class="no-posts">No posts yet — check back soon.</div>
    {% endif %}
  </div>
</div>
