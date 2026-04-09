# KAIRI Analytics

> AI-powered business dashboard platform for SMEs — multilingual landing page with live interactive demo, real-time KPIs, and integrated Claude AI analysis.

🌐 **Live site:** [kairi-analytics.com](https://kairi-analytics.com)

---

## Overview

KAIRI Analytics helps small and medium businesses replace manual Excel reports with intelligent dashboards that update automatically, surface what matters, and detect problems before they become visible in a spreadsheet.

This repository contains the full multilingual landing page with an embedded interactive demo dashboard powered by the Claude API.

---

## Features

- **Trilingual** — full site in English, German and Spanish with automatic browser language detection
- **Live demo dashboard** — interactive sales KPIs, Chart.js visualizations, regional filters, and automatic alerts
- **AI analysis** — integrated Claude API delivering real-time executive summaries and natural language Q&A over business data
- **Netlify Forms** — contact form submissions delivered directly to email, zero backend required
- **Zero dependencies** — pure HTML + CSS + vanilla JS, no framework, no build step
- **One-click deploy** — drop into any static host (Netlify, GitHub Pages, Vercel)

---

## Stack

| Layer | Technology |
|---|---|
| Frontend | HTML5 · CSS3 · Vanilla JavaScript |
| Charts | Chart.js 4.4.1 |
| AI engine | Claude API (claude-sonnet-4) |
| Forms | Netlify Forms |
| Hosting | Netlify + custom domain |
| DNS | Namecheap → Netlify DNS |
| Email | Zoho Mail (`kontakt@kairi-analytics.com`) |

---

## Structure

```
kairi-analytics/
├── index.html          # Language detector — auto-redirects by browser locale
├── es/
│   └── index.html      # Spanish version
├── en/
│   └── index.html      # English version
└── de/
    └── index.html      # German version
```

---

## Deploy

### Netlify (recommended)

1. Fork or clone this repo
2. Connect to [Netlify](https://netlify.com) via "Import from Git"
3. No build command needed — publish directory is `/`
4. Add your custom domain in **Domain management**

### GitHub Pages

1. Push to any public repo
2. Enable GitHub Pages from **Settings → Pages → Deploy from branch**
3. Site available at `yourusername.github.io/kairi-analytics`

---

## Local development

No build step required. Open any `index.html` directly in your browser or serve with any static server:

```bash
# Python
python -m http.server 8000

# Node
npx serve .
```

---

## AI integration

The dashboard uses the Claude API for two features:

- **Automatic analysis** — on page load, Claude generates a 3-sentence executive summary of the current KPI state
- **Q&A** — users can ask free-form questions about the data in natural language

The API key is handled server-side by the Netlify proxy — no key is exposed in the frontend.

---

## Services & pricing

| Package | Price | Delivery |
|---|---|---|
| Starter | €500 | 5 days |
| Business | €1,200 | 7 days |
| AI-Powered | €2,400 | 10 days |
| Monthly maintenance | from €150/mo | ongoing |

---

## Author

**Kent Valera Chirinos**
ML Engineer · AI Dashboard Developer · Founder @ KAIRI Analytics

- 🌐 [kairi-analytics.com](https://kairi-analytics.com)
- 💼 [LinkedIn](https://linkedin.com/in/kent-valera-chirinos-44ba721b)
- 📧 kontakt@kairi-analytics.com
- 📍 Dresden, Germany

---

## Related projects

| Project | Description |
|---|---|
| [KAIRI Sentient Nexus](https://github.com/kentvalerach) | Algorithmic crypto trading system — LONG/SHORT ML models in live production on Bitget/OKX |
| KAIRI-SIO-SATELITAL | Satellite flood early warning system for Spanish Mediterranean basins (Google Earth Engine + Streamlit) |
| KAIRI-SIO | Hydrological signal integrity verification system — 260K+ observations, 2015–2024 |

---

*Built with Python · PostgreSQL · LightGBM · Streamlit · Google Earth Engine · Claude API*
