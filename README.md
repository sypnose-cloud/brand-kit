# SYPNOSE — Brand Identity Bundle

**Mithos Edition · v1.1 · 12 May 2026**

Complete corporate identity system for **Sypnose Mithos** — the AI worker orchestration platform built by Carlos De La Torre, Architect of SYPNOSE.

> *"One command. Entire AI organization."*

Eight deliverable blocks, all built to the **Iron Rule**: no claim without a metric, no asset without a purpose.

**What's new in v1.1**
- Block 05 · native editable **`.pptx`** export (1920×1080, 15 slides + speaker notes)
- Block 08 · expanded from 18 → **36 social templates** (12 typologies × 3 dimensions)

---

## ▌ Bundle contents

```
sypnose-identity/
├── README.md                       ← this file
├── BRAND-PALETTE.md                ← quick color/font reference
├── index.html                      ← navigable hub for all 8 blocks
│
├── Logo System.html                ← Block 01 · 12 variants + 12×12 grid
├── Favicon Set.html                ← Block 02 · 10 favicons + manifest.json
├── Email Signatures.html           ← Block 03 · 6 signatures (min/full/promo × light/dark)
├── Business Cards.html             ← Block 04 · print 85×55mm + digital vCard QR
├── Pitch Deck.html                 ← Block 05 · 15 slides + speaker notes (1920×1080)
├── Brand Guidelines.html           ← Block 06 · 22-page printable A4 brand book
├── Email Transactional.html        ← Block 07 · 6 SaaS emails (welcome, quota, fail, POC, invoice, digest)
├── Social Templates.html           ← Block 08 · 12 typologies × 3 dimensions = 36 templates
│
├── assets/
│   ├── symbol.svg                  ← canonical symbol vector
│   └── Sypnose-Pitch-Deck-v1.1.pptx ← ★ native editable PowerPoint (722 KB)
├── favicons/                       ← 10 SVG favicon variants + manifest.json + browserconfig.xml
├── signatures/                     ← 6 standalone signature HTML files
├── site.webmanifest                ← PWA manifest for sypnose.cloud
└── deck-stage.js                   ← slide deck runtime
```

---

## ▌ The mark, in one paragraph

A single architect hub (terra cotta `#da7756`) at the center, six worker satellites (slate `#3d3929`) on a hex perimeter, six radial spokes for the A2A bus. It is a literal diagram of the Sypnose orchestrator — not abstract, not decorative. Built on a 12×12 unit grid, hub Ø 4u, satellites Ø 2u, clearspace 1u on all sides.

## ▌ Palette · strict

| Role | HEX | RGB | CMYK | Pantone | Use |
|---|---|---|---|---|---|
| Terra Cotta | `#DA7756` | 218 · 119 · 86 | 0 · 55 · 65 · 0 | 165 C | Accent, hub, CTA |
| Cream | `#EEECE2` | 238 · 236 · 226 | 5 · 4 · 11 · 0 | Warm Gray 1 | Daylight ground |
| Dark Slate | `#3D3929` | 61 · 57 · 41 | 55 · 56 · 75 · 65 | 7531 C | Type, night ground |

**60 / 30 / 10 rule** — Cream fills 60%, slate fills 30%, terra fills 10%. Never invert.

## ▌ Type stack

| Family | Weights | Use |
|---|---|---|
| **Poppins** | 400 / 500 / 600 / 700 / 800 | Wordmark, headings, display |
| **Lora** | 400 / 500 / 600 (+ italics) | Pull quotes, manifesto lines, monogram |
| **DM Sans** | 400 / 500 / 600 / 700 | Body, UI, captions, forms |
| **JetBrains Mono** | 400 / 500 / 600 | Code, CLI, meta tags, tickers |

All four ship through Google Fonts under the OFL — safe to embed in production.

---

## ▌ Voice & tone

**The Iron Rule applies to copy:** *no proof, no done*. If a sentence claims "fast," it must show milliseconds. If it claims "reliable," it must show the error count. If no metric exists, cut the sentence.

### Metrics that are real (verified, May 2026)

- **300** workers — maximum parallel pool
- **47** models — routed across Claude / GPT / Gemini / Mistral
- **741 ms** — agent-to-agent end-to-end latency (incl. memory hydration)
- **93 %** — first-pass review rate
- **95 %** — compute on free tiers across 11 providers
- **4-year** — memory horizon (Postgres + pgvector)
- **1,708** — knowledge entries indexed
- **43** — active projects
- **5** — products in production
- **314** — paying clients on GestoriaRD
- **312** tasks · **0** errors · 9 agents — overnight benchmark
- **512K** — lines of Claude Code source audited
- **27 h** — Stratos trading console end-to-end ship time
- **6 h** — HUYGHU full brand kit build time
- **1** — VPS running all 5 products

### Never say

- "Cutting-edge", "revolutionary", "best-in-class", "unprecedented"
- "AI Engineer", "ML Engineer" — Carlos is **Architect of SYPNOSE**
- Any superlative without a number under it

---

## ▌ Pricing (canonical)

| Tier | Price | Includes |
|---|---|---|
| **Agent Free** | $0 forever, BYO keys | 300 workers, full memory, all 47 models, MIT |
| **★ Agent Sypnose** | **$2,400 / mo · 5 seats** | Managed compute, hosted memory, Grafana, overnight queue, Slack channel |
| **Agent Platform** | Custom annual | VPC deploy, SOC 2, SSO, dedicated architect |

