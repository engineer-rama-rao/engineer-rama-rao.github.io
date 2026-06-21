# Rama H. S. Rao — Personal Portfolio

Personal website for **Rama H. S. Rao, BEng (PhD)** — Senior Project Senior Project & Highway Engineer, FCIHT, FIHE Highway Engineer, BEng (PhD), FCIHT, FIHE, CDMC.

🌐 **Live site (target):** https://engineer-rama-rao.github.io

## What's here

A single-page static portfolio designed for recruiters and hiring managers:

- Hero with portrait, availability (immediate start, 5 days in office, happy to relocate), stat block (25+ / 9 / 2) and one-click CTAs (CV, email, phone, LinkedIn)
- About / core competencies / technical tools
- Full career timeline (13 roles, TfL → London boroughs → consultancies)
- Selected projects gallery (42 images) with keyboard-navigable lightbox
- **Applied research** — UCL work framed as expertise, not student status
- **Writing & thought leadership** — 10 curated LinkedIn posts
- Credentials & certifications, each linked to its source PDF
- SEO infrastructure: JSON-LD `Person` schema, Open Graph, branded 1200×630 social share card, sitemap, robots
- 404 page and SVG favicon

## Project structure

```
.
├── index.html                       # Main page
├── styles.css                       # All styling
├── script.js                        # Gallery + lightbox
├── 404.html
├── robots.txt
├── sitemap.xml
├── cv/
│   ├── Rama-Rao-CV.pdf              # Downloadable CV
│   ├── Rama-Rao-CV.docx             # Word original
│   └── cv.html                      # HTML source for the PDF
├── assets/
│   ├── rama-portrait.jpg            # Hero portrait
│   ├── icons/
│   │   ├── favicon.svg
│   │   ├── og-image.png             # 1200×630 social share card
│   │   └── og-template.html         # HTML source for the OG card
│   ├── projects/                    # 42 project images
│   └── certifications/              # 9 certificate PDFs/JPG
├── certifications/                  # Source certificates (originals)
├── linkedin_screenshots/            # Source LinkedIn screenshots
└── Rama Portfolio.docx              # Original portfolio source
```

## Local preview

```bash
python3 -m http.server 8000
# open http://localhost:8000
```

## 🚀 Publishing — moving to the new GitHub account

The repo is currently under a development account. The plan is to publish from a new GitHub account owned by Rama so the public URL is clean:

**Target URL:** `https://engineer-rama-rao.github.io`

### Step-by-step

1. **Create a new GitHub account** for Rama at https://github.com/signup using username **`engineer-rama-rao`** (and an email she owns). This matches her existing Lovable handle.
2. **Create a new repo** on that account, named exactly **`engineer-rama-rao.github.io`** (username and repo name MUST match for Pages to serve at the bare URL). Public, no README/.gitignore/LICENSE — empty.
3. From this folder on your machine, add the new remote and push:
   ```bash
   git remote add rama https://github.com/engineer-rama-rao/engineer-rama-rao.github.io.git
   git push rama main
   ```
4. On the new repo's **Settings → Pages**: source = "Deploy from a branch", branch = `main` / root, save.
5. Within ~1 minute the site is live at https://engineer-rama-rao.github.io

### Optional: custom domain later

If you ever want `ramarao.co.uk` (or similar), buy the domain, add a `CNAME` file to the repo root containing the domain, and point DNS at GitHub Pages. Enable HTTPS in Pages settings.

## Maximising recruiter visibility

After deploying, do all of these (each one takes 2 min):

1. **Google Search Console** — add `https://engineer-rama-rao.github.io`, verify (HTML tag method), submit `sitemap.xml`.
2. **Bing Webmaster Tools** — same.
3. **LinkedIn profile**:
   - Update Contact info → add the URL as her website.
   - Add the site to the **Featured** section (most impactful).
   - Update Headline to include "Senior Project & Highway Engineer · Open to opportunities".
   - Pin one of her LinkedIn posts that links to the new site.
4. **CV header** — put the URL in the PDF (already implemented in `cv/cv.html`; regenerate if needed).
5. **Email signature** — add the URL.
6. **Share once on LinkedIn** — the OG card will preview beautifully, drives initial traffic.

## Regenerating artefacts

**CV PDF:**
```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless --disable-gpu --no-pdf-header-footer \
  --print-to-pdf=cv/Rama-Rao-CV.pdf \
  "file://$(pwd)/cv/cv.html"
```

**Social share card (1200×630):**
```bash
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless --disable-gpu --window-size=1200,630 --hide-scrollbars \
  --screenshot=assets/icons/og-image.png \
  "file://$(pwd)/assets/icons/og-template.html"
```

## Credits

Content © Rama H. S. Rao. Site built collaboratively.
