# Lab 5 — CSS Foundations: Super Ai Dash Login

## Overview
This lab practices HTML and CSS by trying to replicate the replication.png picture. 
Using progressive enhancement I started with all the HTML and worked my way to CSS.

## Live Site
**GitHub Pages:** https://<your-username>.github.io/lab5-css-foundations/  
_(Replace `<your-username>` with your GitHub handle.)_

## Project Goals
- Two-column layout (brand panel left, form panel right) using **CSS Grid**.
- Semantic form with labels/inputs/buttons; keep **custom elements** `<form-field>` and `<password-recovery>`.
- **Flexbox** to center content within each panel and align the actions row.
- **CSS custom properties** for radius, colors, shadows, spacing.
- **Responsive units** and **fluid typography** with `clamp()`.
- Hover, active, and accessible focus styles.
- Clean, valid HTML (W3C).
- Publish to **GitHub Pages** from `/docs`.

## Issues & Nuances
1) **Brand text too small on large monitors**  
   • Cause: restrictive font sizing   
   • Fix:`clamp()` font sizes so text scales and “fills out” on big screens.

3) **Button & “Forgot password?” alignment**  
   • Fix: Made them combined in one custom tag,so I could align them on the same grid

5) **Selector typo blocked label styles**  
   • Fix: corrected `form field label` → `form-field label`.

6) **Text block centered but left-aligned**  
   • Fix: centered the block with `align-items: center` on `#login-info`, gave `h1` and `p` 

## Design Decisions
- **No `<div>`s:** following prof's preference 
- **Grid ratio:** `4.5fr / 6fr` so the form side has a bit more space.
- **Fluid type:**
    - Heading: `clamp(2.25rem, 6vw, 4rem)`
    - Paragraph: `clamp(1.05rem, 1.25vw, 1.25rem)`
- **Spacing:** responsive page padding `clamp(1rem, 3vw, 2rem)`; internal spacing with `gap`.
- **Polish:** gradient brand panel, rounded corners (`--radius`), subtle shadows, lighter input borders, clear hover/active states.
- **Accessibility:** labels tied to inputs, visible focus rings, `autocomplete` enabled.

## Author
Roy Haynes

## License
MIT

