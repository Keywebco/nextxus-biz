# Federation desktop v2 — report, 2026-11-13

Roger, 2026-11-13 09:50 CST, after seeing v1 on mobile and calling it useless.
His words, cleaned: v1 was a video library, not a desktop. Rebuild as a desktop.

## What v1 got wrong (Roger's verdict, his words kept plain)

- On mobile it rendered horribly. Square videos were blown up too large — you
  could not even see them. The rectangular ones fit.
- It looked like a video library: a whole bunch of clips he gave us, labeled.
  The clips were supposed to be used for websites and everything else, not to
  be the page itself.
- The windows were not uniform in size. Text was uneven — huge amounts on
  some tiles, little on others.
- None of them had a button to connect to anything.

## What v2 is

`full-federation-v2.html` — a NEW file. v1 `full-federation.html` is untouched.
A desktop, not a video library. Fixed Crab Nebula background, visible through
everything. Everything opens in small movable, stackable, reducible mini
browsers. The bottom of the screen has a dock with icons, including search
and menu.

### Layout, top to bottom (Roger's order)

1. **Video header** — `video-header.mp4`, the logo video he made, renamed
   "Video header". The absolute no-cover rule from PR #2 carries over:
   nothing sits on top of it, not the search, not a window, not a panel.
   Hero text sits below the video. Voice-once ("Hear it once") kept.
2. **Text-box sequence, full width, in order** — first box is welcome and
   sign up; then one box per category, across, each with a basic summary and
   a "Go there" link to its row. Sign-up is a plain form that opens the
   visitor's mail app addressed to roger@next-xus.net — no list is kept on
   the page, nothing is sent without the visitor pressing send. Said so on
   the page.
3. **Informational line** — a horizontal scrollable line, one card per
   category with a basic summary. Clicking a card does NOT pop a mini
   browser: it scrolls to that category's row. Simple text things and forms
   pop out in the app (a plain panel), not in a mini browser.
4. **Actual linkage rows** — one horizontal row per category, small uniform
   tiles. Rows loop back to the beginning (the rail is duplicated and the
   scroll wraps), so there is never any empty space. Some rows are 50–60
   long (Programs: 50; Tools: 51), some 10–15 (AI: 22, Timeline: 15,
   Information: 14, Throne: 10), some 2 (Guides, Maps, Books, Long).
5. **Bottom dock** — fixed at the bottom: Home, Search, Guide, Menu,
   Background, Close all. Search and menu live here, not at the top.

### Removed

- **No side menu.** Roger could not see it on mobile.
- **No wide menu under the header.** Waste of space.

### Tiles — uniform, mobile first

- Every tile the same size: 150 px wide on a wide screen, 112 px on a phone.
  About eight fit across on a wide screen; about three across on a phone.
  (Eight across a phone screen was not possible at a usable size — said
  plainly here, not hidden.)
- Image area fixed height, `object-fit: contain` — square videos are fitted,
  never blown up, never cropped large. Rectangular ones fit the same way.
- Title one line, description two lines, clamped. Every description trimmed
  to 90 characters or less in the build; titles are Roger's own wording,
  kept as made, shown on one line each.
- Every tile has an **Open** button. Tap a tile (or Open) and a mini browser
  pops up with it inside. Video tiles play in the window, with sound on/off.
  Site tiles load the site in an iframe, with an "Open in a new tab" button
  — and a plain note that some sites block embedding, their choice, not a
  bug. Text tiles pop out in the app.

### Mini browsers

- Movable by the gold title bar, stackable, reducible (–), maximise (▢),
  close (×), resize by the bottom-right corner. Default small so about
  eight fit; cascade offset.
- **Lighter:** window background `rgba(8,10,24,0.20)` with a soft shadow,
  so the nebula shows through. Text stays solid white with a shadow, so it
  still reads. (v1 windows were 10% black with a heavier feel; the
  darkening is lighter now and the blur is stronger.)
- Cannot be dragged up over the video header (clamped at the header's
  bottom edge + 8 px); a scroll that brings the header back pushes open
  windows down below it. Maximised windows sit below the header too.

### Attached buy pop-up

Next to every tile's mini browser, a second small pop-up opens: "Get it /
buy it". It shows the website or Gumroad listing to buy — or says plainly
"Free — no purchase" for the free tools, or "No buy link yet — that is
Roger's to add" where no real buy link exists. **No buy link was invented.**

### Categories — pulled from the video that has the map

The opening video's map gives the four doors: Tools, Guides, Maps, Systems.
The rows are those four plus the Federation categories already in v1: seals,
information, AI, meeting room, business, Galactic timeline, programs,
throne/Senate, long programs, books, and a new row, Roger.

### Content — 15 categories, 205 tiles

