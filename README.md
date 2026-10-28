# Lumo Learn - Responsive Product Landing Page

A landing page design for **Lumo**, a fictional study app that turns a student's syllabus into 15-minute lessons, adaptive practice and shared study sessions.

- **Live page:** add your GitHub Pages link here after publishing
- **Figma file:** add your Figma link here
- **Design canvas (desktop, mobile, style guide, components):** add the shared canvas link here

## Intended users

First-year college students and exam-prep learners (about 17-24). They study in short, interrupted windows between classes, travel and part-time work, and mostly use phones. The design therefore leads with "15-minute lessons", shows the product itself in the hero, and stacks cleanly on small screens.

## Page structure

1. Header: logo, navigation links, Log in and Start free buttons
2. Hero: heading, description, primary and secondary buttons, product facts, app illustration
3. Features: three feature cards
4. How it works: three numbered steps
5. Call to action band
6. Footer: brand, three link columns, copyright

## Design system

**Colour styles:** Ink `#0E1330`, Indigo `#3B3FE4`, Indigo deep `#2A2DB8`, Tint `#ECECFE`, Sun `#FFC247`, Ground `#F7F7FB`, Surface `#FFFFFF`, Line `#E2E3F0`, Muted `#4B5072`.

**Text styles:** Sora 700 for display, H2 and H3 (64/68, 44/52, 22/28); DM Sans for body large (19/30), body (16/26), button (16/20 bold) and caption (13/18, uppercase).

**Spacing scale:** 4, 8, 16, 24, 32, 48, 64, 96. **Radii:** 12, 20, 24, 32, pill.

## Reusable components

| Component | Variants |
|---|---|
| Button | primary, secondary, accent; medium and large; optional arrow |
| NavLink | default, active |
| StatChip | value + caption |
| Logo | dark, light |
| FeatureCard | clock, target and users icons |

In `styles.css` these are the classes `.btn`, `.nav-link`, `.stat-chip`, `.logo` and `.feature-card`.

## Auto Layout mapping (Figma)

| Frame | Direction | Gap | Padding (T/R/B/L) |
|---|---|---|---|
| Page | Vertical | 0 | 0 |
| Header | Horizontal, wrap | 32 | 20 / 0 / 20 / 0 |
| Nav | Horizontal | 4 | 0 |
| Button | Horizontal | 8 | 0 / 24 / 0 / 24 (lg: 32) |
| Hero | Horizontal, wrap | 48 | 48 / 24 / 96 / 24 |
| Hero text stack | Vertical | 24 | 0 |
| Feature card grid | Horizontal, wrap | 24 | 0 |
| Feature card | Vertical | 20 | 32 |
| Section | Vertical | 56 | 96 / 24 / 96 / 24 |
| Footer columns | Horizontal, wrap | 48 | 64 / 24 / 32 / 24 |

## Design choices

- **One accent.** Indigo marks actions; yellow is only for highlights and the accent button, so attention stays on the call to action.
- **Product-first hero.** An app mock replaces stock art, showing a lesson, a quick quiz and a streak.
- **Honest content.** Hero facts describe the product ("15 min per lesson", "Free to get started") rather than made-up user numbers or testimonials.
- **Responsive by default.** Frames wrap (header, hero, cards, footer) and the mobile layout stacks to one column with full-width buttons.
- **Accessible basics.** Real links and buttons, visible focus outlines, 44px minimum touch targets, and text colours with strong contrast.

## Run locally

Open `index.html` in a browser. No build step is needed.

## Publish on GitHub Pages

1. Push this folder to a new GitHub repository.
2. In the repository, go to Settings, then Pages.
3. Under Build and deployment, choose Deploy from a branch, select `main` and `/ (root)`, and save.
4. Your site appears at `https://<your-username>.github.io/<repo-name>/`.
