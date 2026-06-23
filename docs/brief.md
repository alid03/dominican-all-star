# Dominican All Star — Claude Code Project Brief

## What this is
A static website for **Dominican All Star Barbershop & Glam Dominican Salon** in Marietta, GA.
One HTML file, one CSS (inline in the HTML), one JS (inline). No frameworks. No build tools. Pure HTML/CSS/JS.

## File structure
```
dominicanAllStar/
├── site/
│   ├── index.html        ← the entire site lives here
│   └── assets/
│       └── images/       ← all photos, already named
│           ├── hero-barber-hot-towel.jpg
│           ├── gallery-01-cornrows-fade.jpg
│           ├── gallery-02-slickback-high-fade-beard.jpg
│           ├── gallery-03-action-locs-design.jpg
│           ├── gallery-04-low-fade-waves.jpg
│           ├── gallery-05-braids-fade-beard.jpg
│           ├── gallery-06-slickback-detail.jpg
│           ├── gallery-07-kids-cut-fade.jpg
│           ├── gallery-08-action-waves-banner.jpg
│           ├── gallery-09-curly-rizo-taper.jpg
│           ├── gallery-10-taper-textured-beard.jpg
│           ├── gallery-11-afro-taper.jpg
│           └── gallery-12-action-twists-star.jpg
├── media/                ← original unedited photos (don't touch)
└── docs/
```

## The business
- **Dominican All Star Barbershop** — Suite A
- **Glam Dominican Salon** — Suite B (next door, same address)
- **Address:** 677 Franklin Gateway SE, Marietta, GA 30067
- **Barber phones:** (678) 540-3610 · (917) 615-7092
- **Salon phone:** (770) 421-8380
- **Owner/head barber:** Adrian
- **Other barbers:** Juan, Kelvin, Felipe, Suerto, Noel (+ more, 7+ total)
- **Walk-ins ONLY** — never say "book" or "appointment"
- **Hours barber:** Mon–Thu 10am–8pm · Fri–Sat 9am–8:30pm · Sun 10am–5pm
- **Hours salon:** Mon–Thu 10am–7pm · Fri–Sat 9am–9pm · Sun 10am–7pm
- **Socials:** Facebook @AllStarDominicanBarbershop · YouTube @allstardominicanbarbershop9646 · Instagram @glamdominicansalon · TikTok: all-star-dominican-barber
- **Nearby landmark:** Casa Grande Bar & Grill is literally next door on Franklin Gateway

## Design direction
The reference site is **mycasagrande.com** — same street, same neighborhood energy.
Study it. The goal is that same feel: clean, real, confident, local business that takes itself seriously.

### What makes Casa Grande work (copy this approach):
- Fonts: **Bebas Neue** for display/headings, **Montserrat** for labels/nav/UI, **Bitter** for body serif, **Lato** for body sans — load all via Google WebFont loader
- Alternating sections: white → dark (#1a1010) → light grey (#f5f2ef) → dark → white. Never same background twice in a row
- No scroll animations, no elements flying in. Everything is just THERE when the page loads
- Photos do the heavy lifting — big, full bleed, confident
- Simple 4-col photo grid like Casa Grande's gallery grid-4
- Labels are tiny Montserrat caps with letter-spacing. Not bold section headers everywhere
- Red accent color: **#c0392b**

### What to AVOID (this is what made it look AI/vibe-coded):
- Repeating the same pattern every section (label → divider → big title → cards)
- Icon grids for services
- Ticker/marquee bars
- Too many animations or reveal effects
- All-dark color scheme with gold accents (that was the first attempt — it looked like every AI barbershop site)
- Playfair Display (too fashion/editorial, not right for this shop)
- Generic template structure

## Current site sections (in order)
1. **Navbar** — dark #1a1010 bg, Bebas Neue logo, Montserrat nav links, EN/ES toggle, phone CTA
2. **Hero** — full viewport, photo bg (gallery-03), overlay gradient, Bebas Neue headline "DOMINICAN / ALL STAR"
3. **About** — white bg, centered, Bitter serif, real review quote pulled from Google
4. **Gallery** — dark bg, 4-col photo grid (5 photos row 1 with tall first cell, 3 photos row 2)
5. **Services** — grey bg, 2-col layout (sticky left label/title, right is menu list with dashed dots + prices)
6. **Salon** — dark bg, 2-col (photo left, content right), Glam Dominican Salon info + service tags
7. **Reviews** — white bg, 3 real Google review cards with red top border
8. **Contact** — grey bg, 2-col (hours for both locations side by side + links, map right)
9. **Footer** — dark bg, logo + social links + copyright

## EN/ES bilingual toggle
Every text element has `data-t="key"` attribute. JS object `TR` has `en` and `en` keys with all translations.
`setLang(l)` function swaps all text. Buttons `#btn-en` and `#btn-es` toggle class `on`.

## Known issues to fix / things still needed
- Gallery grid had a blank space (partially fixed — may need more photos to fill properly)
- No logo image in nav yet (have the logo PNG — red/white/blue All Star star design)
- Services prices are estimates — confirm real prices with Adrian
- Salon section uses a barbershop photo as placeholder — ideally get a real salon photo
- Mobile nav needs a hamburger menu (nav-links hidden on mobile currently)
- Could add a full-screen photo slider in the hero like Casa Grande's section-sliders
- Consider adding Instagram embed or feed section
- No favicon set yet (logo PNG exists)

## Tone of copy
- Short. Punchy. No long paragraphs
- Not corporate. Feels like the shop — confident, warm, community
- "Walk in" not "book" or "schedule"
- "Culture" is a key word for this brand
- Bilingual matters — many customers are Spanish-speaking Dominican/Latin community

## The vibe in one sentence
Dominican All Star should feel like walking into the shop — red chairs, Latin music, barbers in uniform, the energy hits you before you even sit down.
