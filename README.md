# FlowPilot — marketing website for an HR-tech studio

**Live:** https://flowpilot-site.den-danchenkoo.workers.dev

Marketing website for **FlowPilot**, a studio that builds websites, CRM systems and automations for recruitment agencies in Poland.
A single, dependency-free static page with a premium dark design, animated product mockups and a Polish-language sales funnel, deployed on Cloudflare.

![FlowPilot website — desktop](docs/desktop.png)

<p align="center"><img src="docs/mobile.png" alt="FlowPilot website — mobile" width="300"></p>

## Highlights

- **Zero-build static site** — one `index.html` with inline CSS and vanilla JavaScript; nothing to install to run it.
- **Animated hero** — canvas scene with a day/night phase, a live CRM dashboard mockup and counters that animate into view (`IntersectionObserver`).
- **Animation that respects the device** — loops pause when the tab is hidden and pause off-screen, so the page stays light on battery and CPU.
- **Responsive images** — separate desktop and mobile backgrounds (2400 px / 1400 px), served with year-long immutable caching.
- **Security headers** — `X-Content-Type-Options`, `Referrer-Policy`, `X-Frame-Options` and a restrictive `Permissions-Policy` via `_headers`.
- **SEO and sharing** — description, Open Graph tags and a theme colour.
- **Full sales funnel** — products, solutions, implementation process, pricing, FAQ and contact form.

## Structure

```
public/
├── index.html     Page, styles and scripts
├── img/           Desktop and mobile backgrounds
├── favicon.svg
├── robots.txt
└── _headers       Caching and security headers
wrangler.jsonc     Cloudflare Workers static-assets deployment
```

## Run locally

Open `public/index.html` in a browser, or use the Cloudflare dev server:

```bash
npm install
npm run dev       # http://localhost:8787
npm run deploy    # deploy to Cloudflare Workers
```

## Tech

HTML5 · CSS3 · vanilla JavaScript (Canvas, IntersectionObserver) · Cloudflare Workers static assets

## Author

Designed and built by **Denis Danchenko** — AI automation, CRM and web developer.
Available for projects on [Upwork](https://www.upwork.com/freelancers/~016707bca373f53f65).

---

© 2026 FlowPilot. The source is published as a portfolio sample; the brand, copy and images are not licensed for reuse.