**6-hour POC** — free. We ship one real feature on Sypnose, tests included. Email `hello@sypnose.cloud`.

---

## ▌ Deploy to `github.com/sypnose-cloud`

This bundle lives alongside the public Sypnose orgs:

- **`sypnose-cloud/agent-free`** — MIT, the free CLI
- **`sypnose-cloud/agent-sypnose`** — MIT, the Business tier
- **`sypnose-cloud/brand`** ← **this bundle**

### Step 1 — create the brand repo

```bash
gh repo create sypnose-cloud/brand \
  --public \
  --description "Sypnose Mithos — corporate identity bundle (v1.0)" \
  --license MIT
```

### Step 2 — clone, copy, commit

```bash
git clone git@github.com:sypnose-cloud/brand.git
cd brand
cp -r /path/to/sypnose-identity/* .
git add .
git commit -m "feat: v1.0 — Mithos identity bundle (8 blocks, Iron Rule compliant)"
git push origin main
```

### Step 3 — publish the site

```bash
# the entire bundle is static HTML — drop on Cloudflare Pages
wrangler pages deploy . --project-name=sypnose-brand
# → https://brand.sypnose.cloud
```

### Step 4 — wire the favicons

Copy these files (or their PNG exports from `Favicon Set.html`) to your site root:

```
/icons/favicon-16.png
/icons/favicon-32.png
/icons/favicon-48.png
/icons/apple-touch-icon.png
/icons/android-chrome-192.png
/icons/android-chrome-512.png
/icons/maskable-icon-512.png
/icons/safari-pinned-tab.svg
/icons/mstile-150.png
/og-image.png
/site.webmanifest
```

The full `<head>` snippet is in **Favicon Set.html § 02.D** — copy-paste ready.

### Step 5 — `.gitignore`

```gitignore
.DS_Store
node_modules/
dist/
.wrangler/
```

### Repo conventions

- **Branching** — `main` is the deployed brand. Open PRs against `next` for v1.1 work.
- **Commits** — Conventional Commits. `feat:`, `fix:`, `chore:`, `docs:`.
- **Versioning** — semver on the bundle as a whole. Tag releases (`v1.0`, `v1.1`).
- **License** — MIT. Use is free for Sypnose customers, partners, and press. Use of the mark requires written permission via `hello@sypnose.cloud`.

---

## ▌ How to use each block

| Block | Source of truth | Use it when |
|---|---|---|
| 01 Logo System | `Logo System.html` | You need a variant of the mark. Never modify — pick another. |
| 02 Favicon Set | `Favicon Set.html` | Any new web property under sypnose.cloud. |
| 03 Email Signatures | `Email Signatures.html` | Copy the HTML directly into Gmail / Superhuman signature editor. |
| 04 Business Cards | `Business Cards.html` | Print run · vCard QR generation. |
| 05 Pitch Deck | `Pitch Deck.html` + `assets/Sypnose-Pitch-Deck-v1.1.pptx` | Sales calls for Business tier. Open the HTML for the live deck, or the PPTX for PowerPoint / Keynote editing. Speaker notes embedded in both. |
| 06 Brand Guidelines | `Brand Guidelines.html` | Onboarding new contributors. Print to PDF via the ▶ button. |
| 07 Email Transactional | `Email Transactional.html` | Wire into the SaaS — copy the table HTML, swap merge tags. |
| 08 Social Templates | `Social Templates.html` | Any post to LinkedIn / IG. **12 typologies** × 3 dimensions = 36 templates. Do not invent a thirteenth. |

---

## ▌ Contact

| | |
|---|---|
| **Architect** | Carlos De La Torre |
| **Role** | Architect of SYPNOSE |
| **Email** | `carlos@huyghusrl.com` · `hello@sypnose.cloud` |
| **Tel** | +1 809 424 0731 (WhatsApp) |
| **Web** | [sypnose.cloud](https://sypnose.cloud) |
| **GitHub** | [github.com/sypnose-cloud](https://github.com/sypnose-cloud) |
| **LinkedIn** | [linkedin.com/in/carlosdelatorre-ai](https://linkedin.com/in/carlosdelatorre-ai) |
| **Address** | Puerto Plata, Dominican Republic |
| **Live since** | January 2026 |

---

## ▌ License

MIT — the bundle, the code, the assets. **The mark itself** (the hub-and-six-satellites symbol and the "sypnose" wordmark) is © 2026 SYPNOSE · use requires written permission.

---

**SYPNOSE © 2026** · *No proof, no done.*

---

## ▌ Changelog

### v1.1 · 12 May 2026
- **Block 05** · added native editable `Sypnose-Pitch-Deck-v1.1.pptx` (15 slides, 1920×1080, speaker notes attached)
- **Block 08** · expanded from 18 → 36 social templates (added 6 typologies: testimonial, partnership, jobs ladder, behind-the-scenes, milestone, comparison)

### v1.0 · 12 May 2026
- Initial release · all 8 blocks shipped
- Logo System, Favicons, Signatures, Business Cards, Pitch Deck (HTML), Brand Guidelines, Email Transactional, Social Templates (18)
