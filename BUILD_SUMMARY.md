# Rama H. S. Rao — Job Search Portfolio Build Summary

A complete inventory of everything built for Rama's job search, designed to be readable by anyone helping out.

**Live site:** https://engineer-rama-rao.github.io
**GitHub repo:** https://github.com/engineer-rama-rao/engineer-rama-rao.github.io
**Status:** Live, indexed in Google & Bing, fully automated for inbound recruiter contact.

---

## 1. Infrastructure set up

| Item | What it is | Where |
|---|---|---|
| GitHub account | `engineer-rama-rao` | https://github.com/engineer-rama-rao |
| Repository | `engineer-rama-rao.github.io` | (public, source for the live site) |
| GitHub Pages | Enabled, HTTPS enforced | Auto-deploys from `main` |
| Calendly | 30-min booking link | https://calendly.com/engineer_rama/30min |
| Backup mirror | `rajathn8/rama.github.io` | Same code, second copy |

---

## 2. The website itself

A single-page static portfolio at **https://engineer-rama-rao.github.io** with 9 numbered sections:

1. **Hero** — name, credentials (`BEng (PhD)`), portrait, availability badges (Available now / Immediate start / Happy to relocate), 6 CTAs (Download CV, Book a call, Email, Call, WhatsApp, Text, LinkedIn), stat block (25+ years / 9 boroughs / 2 fellow memberships), profile card with pill-format Recent Clients / Specialisms / Sectors.
2. **About** — credentials lead line + experience summary, then visual pill grids for Scheme Types Delivered (LCN, LCN+, cycle routes, School Streets, bus priority, etc.) and Direct Delivery On (TLRN, 9 London Borough Councils, surrounding home county authorities).
3. **Experience** — Timeline of 13 roles from 1996 to present (TfL, 9 London boroughs, WSP, etc.) with date column + content cards.
4. **Selected projects** — Gallery of 42 project images (UK highway schemes, India airports, golf resorts) with keyboard-navigable lightbox.
5. **Applied research** — Frames UCL postgraduate research as expertise feeding into delivery (not as student status).
6. **Writing & thought leadership** — 10 curated LinkedIn article links.
7. **Credentials & certifications** — Cards linking to source PDFs (CDM 2015 PD, RSA, PMO, etc.) + Education cards (BEng, Trained Landscape Designer, UCL research).
8. **Roles I'm a strong fit for** — 4 pill-grid blocks: Role titles, Sectors & clients, Contract types, Location. Designed so a recruiter can match her to a vacancy in 5 seconds.
9. **Send Rama a role** — A 10-field form recruiters fill in 60 seconds; clicking submit opens a pre-addressed email with a structured role brief landing directly in Rama's inbox.
10. **Get in touch** — Contact cards (Calendly, Email, Phone, WhatsApp, SMS, LinkedIn, Full CV, 1-page CV) + "Know someone hiring? Share this page" block with LinkedIn / WhatsApp / Email / Copy-link share buttons.

Plus footer with downloads (Full CV, 1-page summary, Word CV, vCard, business card PDF).

### Mobile-responsive
Tested at 360px, 390px (iPhone), 720px, 960px and 1400px. Buttons grid 2-up on mobile, photo crops to square, pills wrap cleanly, timeline collapses with dates above each card.

### Image optimisation
All 42 project images + portrait converted to **WebP** at two sizes (full + thumb). Total image weight dropped from 15.3 MB → 5.7 MB. Mobile loads in ~1 second on 4G.

---

## 3. Downloadable artefacts (under `/cv/` and `/assets/`)

| File | Purpose |
|---|---|
| `cv/Rama-Rao-CV.pdf` | Full 2-page CV |
| `cv/Rama-Rao-CV-1page.pdf` | 1-page summary recruiters can skim in 6 seconds |
| `cv/Rama-Rao-CV.docx` | Original Word source |
| `assets/Rama-Rao.vcf` | vCard — recruiter taps once on phone, contact saved |
| `assets/business-card.pdf` | Printable 85×55mm card with QR code linking to portfolio |
| `assets/icons/qr-portfolio.png` & `.svg` | QR code for in-person/print use |
| `assets/icons/og-image.png` | Branded 1200×630 social preview (navy + gold) |

---

## 4. Inbound automation — zero effort on Rama's side

Every channel below works without her lifting a finger. Recruiters self-serve.

