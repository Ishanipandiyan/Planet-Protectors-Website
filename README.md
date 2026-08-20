# Planet Protectors Enviro — Website

## Project structure

```
planet-protectors-website/
├── index.html          Homepage markup — reflects PPEPL's actual services
├── css/
│   └── styles.css      All styles (design tokens, layout, responsive rules)
├── js/
│   └── main.js         Header scroll state, mobile menu, scroll-reveal
├── images/
│   └── logo.png         Shield emblem (background removed, cropped)
└── README.md
```

## What's on the page now

Rebuilt from `Company_Profile_-_PPEPL_-_R6.docx`. Every section is sourced from that
document — nothing invented:

- **Hero & About** — company overview, incorporation date (May 2025), focus areas
  (bio-mining, pyrolysis, electrical, infrastructure operations).
- **Stat strip** — incorporation date, 20+ years leadership experience, 7+ years
  specialized field experience, 10 service lines. All real figures from the profile.
- **Services (10)** — Bio-Mining & Waste Management, Electrical Projects & Installations,
  BOV Supply & Operation, Incinerator AMC & O&M, Plastic Pyrolysis Plant O&M, RDF &
  Biomass Transportation, Project Management & Cost Control, Manpower & Machinery Supply,
  Civil Projects & Interiors, Site Coordination & Documentation.
- **Operational Strengths (6)** — from the profile's strengths table.
- **Core Values (5)** — Integrity, Sustainability, Innovation, Teamwork, Accountability.
- **Vision & Mission** — quoted directly from the profile.
- **Quality, Safety & Environment Policy (4 points)**.
- **Who We Serve** — Government Departments, Municipal Corporations, Town Panchayats,
  Pollution Control Boards, Environmental Agencies.
- **Footer** — full registered address, phone numbers, and both email addresses.

Photography is loaded from Unsplash's CDN directly in `index.html` (free-to-use,
commercially licensed) — matched to each service (excavator for bio-mining, electrical
panel for electrical works, EV charging for BOV, industrial plant for pyrolysis/
incinerator, etc). No local copies needed; see the "Still to do" note below if you'd
rather self-host them.

## Running it locally

No build step — it's plain HTML/CSS/JS. Either:
- Double-click `index.html` to open it in a browser, or
- Serve it locally: `python3 -m http.server 8000` from this folder, then visit
  `http://localhost:8000`

## Deploying on Zoho Sites

Upload the whole folder (keeping the `css/`, `js/`, `images/` structure intact) to your
Zoho Sites file manager, or paste `index.html`'s contents into a Custom HTML block and
upload `css/styles.css`, `js/main.js`, and `images/logo.png` alongside it, updating the
paths if Zoho flattens the folder structure.

## Still to do

- Swap in real project photography once available (currently licensed stock, chosen to
  match each service).
- Build out dedicated Services, About, and Contact pages if you want more depth than the
  single homepage.
- Confirm/replace CIN, GST, or other registration numbers if you'd like them displayed —
  none were in the source profile, so none are shown.
