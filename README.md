# Peroche Business Intelligence Unit
### Carolina Aguayo — Experience Economy Desk

**Live site:** https://jfcarpiopuntocom.github.io/carolina_aguayo/  
**Contact:** hello@peroche-strategies.com  
**Markets:** Americas — hospitality, tourism, real estate

---

## What this is

Single-page website for Peroche BIU — Carolina Aguayo's boutique intelligence firm delivering sector-specific reports, dashboards, and ad hoc studies to family offices, investment groups, and executive teams across the Americas.

No framework. No build step. One HTML file.

---

## File structure

```
carolina_aguayo/
├── index.html              ← the entire site (HTML + CSS + JS, self-contained)
├── index_files/
│   ├── logo.jpg            ← Peroche logo (used in nav, footer, CTA)
│   └── css2.css            ← Google Fonts local cache (Inter + Playfair Display)
├── peroche-dashboard.jpg   ← Featured work: BI dashboard sample
├── peroche-report.jpg      ← Featured work: Experience Economy Report cover
└── peroche-testimonial.jpg ← J.F. Carpio recommendation screenshot
```

---

## How to edit

Open `index.html` in any editor. Everything lives in one file:
- **Styles:** `<style>` block in `<head>` — CSS variables at the top under `BRAND TOKENS`
- **Content:** HTML body — sections are clearly commented (`─── HERO`, `─── SERVICES`, etc.)
- **Behavior:** `<script>` block at the bottom — scroll reveal + card tilt + nav hover

Before any edit, make a timestamped backup:
```bash
cp index.html index_2026-MM-DD_HH-MM.html
chmod 444 index_2026-MM-DD_HH-MM.html
```

---

## Brand rules (do not break these)

| Token | Value | Use |
|---|---|---|
| `--midnight` | `#0B0B0D` | Page background |
| `--charcoal` | `#121316` | Section / card backgrounds |
| `--warm-gold` | `#C8A36B` | Primary accent, labels, icons |
| `--champagne` | `#E7D3A8` | Secondary accent, strong text |
| `--ember` | `#C75A44` | CTA band, testimonial bar, heat accents |
| `--off-white` | `#F0EBE1` | Primary text |
| `--muted` | `#999999` | Body / secondary text (never below #999) |

**Typography:**
- Headings / quotes / numbers: `Playfair Display` (serif, elegant)
- Body / labels / UI: `Inter` (sans-serif, precise)

**Absolute rules:**
- No `opacity` on any text element, ever
- No `rgba()` for text colors — solid hex only
- No font-size below `0.82rem` anywhere visible
- Mobile-first CSS always

---

## Deploy

Site runs on GitHub Pages from the `main` branch root. Push to `main` and the live URL updates automatically in ~30 seconds. No build, no CI, no config needed.

```bash
git add index.html
git commit -m "your change description"
git push origin main
```

---

## Services offered

| Service | Description |
|---|---|
| BI Reports | Deep-dive sector briefs — hospitality, tourism, alternative investments |
| Dashboards | Live occupancy, RevPAR, ADR, market share — tailored to portfolio |
| Ad Hoc Studies | Custom research: feasibility, due diligence, site selection, competitive positioning |

**Offices:** New York City · Quito · Guayaquil