| Channel | How it works |
|---|---|
| **Calendly** | One click → recruiter picks a 30-min slot → lands in her calendar |
| **WhatsApp deep-link** | One tap on phone → chat opens pre-filled "Hi Rama, we're hiring for [role]" |
| **SMS deep-link** | Same as above but via text |
| **"Send Rama a role" form** | Recruiter fills 60s, clicks submit, builds structured email pre-addressed to her |
| **Hotmail auto-responder** | (template provided; Rajath sets up) Every email gets the portfolio + CV + Calendly reply automatically |
| **Refer-me share buttons** | Network shares the site via LinkedIn / WhatsApp / Email / Copy-link with one click |
| **vCard download** | One tap saves Rama's contact details to recruiter's phone |
| **JobPosting schema** | Recruiter-side AI tools (Lusha, Apollo, LinkedIn Recruiter) index her as "live open candidate" |

---

## 5. SEO and discoverability — "visible from the moon" mode

### Structured data (6 JSON-LD blocks)
Person, WebSite, ProfilePage, JobPosting (her as the open candidate), FAQPage (6 recruiter questions = rich snippets in Google), BreadcrumbList.

### Search engines registered
- **Google Search Console** — verified via HTML file, sitemap submitted.
- **Bing Webmaster Tools** — verified via BingSiteAuth.xml.
- **IndexNow** — URLs submitted to Bing, Yandex, Seznam (Czech), aggregator.

### AI / LLM crawlers explicitly welcomed in `robots.txt`
GPTBot, ChatGPT-User, OAI-SearchBot, ClaudeBot, anthropic-ai, PerplexityBot, CCBot (Common Crawl), Bytespider, Applebot-Extended, Google-Extended, MistralAI-User, cohere-ai, Amazonbot, FacebookBot, LinkedInBot, PiplBot, archive.org_bot, plus the standard Googlebot/Bingbot/DuckDuckBot stack.

### LLM-readable resume
`llms.txt` — an emerging plain-text format that AI search tools (ChatGPT search, Perplexity, Claude with web access) read directly. Lists every role type, sector, qualification, work history with an explicit "available immediately" signal.

### Meta files
- `humans.txt` — team/credentials/status
- `ai.txt` — explicit AI training/embed/cite allow
- `ads.txt` — no ad relationships (professional signal)
- `.well-known/security.txt` — RFC 9116 compliance
- `feed.xml` — RSS subscription for her availability

### Image sitemap
All 42 project images + portrait + OG card listed for Google Images.

### Geographic SEO signals
`geo.region: GB-LND`, `ICBM: 51.5074, -0.1278`, `og:locale: en_GB` — Google Knowledge Graph builds her people-card for London-area searches.

---

## 6. Outreach materials prepared (delivered in chat — not on the public site)

| Asset | What it covers |
|---|---|
| 12 specialist recruiter list | UK highway-engineering agencies + phone numbers + email template |
| 30 named target organisations | London boroughs, top 10 consultancies, term contractors with hiring-manager email template |
| 4 cover-letter variants | Public sector / Consultancy / Day-rate contract / Cold recruiter intro |
| Warm-intro LinkedIn DM template | For ex-colleagues at WSP, Atkins, AECOM, etc. |
| Hiring-manager direct cold email | Bypasses recruiters |
| Live vacancies hit-list | Hillingdon Council, LB Newham, Morson Edge (Band 3+ £520/day) |
| 11 jobs platforms | LinkedIn, Indeed UK, TotalJobs, CV-Library, Reed, CIHT Jobs, IHE Jobs, ICE Recruit, LocalGov Jobs, Highways Magazine, GOV.UK Find a Job |
| Hotmail auto-responder text | 5-min setup, runs while she's busy |
| LinkedIn headline / About / Featured / Open-to-Work instructions | Profile optimisation steps |
| Email signature with the portfolio URL | Drop-in text |

---

## 7. Tooling and workflow

- **No paid services used.** Everything is on free tiers or self-hosted.
- **Site framework:** Plain static HTML + CSS + JS, hosted on GitHub Pages. No build step, no framework.
- **CV PDFs:** Generated from HTML via Chrome headless `--print-to-pdf` (no LibreOffice/Word dependency).
- **OG image:** 1200×630 PNG rendered from HTML via Chrome headless screenshot. Branded navy + gold to match the site.
- **QR code:** Python `qrcode` library, generates both PNG and scalable SVG.
- **Image optimisation:** Python Pillow, batch-converted to WebP at two sizes.
- **Multi-account git push:** GitHub CLI (`gh auth login` / `gh auth switch`) — keeps `engineer-rama-rao` and `rajathn8` accounts cleanly separated locally.
- **Cache-busting:** CSS/JS links include `?v=` query strings so recruiters never see stale styles mid-deploy.

