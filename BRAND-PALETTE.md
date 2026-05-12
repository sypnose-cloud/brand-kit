# SYPNOSE · Brand Palette · Quick Reference

**v1.0 · 12 May 2026 · canonical since 26 March 2026**

---

## ▌ Primary palette · three colors, no fourth

| Token | HEX | RGB | OKLCH | CMYK | Pantone |
|---|---|---|---|---|---|
| **Terra Cotta** (`--terra`) | `#DA7756` | 218 · 119 · 86 | 65% · 0.13 · 50° | 0 · 55 · 65 · 0 | 165 C |
| **Cream** (`--cream`) | `#EEECE2` | 238 · 236 · 226 | 94% · 0.01 · 95° | 5 · 4 · 11 · 0 | Warm Gray 1 |
| **Dark Slate** (`--slate`) | `#3D3929` | 61 · 57 · 41 | 28% · 0.02 · 80° | 55 · 56 · 75 · 65 | 7531 C |

**Ratio · 60 / 30 / 10** — cream is the ground, slate is the structure, terra is the spark. Never invert.

## ▌ Extended scale

| Token | HEX |
|---|---|
| `--terra-deep` | `#B85F3F` |
| `--terra-soft` | `#E89A7D` |
| `--cream-2` | `#E6E2D2` |
| `--cream-3` | `#DCD7C4` |
| `--slate-2` | `#5A5443` |
| `--slate-3` | `#8A8472` |
| `--slate-4` | `#2A261B` (terminal background) |

## ▌ Functional · UI state only

| Token | HEX | Use |
|---|---|---|
| `--success` | `#5B8A72` | Pass · OK · 0 errors |
| `--warning` | `#D9A45A` | 80% quota · deprecation notices |
| `--danger` | `#C25B4C` | Build fail · 401 · `exit_code != 0` |
| `--info` | `#5A7A9E` | Neutral status badges |

Never use functional colors in print, social, or pitch material. UI only.

## ▌ Code block tokens

| Token | HEX | Maps to |
|---|---|---|
| `--code-bg` | `#2A261B` | terminal ground |
| `--code-prompt` | `#DA7756` | `$` prompt |
| `--code-ok` | `#A3C9AA` | `✓` lines |
| `--code-warn` | `#E8C068` | `⚡` lines |
| `--code-err` | `#E09080` | `✕` lines |
| `--code-comment` | `#7A7460` | `#` italic |
| `--code-string` | `#CFB98A` | strings |

---

## ▌ Type stack

| Family | Weights | Use | Tracking |
|---|---|---|---|
| **Poppins** | 400 / 500 / 600 / 700 / 800 | Wordmark, headings, display, button labels | Display −1.5 → −4 px · Headings −0.5 → −1 px |
| **Lora** (regular + italic) | 400 / 500 / 600 | Pull quotes, manifesto lines, monogram, ledes | One italic line per surface, max |
| **DM Sans** | 400 / 500 / 600 / 700 | Body, UI, forms, captions, tables | 0 → +0.3 px |
| **JetBrains Mono** | 400 / 500 / 600 | Code, CLI, meta tags, tickers, all-caps chrome | UPPERCASE 1.5 → 2.5 px |

All four available on Google Fonts under OFL. Always preload the four families together — there is no fallback that doesn't break the typesetting.

```html
<link href="https://fonts.googleapis.com/css2?family=DM+Sans:wght@400;500;600;700&family=Lora:ital,wght@0,400..600;1,400..600&family=Poppins:wght@400;500;600;700;800&family=JetBrains+Mono:wght@400;500;600&display=swap" rel="stylesheet">
```

## ▌ CSS tokens — drop-in

```css
:root{
  /* primary */
  --terra:#da7756;
  --terra-deep:#b85f3f;
  --terra-soft:#e89a7d;
  --cream:#eeece2;
  --cream-2:#e6e2d2;
  --cream-3:#dcd7c4;
  --slate:#3d3929;
  --slate-2:#5a5443;
  --slate-3:#8a8472;
  --slate-4:#2a261b;

  /* functional */
  --success:#5b8a72;
  --warning:#d9a45a;
  --danger:#c25b4c;
  --info:#5a7a9e;

  /* type */
  --font-display:'Poppins',ui-sans-serif,system-ui,sans-serif;
  --font-serif:'Lora',ui-serif,Georgia,serif;
  --font-body:'DM Sans',ui-sans-serif,system-ui,sans-serif;
  --font-mono:'JetBrains Mono',ui-monospace,'SF Mono',monospace;

  /* rule */
  --rule:rgba(61,57,41,.14);
  --rule-strong:rgba(61,57,41,.28);
}
```

---

**SYPNOSE © 2026** · *No proof, no done.*
