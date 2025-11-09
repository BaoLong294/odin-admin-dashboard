# Odin Admin Dashboard

## Overview

A clean, responsive admin dashboard built with semantic HTML and modern CSS. The UI includes a persistent sidebar, a two-row header, and a main content area with project cards, announcements, and a trending panel. This project was completed as part of The Odin Project Foundations to practice layout systems, responsive thinking, and subtle interaction design without JavaScript.

## Project Objectives

- Structure a full page UI with semantic, accessible HTML.
- Build a two-column app layout using CSS Grid for the page frame.
- Use Flex box and Grid together to compose interior sections.
- Implement responsive constraints so content stays centred on large screens.
- Add tasteful micro-interactions for icons and buttons with CSS transitions.

## Tech Used

- HTML5
- CSS3
  - CSS Grid for page layout
  - Flex box for component alignment
  - Responsive sizing with clamp()
  - Transitions, shadows, transforms
- SVG sprite icons (<symbol> + <use>)

## Completed Features

- App frame
  - Two-column layout: fixed sidebar, fluid content area
  - Sidebar spans full height of the viewport
- Sidebar
  - Three logical groups: title, primary nav, secondary nav
  - Icon + label rows aligned via CSS Grid
- Header
  - Two rows: search + user row, greeting + action buttons row
  - Centred content with max-width constraints, responsive search input using width: clamp(260px, 38vw, 500px)
- Projects grid
  - Auto-fitting card grid with repeat(auto-fit, minmax(300px, 1fr))
  - Card actions anchored bottom-right with absolute positioning
- Announcements
  - Even vertical rhythm using flex column gaps
  - Divider lines with consistent spacing above each rule
- Trending
  - Compact media rows with avatar + text, consistent spacing
- Micro-interactions
  - Header icons fade on hover with opacity transition
  - Header buttons
    - Hover: color shift plus soft shadow
    - Active: tactile press effect with transform: translateY(2px)
    - Smooth transition: 0.15s ease

## Skills Demonstrated

- **Layout architecture**
  - Page-level Grid, component-level Flex box, grid-within-flex for precise alignment
- **Responsive design**
  - Content centring with max-width guards on header rows
  - Fluid controls using clamp() to cap growth on wide screens
- **Component thinking**
  - Side-by-side icon + label rows via small grid templates
  - Reusable spacing tokens with gap
- **Interaction design**
  - Subtle, performant animations with transition, opacity, box-shadow, transform
  - Clear hover and active without JavaScript
- **Accessibility touches**
  - aria-label on search input
  - Semantic headings for sections

## Lessons Learned

- **Grid for the frame, Flex for the internals:** Grid made the 2-column app shell trivial. Flex box kept interior rows aligned and stable across sizes.
- **Constrain growth early:** Using clamp() on the search input and setting a max-width on header rows keeps the composition centred while letting the page breathe on large screens.
- **Micro-interactions matter:** Small transitions on icons and buttons deliver feedback without visual noise. translateY(2px) on active gives a satisfying press feel.
- **SVG sprites are tidy:** A single icons.svg with <symbol> entries plus <use> references keeps markup lean and makes icon sizing and color easy to control with CSS.

## Credits

- **Icons:** https://pictogrammers.com/library/mdi/
- **Avatars:** Local placeholder images stored under ./avatars, used for demonstration only.

## Contact

- GitHub: [@BaoLong294](https://github.com/BaoLong294)
- Email: longbao2904@gmail.com
- LinkedIn: [Long Bảo](https://www.linkedin.com/in/long-b%E1%BA%A3o-a9226a377/)
