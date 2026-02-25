# Studio Anté - Landing Page

> *Decide before you build.*

Marketing landing page for Studio Anté, pre-investment innovation validation for Flemish SMEs.

## Hosting on GitHub Pages

1. Create a new repository named `Studio-Anté` on GitHub under `JolanDijkmansPortfolio`
2. Push this folder to the repository
3. Go to **Settings > Pages**
4. Under *Source*, select **Deploy from a branch**
5. Select **main** branch and **/ (root)** folder
6. Click Save
7. Your site will be live at `https://jolandijkmansportfolio.github.io/Studio-Anté/`

### Custom domain (optional)

1. Add your custom domain in **Settings > Pages > Custom domain**
2. Edit the `CNAME` file in this repo with your domain
3. Configure DNS at your registrar

## File structure

```
/
├── index.html              Main single-page site
├── innovatie-checklist.pdf  Lead magnet PDF (sent to quiz respondents)
├── TALLY_SETUP.md          Step-by-step guide to connect the quiz form
├── README.md               This file
├── CNAME                   Custom domain config (edit if needed)
└── .nojekyll               Tells GitHub to skip Jekyll processing
```

## Setting up the quiz

Follow the instructions in `TALLY_SETUP.md` to:
1. Create a free Tally.so account
2. Build the quiz form
3. Embed it in the website
4. Start collecting responses

## Editing the site

Everything is in a single `index.html` file. Key areas:

### Colors (CSS variables at the top)
```css
:root {
  --c-accent: #C4841D;     /* Gold accent */
  --c-blue: #3A6B9F;       /* Secondary */
  --c-bg-dark: #1A1D23;    /* Dark sections */
}
```

### Content sections (marked with HTML comments)
- Hero, USP strip, Manifesto
- Het Probleem (problem cards)
- Onze Methode (two-phase process)
- Waarom Wij (value cards)
- Wat wij niet zijn (boundary cards)
- Tools (coming soon)
- Voor Wie (audience)
- Innovatie-check (quiz / Tally embed)
- CTA + Footer

### Adding pricing later
Add a new section before the CTA. Follow the pattern of existing sections.

### Activating tools
Remove `tool-coming-badge` elements and add links/details to each tool card.

## Tech stack

- Pure HTML/CSS/JS, no build tools
- Google Fonts: Instrument Serif + DM Sans
- Inline SVG icons (monochrome)
- Intersection Observer for scroll animations
- Fully responsive
