# M3DocDep — Project Page

CVPR 2026 paper project page for M3DocDep: Multi-modal, Multi-page, Multi-document Dependency Chunking with Large Vision-Language Models.

## Files

```
.
├── index.html              # Main page (single-file: HTML + CSS + JS inlined)
├── assets/
│   ├── architecture.png    # Figure 1: M3DocDep pipeline
│   └── qualitative.png     # Trolleybus qualitative example
└── README.md               # This file
```

## Quick start

Open `index.html` in a browser. That's it — no build step.

## Deploying to GitHub Pages (recommended)

1. Create a public repo on GitHub. Common naming conventions:
   - **`m3docdep.github.io`** — page lives at `https://m3docdep.github.io/`
   - **`<username>/m3docdep`** — page lives at `https://<username>.github.io/m3docdep/`

2. Push these files to the repo's `main` branch:
   ```bash
   git init
   git add index.html assets/ README.md
   git commit -m "initial project page"
   git branch -M main
   git remote add origin git@github.com:<username>/m3docdep.git
   git push -u origin main
   ```

3. On GitHub: **Settings → Pages → Build and deployment → Source: Deploy from a branch → Branch: `main`, `/` (root) → Save**.

4. Wait ~1 minute. Page goes live at the URL shown in the Pages section.

## Customization checklist

Before you publish, update these in `index.html`:

- [ ] **Hero badge buttons** — replace `href="#"` with real URLs:
  - `Paper` → arXiv PDF link or camera-ready PDF
  - `arXiv` → arXiv abstract page
  - `Code` → GitHub repo URL
- [ ] **Footer** — confirm contact email and GitHub repo link
- [ ] **BibTeX** — once the paper is officially published, update the citation block (the `@inproceedings{...}` entry near the bottom of the file). Replace the current placeholder with the official ACM/IEEE citation if needed.
- [ ] **OG meta tags** — for nice link previews on Twitter/Slack, edit the `<meta property="og:title">` and `og:description` tags in `<head>`.

Search the file for `href="#"` to find all placeholder links.

## Updating content

The page is a single HTML file with inline CSS/JS. To edit:

- **Text** — edit directly in the `<body>` markup. Sections are clearly commented (`<!-- ════════ METHOD ════════ -->` etc.).
- **Numbers** — search for the value (e.g., `+10.6%`, `82.9 / 76.5`) to find and update.
- **Colors** — edit the CSS variables at the top (`:root { ... }`).
- **Fonts** — Fraunces (serif headers) and IBM Plex Sans (body) load from Google Fonts. Edit the `<link>` tag in `<head>` to swap.
- **Images** — replace files in `assets/` (keep filenames the same to avoid editing HTML).

## Browser support

- Modern browsers (Chrome, Firefox, Safari, Edge — last 2 versions).
- Uses `IntersectionObserver` for scroll reveals (Safari 12.1+, all modern browsers).
- `backdrop-filter` on sticky nav (degrades gracefully on older browsers).
- Mobile-responsive via media queries (breakpoint at 720px).

## Notes

- Page weight: ~2.2 MB (mostly the qualitative.png image at 540 KB; architecture.png at 1.6 MB). For faster loading, consider running both PNGs through `pngquant` or converting to WebP.
- No JavaScript framework — vanilla HTML/CSS/JS only. Edit with any text editor.
- No tracking, no external scripts beyond Google Fonts.

## License

See LICENSE in the main code repository.
