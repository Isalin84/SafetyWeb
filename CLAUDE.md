# SafetyWeb — Напитки Вместе

## Project
Single-file safety landing page for "Напитки Вместе" beverage company.
Output: `index.html` (standalone, no build step, no dependencies).
Language: Russian (all copy, filenames, and labels).

## Assets
All assets live in `Assets/` — filenames are Cyrillic, browsers handle encoding automatically.
- `Assets/Политика Напитки Вместе в области охраны труда и здоровья.pdf` — safety policy
- `Assets/asessment/Уфа СОУТ.pdf` — SOУТ report (note: folder spelled `asessment`, single `s`)
- `Assets/SAFE_2_5_1_НВ_План_управления_безопасностью.docx` — contractor safety plan

## Design System
Dark theme. Font: `Outfit` (Google Fonts). Single accent: emerald (`#16a34a`).
Base: slate-900 (`#0f172a`), surface: slate-800 (`#1e293b`).
Animations: CSS only (`transform`/`opacity`). Scroll reveals via IntersectionObserver.
Skill used: `taste-skill` — enforces no emojis, no Inter font, no centered hero, `min-h-[100dvh]`.

## Key URLs
- Company principles (Principle #8): https://napitkivmeste.ru/nasha-tsel-i-printsipy/
- Sustainable development: https://napitkivmeste.ru/ustojchivoe-razvitie/
- Video embed (Kinescope): https://kinescope.io/embed/79vonkjwqvwoee5UtkV8mt

## Page Sections (in order)
1. Sticky nav — glassmorphism, mobile hamburger toggle
2. Hero — asymmetric split (52/48), video right, `min-height: 100dvh`
3. Stats bar — 4 metrics (Principle 8 / 100% training / СОУТ / zero injuries)
4. Principle #8 — giant decorative numeral, blockquote, external link
5. Documents hub — asymmetric grid (`policy` spans 2 rows left, СОУТ + contractor stacked right)
6. Contractors — requirements list + CTA card with DOCX download
7. Safety culture — 6-pillar grid (3-col → 2-col → 1-col)
8. Sustainable development strip
9. Footer — 3-col: brand / nav / docs

## Gotchas
- `Assets/asessment/` has ONE `s` — do not autocorrect to `assessment`
- No React, no npm, no build step — pure HTML/CSS/JS
- Firebase debug log exists (`firebase-debug.log`) but Firebase is not configured