| Row | Tiles | Notes |
|---|---|---|
| Federation seals | 4 | v1 tiles, as made |
| Federation information | 14 | v1 tiles; the Federation Tools tile now opens the live Tools site |
| Federation AI | 22 | v1 tiles, as made |
| Meeting room | 5 | ChatGPT, Grok (real links, mini browsers); video call — link is Roger's to add; how it works; permission to act — PROPOSED, not built |
| Federation business | 9 | v1 tiles + Real Agency Kit (real link, free) + Offspring Seed $49/$69 (buy link not set up yet). The "1 Token = $5" tile is flagged on its face: video content only, not a verified Federation price |
| Galactic timeline encyclopedia | 15 | v1 tiles, as made |
| Federation programs | 50 | All 50 program videos, each its own application |
| Federation Tools | 51 | The 51 free tools, names + URLs + Roger's source lines, each opening in a mini browser, all free |
| Federation Guides | 2 | "Not built yet" + one empty slot, Roger's choice |
| Federation Maps | 2 | "Not built yet" + one empty slot, Roger's choice |
| Federation Systems | 8 | Real GitHub repos: nextxus-yaml, offspring-seed, roger-sim-api, nextxus-free-tools, nextxus-tools, nextxus-music, nextxus-biz + a Systems-layer text tile |
| The operational throne / Senate | 10 | v1 tiles, as made |
| Long programs | 2 | 10-second previews; hosted separately, said so on the tile |
| Federation books | 2 | Covers only — the book is not for sale yet, said so on the tile |
| Roger | 9 | Academia (link to be supplied), blog (link to be supplied), music player (live), podcast (live RSS), Benable (live), Redbubble (needs repair), inventory for purchase (Gumroad listing to be supplied), healing frequencies (draft, not live), affiliate links (empty slot — none supplied, nothing invented) |

### Marked plainly, not guessed

- Academia link: to be supplied. Blog link: to be supplied.
- Redbubble: needs repair — no fix attempted, link to be supplied after repair.
- Gumroad inventory listing: to be supplied.
- Affiliate links: empty slot — none supplied, nothing invented.
- Video-call link: Roger's to add.
- Guides (.info) and Maps (.org): not built yet.
- Healing page: draft, not live, target website undecided.

### Kept from v1

Voice-once on the video header. The guide/tour as a panel — it says on its
face it is a guide and tour, not a live AI chat. The meeting-room row.
Transparency and frosted cards. The nebula. The background picker (now a
dock button: nebula default, opening video, video-header video, or load
your own photo — it stays in the browser, never uploaded).

### V1 bug found while building v2

v1's `full-federation.html` references `../opening.mp4` and
`../opening-gif-2026-11-12/…`. Those paths work from the local subfolder
but do NOT resolve from the repo root on GitHub Pages, where the page and
the opening files both sit at root. Some v1 tiles' pictures/videos are
broken live for that reason. v2 uses root paths (`opening.mp4`,
`opening-gif-2026-11-12/opening.gif`) so they resolve. v1 itself is
untouched here — fixing v1's paths is a separate decision for Roger.

## Validation

- HTML parses: no errors, no unclosed tags, divs balanced 30/30.
- The one inline script passes `node --check`.
- Local media: 124 references; the only ones not in the biz folder are
  `opening.mp4` and the `opening-gif-2026-11-12/` set, which live at the
  repo root (pushed there in PR #1) and resolve from the page at root.
- No `main-logo` references left; no side menu anywhere in the file.
- All 65 external URLs in the file are on record (51 tool sites, GitHub
  repos, the live Tools site, music player, podcast RSS, Benable, Real
  Agency Kit, ChatGPT, Grok). Nothing invented.
- Descriptions: none over 90 characters. Titles: Roger's own wording, kept
  as made, one line each.
- Mobile CSS checked by rule (no live browser was available to this build):
  body `overflow-x: hidden`; tiles 112 px on phones; dock 58 px with
  78 px bottom padding so nothing hides behind it; mini windows
  `min(340px, 94vw)`; overlays stop above the dock. **A live mobile check
  is still owed before calling v2 done — Roger, or the live browser, needs
  to open it on a phone and scroll it.**

## Files

- `full-federation-v2.html` (80,198 B) — the desktop. New file.
- `build_v2.py` — the generator (data from v1 tiles + assimilation.yaml).
  Kept in the folder, not in the repo.
- `v2_template.html`, `v2_script.js` — the template and the logic the
  generator assembles. Kept in the folder, not in the repo.
- `FEDERATION-DESKTOP-V2-REPORT-2026-11-13.md` — this report.

## PR

- Branch `federation-desktop-v2-2026-11-13` → `main`, PR number in the
  delivery message. **Not merged — merge only on Roger's word for that
  named PR.**
- PR #2 (v1 header fix, branch `video-header-not-covered-2026-11-13`) is
  **superseded by this v2 direction**. Left open, not merged. Its rule —
  the video at the top does not get covered at all — is built into v2.
- No live URL is claimed until verified live after a merge.

## Exact next step

Roger gives the merge word for the named PR — e.g. "Merge the
next-xus.biz PR #N". Then: merge, verify live on next-xus.biz (desktop
and phone), report back. A live phone check is still owed either way.
