# Sole Intelligence — soleintell.com

Personal website of **Peter Sorensen, DPM, MHA** — podiatric physician, healthcare policy advocate, and clinical AI educator. Platform for *Sole Intelligence*, a Substack covering practical AI for clinical practice.

---

## Tech Stack

- Pure HTML + CSS + Vanilla JS (no build step required)
- Google Fonts (Syne + IBM Plex Sans) via CDN
- Formspree for contact form
- Vercel / GitHub Pages compatible

---

## File Structure

```
/
├── index.html              ← Home / landing page
├── pages/
│   ├── about.html          ← Full bio & affiliations
│   ├── research.html       ← Publications & posters
│   └── advocacy.html       ← Lobbying, speaking, APMA
├── styles/
│   └── globals.css         ← All styles & design tokens
├── scripts/
│   └── main.js             ← Nav, form, scroll behavior
├── assets/
│   └── icons/
│       └── favicon.svg
└── README.md
```

---

## Adding Your Photos

Drop all image files directly into the **project root** (same level as `index.html`):

| File | Used For |
|------|----------|
| `headshot.jpg` | Hero & about page |
| `ToddYoung.jpg` | Home + Advocacy — with Senator Todd Young & Dr. DeHeer |
| `Lobbying.jpg` | Home + Advocacy — Capitol Hill meeting |
| `apma.jpg` | About — APMA podium with Dr. Savannah Santiago |
| `speaking.jpg` | About + Advocacy — 2026 APMA HOD |
| `award.jpg` | About + Advocacy — MILES 2025 award |
| `Martorell.jpg` | Research — Wounds publication |
| `PCFD.jpg` | Research — Podiatry Today cover |
| `Staged Dynamization.jpg` | Research — APMA 2026 poster |
| `Calc Fx.jpg` | Research — APMA 2025 poster |
| `Fish Skin.jpg` | Research — ASVI Symposium poster |
| `ELP.jpg` | About + Research — APMA News feature |

> ⚠️ **Photo Credit Note**: `ToddYoung.jpg` and `Lobbying.jpg` must be credited to **Lisa Helfert Photography**. Credit is already included in the HTML.

---

## Deploy to Vercel (2 minutes)

1. Push this folder to a GitHub repository
2. Go to [vercel.com](https://vercel.com) → **New Project** → Import your repo
3. Vercel auto-detects static HTML — click **Deploy**
4. Set your custom domain to `soleintell.com` in Vercel project settings

No `vercel.json` or build config needed.

---

## Deploy to GitHub Pages

1. Push to a GitHub repo
2. Go to **Settings → Pages**
3. Set source to **main branch / root**
4. Your site will be live at `https://yourusername.github.io/repo-name`

---

## Formspree (Contact Form)

The contact form on `index.html` is already connected to:

```
https://formspree.io/f/xykbwjvn
```

To update it, find this line in `index.html` and replace with your new endpoint:

```html
<form id="contactForm" action="https://formspree.io/f/YOUR_ID" method="POST">
```

---

## Adding Social Links (Facebook & X)

When ready, search for `coming soon` in any HTML file and replace the placeholder spans with:

```html
<a href="https://facebook.com/YOUR_HANDLE" target="_blank" rel="noopener" 
   style="font-size: 0.85rem; color: var(--text-muted); text-decoration: none;">Facebook ↗</a>

<a href="https://x.com/YOUR_HANDLE" target="_blank" rel="noopener"
   style="font-size: 0.85rem; color: var(--text-muted); text-decoration: none;">X ↗</a>
```

---

## Editing Content

All content is in the HTML files — no CMS, no database. Open any file in a text editor, find the section comment (e.g., `<!-- HERO SECTION -->`), and edit the text directly.

### Design tokens (colors, fonts) are all in:
```
styles/globals.css  → :root { ... }
```

---

## Colors

| Token | Value | Use |
|-------|-------|-----|
| `--bg` | `#0C1720` | Page background |
| `--accent` | `#3A9EA5` | Teal — CTAs, highlights |
| `--text` | `#D8E8F0` | Primary text |
| `--text-muted` | `#8BA5BE` | Body text |
| `--bg-card` | `#162535` | Card backgrounds |

---

## Contact

Peter Sorensen, DPM, MHA  
[soleintell.com](https://soleintell.com)  
[substack.com/soleintell](https://substack.com/soleintell)
