# BCM Laundry Quiz Website Roadmap

## Overview
This repository contains a lightweight single-page laundry habits quiz designed for static hosting on GitHub Pages. The project stays intentionally simple: plain HTML, CSS and JavaScript, short completion time, and lightweight client-side behaviour.

## Project goals
- Keep the site easy to deploy and maintain on GitHub Pages.
- Help a user complete a short laundry habits quiz in under a minute.
- Return simple, practical laundry guidance based on the score.
- Keep the implementation readable enough for straightforward iteration.

## Current website features
- Single-page quiz experience
- Seven laundry habit questions
- Three result categories with tailored guidance
- Randomised question order on page load
- Randomised answer order within each question
- Client-side page view counter using `localStorage`
- Responsive layout suitable for desktop and mobile

## Key implementation decisions
### Static-first approach
The site uses plain HTML, CSS and JavaScript so it can be hosted directly on GitHub Pages without a build step.

### Short quiz format
The quiz is intentionally short to reduce friction and improve completion rate for a proof of concept.

### Score-based advice
Advice is grouped into simple result bands to keep the logic transparent and easy to edit.

### Client-side page counter
The current counter uses `localStorage`, which keeps the implementation simple for a static site. It is a per-device demo counter rather than a shared global counter.

## Open items / not yet built
### Higher-priority backlog
- Persistent global page counter
- Shareable results
- More personalised advice based on specific answer combinations
- Additional accessibility improvements
- Simple analytics for completion and answer patterns

### Lower-priority ideas
- Light branding or illustrations
- Optional README screenshots / deployment notes
- Theme toggle
- Simple animation on result reveal

## Change log

### 2026-06-21 — Initial proof of concept
- Created the first single-page quiz implementation.
- Added seven multiple-choice laundry questions.
- Added three score bands:
  - Laundry Chaos Goblin
  - Spin Cycle Survivor
  - Laundry Legend
- Added a client-side page view counter using `localStorage`.
- Structured the project for straightforward GitHub Pages deployment.

### 2026-06-22 — Quiz fairness and documentation update
- Updated the quiz to randomise question order on render.
- Updated the quiz to randomise answer order within each question.
- Kept scoring tied to answer values so randomisation does not change result logic.
- Removed the manual reshuffle button to keep the interaction simpler.
- Reworked this document into a changelog-style roadmap with dated entries.
- Removed the earlier “definition of done” and “suggested next step” sections.

## Suggested repo structure
```text
/
├─ index.html
├─ ROADMAP.md
└─ (optional later) assets/
```
