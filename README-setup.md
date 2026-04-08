# Areinholdt.github.io — Setup Guide

## Files to copy into your GitHub repo

Replace or create each file below in your repository root.

### Required files (copy all of these)

| File | Description |
|------|-------------|
| `_config.yml` | Site configuration — **replaces your current one** |
| `_layouts/default.html` | Main layout with navigation and deep-ocean design |
| `_layouts/post.html` | Blog post layout |
| `index.html` | Homepage |
| `about.md` | About me page |
| `research.md` | Research projects page |
| `posts.md` | Blog listing page |
| `cv.md` | CV page |
| `contact.md` | Contact page |
| `_posts/2026-04-07-my-first-post.md` | Your first blog post (updated) |

---

## How to upload to GitHub

1. Go to your repo at github.com/Areinholdt/Areinholdt.github.io
2. For **new folders** like `_layouts/`: click "Add file" → "Create new file" → type `_layouts/default.html` as the filename (GitHub will create the folder automatically)
3. Paste the file content and commit
4. Repeat for each file

---

## Adding your photos

The site has placeholder slots for photos. To add real images:

1. Upload your images to the `/images/` folder in your repo
2. In each file, find the comment lines like:
   ```html
   <!-- <img src="/images/TVA-kaskelothvalen.jpg" alt="Sperm whale"> -->
   ```
3. Remove the `<!--` and `-->` around the `<img>` tag to activate it
4. Delete the placeholder `<div class="img-placeholder">...</div>` above it

**Recommended photos to add:**
- `/images/TVA-kaskelothvalen.jpg` — already in your repo ✓
- `/images/portrait.jpg` — your headshot (for the About page)
- `/images/fieldwork.jpg` — any expedition photo
- `/images/lab.jpg` — lab work photo

---

## Setting up the contact form

The contact form uses [Formspree](https://formspree.io) (free tier = 50 submissions/month).

1. Go to formspree.io and create a free account
2. Create a new form — it gives you a form ID like `xpzgkdqw`
3. In `contact.md`, replace `YOUR_FORM_ID` with your actual ID:
   ```
   action="https://formspree.io/f/xpzgkdqw"
   ```

---

## Adding new blog posts

Create a new file in `_posts/` with the format:
```
YYYY-MM-DD-your-title.md
```

Start every post with:
```yaml
---
layout: post
title: "Your Post Title"
date: 2026-04-08 12:00:00 +0000
categories: blog research
excerpt: "A short summary shown on the blog listing page."
---

Your post content here...
```

---

## Uploading your CV PDF

Place your CV PDF at `/assets/CV_Reinholdt.pdf` in your repo.
The CV page has a "Download PDF" button already linked to this path.