---

## 8. What still requires Rama or Rajath to do manually

These need a human login and can't be automated.

| Action | Where | Time | Why it matters |
|---|---|---|---|
| Set LinkedIn "Open to Work" to **Recruiters only** | LinkedIn profile | 2 min | Single biggest LinkedIn Recruiter visibility lever |
| Add the portfolio URL to LinkedIn **Featured** section | LinkedIn profile | 3 min | Top of profile, biggest single touchpoint |
| Update LinkedIn **Headline** to "Senior Project & Highway Engineer · Open to opportunities" | LinkedIn profile | 1 min | First thing recruiters read |
| Update LinkedIn **About** section using the rewrite provided | LinkedIn profile | 3 min | Removes "PhD student" framing |
| Set up the **Hotmail auto-responder** with the template provided | Outlook.live.com | 5 min | Runs while she's busy |
| Verify her **CIHT / IHE** Fellow public listings include the portfolio URL | ciht.org.uk + theihe.org | 5 min each | High-authority backlinks |
| Apply to the **Hillingdon Council Highway Engineer** vacancy directly | jobs.hillingdon.gov.uk | 10 min | Warm internal application |
| Email the **12 specialist recruiters** with the cold-email template | Email | 60 min | Each one likely has a live unadvertised role |
| Register on the **11 jobs platforms** and set up alerts | Various | 90 min total | Catches every new vacancy within minutes |

---

## 9. Repository layout

```
engineer-rama-rao.github.io/
├── index.html                    # Main page
├── styles.css                    # All styling
├── script.js                     # Gallery + lightbox + intake form
├── 404.html
├── sitemap.xml                   # All URLs + image sitemap
├── feed.xml                      # RSS feed for availability
├── robots.txt                    # AI/LLM crawlers welcomed
├── llms.txt                      # LLM-readable resume
├── humans.txt
├── ai.txt
├── ads.txt
├── google7009d0600350d94a.html   # Google Search Console verification
├── BingSiteAuth.xml              # Bing verification
├── d135f6d9...txt                # IndexNow verification key
├── .well-known/
│   └── security.txt
├── cv/
│   ├── Rama-Rao-CV.pdf
│   ├── Rama-Rao-CV-1page.pdf
│   ├── Rama-Rao-CV.docx
│   ├── cv.html                   # Source for full CV PDF
│   └── cv-onepager.html          # Source for 1-page PDF
├── assets/
│   ├── rama-portrait.{jpg,webp}  # Hero photo + responsive variants
│   ├── Rama-Rao.vcf              # vCard
│   ├── business-card.pdf         # Printable card
│   ├── icons/
│   │   ├── favicon.svg
│   │   ├── og-image.{png,webp}   # Social share card
│   │   ├── og-template.html      # Source
│   │   ├── card-template.html    # Source for business card
│   │   ├── qr-portfolio.{png,svg}
│   ├── projects/                 # 42 project images (JPG/PNG + WebP variants)
│   └── certifications/           # 9 source certificate PDFs/JPG
├── linkedin_screenshots/         # Source LinkedIn snapshots for content
└── Rama Portfolio.docx           # Original source document
```

---

## 10. How to make changes

If anything needs editing (e.g. correcting a credential, swapping a phone number), the workflow is:

```bash
cd /Users/rajathrao/Documents/GitHub/rama.github.io
# 1. Edit the relevant file (index.html, llms.txt, cv/cv.html, etc.)
# 2. If you edited cv/cv.html or cv/cv-onepager.html, regenerate the PDF:
"/Applications/Google Chrome.app/Contents/MacOS/Google Chrome" \
  --headless --disable-gpu --no-pdf-header-footer \
  --print-to-pdf=cv/Rama-Rao-CV.pdf \
  "file://$(pwd)/cv/cv.html"
# 3. Commit:
git add -A && git commit -m "describe the change"
# 4. Push to both remotes:
gh auth switch --user engineer-rama-rao && git push rama main
gh auth switch --user rajathn8 && git push origin main
```

GitHub Pages rebuilds in ~60 seconds after each push.

---

**Built with care to maximise Rama's inbound recruiter contact while she has zero time to do outbound search.**
