# Vokabeln — Nothing Edition

Spanish → German vocabulary trainer with a 5-compartment Leitner spaced-repetition system, designed in the Nothing Design language (OLED black, Doto dot-matrix hero type, Space Grotesk / Space Mono UI, one red accent per screen).

## Leitner logic

- Correct answer: card advances `F{n} → F{n+1}` (capped at F5 "mastered").
- Wrong answer: card drops to F1.
- Next card is weighted by lowest Fach first, so due cards surface before mastered ones.

## Stack

Static single-file app. React 18 + Babel-standalone + Tailwind via CDN. No build step — Vercel serves `index.html` directly.

Designed mobile-first for iOS (safe-area insets, `100dvh`, PWA meta tags). On desktop the app renders inside an iPhone frame; on phone it fills the viewport.

## Run locally

Open `index.html` in any browser, or serve the directory:

```
python3 -m http.server 3000
```

## Deploy

Pushed to GitHub and deployed via Vercel — no configuration required.
