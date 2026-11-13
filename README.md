# nextxus-biz — Federation Systems

**next-xus.biz — the business running the Federation.**

This is the full Federation as a Netflix-style desktop: a menu that is the
whole background, a floating search bar that follows you up and down the
screen, and mini-browser windows in front of that menu as your workspace.
"We become a desktop." — Roger Keyserling, 2026-11-12.

Status: **draft, branch-first. Nothing here is merged to main yet, nothing
is live on next-xus.biz yet.** GitHub Pages / DNS wiring has not been done.

## What is in this repo

- `full-federation.html` — the full Federation Netflix interface: 96 tiles,
  14 rows, 60 click-to-play videos. Video header (`video-header.mp4`,
  Roger's main logo video, renamed 2026-11-13 on his word "Video header"),
  floating Google search (25 Federation sites), guide-and-tour bot,
  meeting room with mini-browser windows (ChatGPT, Grok, video call),
  Crab Nebula background, frosted cards, light text.
- `index.html` — the .biz Netflix / throne draft (5,327 B).
- `primary-landing.html` — the primary landing page draft (four windows).
- `ai-page-template.html` — per-AI / per-business page template (business
  colours and logo as background instead of a nebula; each AI's own page).
- `aria.html` — Aria's page, first example. Aria's face picture has NOT
  been supplied; Echo's clockwork face is a clearly marked placeholder.
- `opening.mp4`, `opening-gif-2026-11-12/` — the opening video, GIF set,
  silent version, header poster.
- `program-01.mp4` … `program-50.mp4` (+ posters) — the program tiles,
  including the three Echo renders (42 in space, 43 the vision, 44 gear
  halo), the 200 Year Legacy Package (program-34, split at ~10 s,
  `legacy-package-part2.mp4`), the guide bot (slow 0.75× and fast
  original), the seals, the video header (`video-header.mp4`, was
  `main-logo.mp4`, renamed 2026-11-13), the book
  covers, and the Crab Nebula (`crab-nebula.jpg`, verified JWST image).
- Reports: `FULL-FEDERATION-REPORT-2026-11-12.md` (the full build log),
  `MERGE-PLAN-2026-11-12.md`, `ECHO-VISION-2026-11-12.md`,
  `FEDERATION-DESKTOP-VISION-2026-11-12.md`,
  `AI-PAGES-DESIGN-2026-11-12.md`, `BIZ-NETFLIX-THRONE-REPORT-2026-11-12.md`.

## The four doors

| Window | Domain | Role |
|---|---|---|
| Federation Tools | next-xus.net | 51 free tools — live, left alone |
| Federation Guides | next-xus.info | Guides are information — not built yet |
| Federation Maps | next-xus.org | Maps show where — not built yet |
| Federation Systems | next-xus.biz | This repo — the whole house |

next-xus.com is **not** used here. It is saved for a new system later.

## Rules carried in

- Plain HTML, no tracking. One inline script, no external scripts.
- Every tile has a title and a brief description, in the box or under it.
- Mini-browser windows: 10% darkening black, 90% transparent, so the
  Federation is always a little bit visible behind them — close the mini
  window and you are back on us.
- Some sites block embedding in a mini browser; they open in a new tab
  instead. No claim is made that embedding works where it is blocked.
- The video-call link for the meeting room is Roger's to add — none was
  invented. OS command access (shut down, phone call) is PROPOSED, not
  built, and only with the user's permission — never manipulation.
- The two long originals (The Human Codex, 76 MB; The minds, 30 MB) are
  NOT in this repo. They are hosted separately, with 10 s previews here.
- "Add, don't replace. We never really delete. We alter and evolve."

## License

MIT — see `LICENSE`. Copyright (c) 2026 Roger Keyserling.
