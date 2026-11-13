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

- **PR #3:** https://github.com/Keywebco/nextxus-biz/pull/3 — "Federation desktop v2: a desktop, not a video library", branch `federation-desktop-v2-2026-11-13` → `main`, commit `3bd02a82…`, open, mergeable: true, not merged. Branch blobs verified identical to local files; v1 `full-federation.html` untouched on the branch (same SHA as main, `1bf8dc72…`).
- PR #2 (v1 header fix, branch `video-header-not-covered-2026-11-13`) is
  **superseded by this v2 direction**. Left open, not merged. Its rule —
  the video at the top does not get covered at all — is built into v2.
- No live URL is claimed until verified live after a merge.

## Exact next step

Roger gives the merge word for the named PR — e.g. "Merge the
next-xus.biz PR #N". Then: merge, verify live on next-xus.biz (desktop
and phone), report back. A live phone check is still owed either way.

## Merge + live verification — 2026-11-13 09:57 CST

- Roger's merge word, 2026-11-13 09:56 CST: "Merge and proceed" — for the named PR #3 just presented to him.
- PR #3 re-checked before merging: open, merged false, mergeable true, mergeable_state clean. Head `federation-desktop-v2-2026-11-13` `3bd02a82…`, base main `54aa53fc…`.
- **Merged with a standard merge commit: `577948b81dd977262f95a0bb35d83f3de5cc5fcf`.** Main ref verified = merge commit. PR #2 left open, not merged.
- `full-federation-v2.html` on main: 80,884 B, blob sha `f33f43e0c906e8c1a4e5acdc553727615c0dcbd2`, byte-identical to the local file (the report's earlier "80,198 B" was stale).
- Live over HTTP (https for next-xus.biz still broken — certificate not issued):
  - `http://next-xus.biz/full-federation-v2.html` — first check 404 (Pages build still running after the merge), after ~60 s **HTTP 200, 80,884 B**, title "The Federation — Desktop — next-xus.biz". Served file hash matches the main blob exactly (md5 `bf6ff35d8b081d4938d5be4e6dd4af16`).
  - Served-file checks: 15 categories, 205 tiles parsed from the page's own data (Programs 50, Tools 51, AI 22, Timeline 15, Information 14, Throne 10, Business 9, Systems 8, Meeting 5, Seals 4, Guides 2, Maps 2, Long 2, Books 2, Roger 9); inline script passes `node --check`; dock present (`id="dock"`, 58 px, fixed bottom); `@media (max-width:640px)` with 112 px tiles; `overflow-x:hidden` on the body; mini windows `min(340px, 94vw)`; row loop via duplicated track + scrollLeft wrap; 65 external URLs, all on record.
  - Live media spot checks: crab-nebula.jpg 200 (342,975 B), opening.mp4 200 (1,866,876 B), ring-of-12-seal.mp4 200 (1,761,657 B), program-01.mp4 200 (2,572,665 B).

### Header files were missing on main — fixed, reported plainly

- The merged v2 page references `video-header.mp4` / `video-header.jpg` — the name Roger chose 2026-11-13 09:29 CST — but that rename lived only in PR #2, which was superseded and never merged. Main still had only `main-logo.mp4` / `main-logo.jpg`, so the v2 header video and poster **404'd live** after the merge.
- Fix: commit `d6bd8679fe1eee0c37bb1f89e900a7d3afb28c25` added ONLY those two files to main, byte-identical to the main-logo files already on main (md5 `bc76fcb6c2d2a6b1ba0c5bd504d62554` / `c0f191c28ac9e3965ea643162d9b38e5`). PR #2 was NOT merged. No other file touched. Reversible by a delete commit. Live re-check after the Pages rebuild: video-header.mp4 **HTTP 200, 5,874,929 B**; video-header.jpg **HTTP 200, 24,328 B**.
- The four "missing media" hits from the local check (`opening.mp4`, `opening-gif-2026-11-12/opening.gif`, `opening-header.png`, `opening-header.gif`) are at repo root, not in the local subfolder — v2 uses root paths, so they resolve live (verified 200 above and via the contents API).

### Still owed — live rendered check

- The checks above are served-file and HTTP checks. **No live browser render was available to this merge task**, so the desktop-viewport and phone-viewport visual check (does it look like a desktop, do the rows loop, do tiles fit on a phone, does the bottom dock show, does the video header stay uncovered) is still owed — it needs the parent agent's live browser task, or Roger opening it on his phone: http://next-xus.biz/full-federation-v2.html
- HTTPS for next-xus.biz is still broken (certificate not issued); the http links above are the way to open it for now.
- v1 bug from the build report still open: v1's `full-federation.html` references `../opening.mp4` etc., which do not resolve from the repo root on GitHub Pages — some v1 tiles are broken live. v1 untouched here; fixing its paths is a separate decision for Roger.

## Fix — double-open bug, 2026-11-13 10:02–10:07 CST live check

- Found by a live desktop browser check: tapping a tile's "Open ↗" button opened the mini browser TWICE — two stacked offset copies of the same mini browser, and two copies of the "Get it / buy it" pop-up.
- Cause: every tile had TWO click handlers. `buildAll` called `makeLoop(rail)` first, whose `ensure()` wired every tile with a click handler; then `buildAll` attached a second, unguarded click handler (and keydown handler) to every tile. One tap called `openTile` twice. Keyboard Enter/Space double-fired the same way. The nested `<button class="open">` inside the `<article role="button">` tile was also invalid HTML, and its `stopPropagation()` branch was a no-op (it ran inside the tile's own listener).
- Fix, in the generator sources (`v2_script.js`, `v2_template.html`), rebuilt with `build_v2.py`:
  - One `wireTile(el)` helper attaches the click + keydown handlers once, guarded by a JS property on the element (`el._wired`), NOT a data attribute — `makeLoop` duplicates rails with `innerHTML`, which destroys old tile elements and their listeners; a data attribute would survive the copy and wrongly mark fresh, unwired tiles as wired. A property dies with the element, so duplicated tiles get wired and existing tiles never twice. This also fixes a latent bug: a resize-triggered duplication used to create tiles the old `dataset.wired` guard skipped, leaving them dead.
  - Both wiring sites (`buildAll` and `makeLoop.ensure()`) now call `wireTile` and nothing else.
  - The "Open ↗" label is now a `<span class="open">`, not a nested button — the tile itself is the button (`role="button"`, `tabindex="0"`). CSS `.tile .open` gained `display:block;text-align:center` so the label looks exactly as before.
  - Maximise fix (small change, done): the buy pop-up used to sit behind a maximised window (window z-index beats the pop-up's 121). On Maximise the pop-up is now pinned to the top-right corner below the header, above the window, and put back beside the window on restore. Bringing a window to the front (pointerdown) raises its buy pop-up with it.
- Verification (branch file, before PR): HTML parses, no errors, divs balanced; script passes `node --check`; exactly one `wireTile` definition; both `.tile` query sites route to it; `openTile(findTile` appears exactly twice, both inside `wireTile`; zero nested `button.open`, zero `dataset.wired`, zero `stopPropagation`; diff against main's blob shows ONLY the fix lines; 15 categories, 205 tiles unchanged; no other tile behaviour changed. Base verified in sync with main before editing (local `git hash-object` = main blob `f33f43e0…`, 80,884 B).
- Still owed: a live browser re-check of the fix after merge (one tap = one mini browser + one buy pop-up, on desktop and phone). No live browser was available to this fix task.
- Bottom dock note (observed in the same live check, NOT changed): the fixed dock covers the bottom edge of content scrolling under it at the very bottom of the screen. The page already has `padding-bottom:78px` on the body against a 58 px dock (20 px clearance at the document end), so this is content passing under the fixed dock while scrolling, which is inherent to a fixed dock. Left as is for Roger's call — no padding change made, since it would not change the scrolling-under behaviour.

## Fix — black screen on phone, looping off, row count + back to beginning, 2026-11-13 10:13–10:14 CST

Roger, on his Android phone: the page does not load — nothing but a black screen. His word, 2026-11-13 10:13 CST: "Looping off. Just put it the number of links. It is at the end. Put [a] button back to the beginning and if they push it [it takes] them to the beginning of the row on the left."

### Black screen — cause (live desktop browser diagnosis, 2026-11-13 10:11–10:14 CST)

The page itself loads fine and is not broken: no overlay, no missing background (crab-nebula.jpg loads immediately). The cause is the video header itself:

- It fills about 62% of the viewport, the video picture is pillar-boxed with solid black bars left and right (max-height clamps the box, the video keeps its aspect), its opening frame is near-black (white "NextXus" over a dark image), and video-header.mp4 loads very slowly — opened directly it showed a black screen with a buffering spinner and no duration, and after about 20 seconds it showed only 0:00 of 0:30.
- On a small portrait phone that tall black slow box fills the first screen, there is no bright placeholder while it loads, and the text below is off-screen until you scroll; the phone may also not autoplay it.
- The page is also very heavy: 1,781 elements, 547 Open buttons (the loop duplication), 39 card images still pending at the bottom.

### Black screen — fixes

- **Bright poster.** The old poster was the frame at 1 second — mean brightness 36.5, median 18, nearly black. The new poster is the frame at 29 seconds: the glowing city with "NextXus", mean brightness 65.0, nearly twice as bright. `video-header.jpg` replaced (24,328 B → 52,920 B, same 848×478). It now shows bright the moment the page opens, while the video loads.
- **Poster behind the video bars.** The video element's background is now the poster itself (`background:#000 url("video-header.jpg") center center / cover`), so the black bars left and right show the bright poster, not solid black.
- **Smaller, faster video.** `video-header.mp4` re-encoded, same content, same resolution (848×478), same duration (30.57 s), same h264 + AAC: 5,874,929 B → 4,009,774 B (32% smaller), moov atom at the front (fast start — it already was, verified: moov at byte 52, before mdat at 11011). Frame check at 15 s: identical mean brightness (55.6 vs 55.6), no visible quality loss.
- **Shorter header on phones.** On screens 640 px and under, the header video is 22vh tall with object-fit:cover, and the hero is compact (smaller padding, 1.3rem heading, .95rem text), so the welcome box and the content below are visible without scrolling.
- **Less page weight.** Removing the loop duplication (below) cuts the page from 547 tile buttons to 205, and the informational line from 30 cards to 15. The built file is 83,037 B.

### Looping off

- `makeLoop` is deleted entirely — no rail duplication, no scroll wrap, no resize re-duplication. Rows scroll normally and stop at the end. The informational line is no longer doubled either (was `cards + cards`, now one set).
- Verified in the built file: zero `makeLoop`, zero `innerHTML += rail.innerHTML`, zero `scrollLeft -= half`, zero `cards + cards`.

### Count at the end + back to the beginning

- Every row now ends with a `.rail-end` card, same size as a tile, gold border: the number of links in that row, plainly (e.g. "50 links"), and a button "← Back to the beginning". Tapping it scrolls that row back to its beginning on the left (`scrollTo({left:0, behavior:'smooth'})`).
- Verified by rendering the row template in node: `<div class="rail-end"><span class="rail-count">2 links</span><button type="button" class="back-btn">← Back to the beginning</button></div>` — count and button present, at the end of the rail, after the last tile.

### Double-open fix included — this branch supersedes PR #4

- The `wireTile` one-tap-one-window fix from PR #4 (branch `federation-desktop-v2-double-open-fix-2026-11-13`, not merged) is included here: exactly one `wireTile` definition, `openTile(findTile` appears exactly twice (both inside `wireTile`), zero nested `button.open`, zero `dataset.wired`, zero `stopPropagation`. PR #4 is left open, not merged; this branch supersedes it.

### Verification (branch file)

- HTML parses, no errors, divs balanced 31/31; inline script passes `node --check`; 125 local media references, none missing (5 regex hits are JS template fragments, not paths); 15 categories, 205 tiles unchanged in content (Programs 50, Tools 51, AI 22, Timeline 15, Information 14, Throne 10, Business 9, Systems 8, Meeting 5, Seals 4, Guides 2, Maps 2, Long 2, Books 2, Roger 9); base verified in sync with main before editing (main blob `f33f43e0…`, 80,884 B).
- Still owed: a live phone render check after merge — I cannot render-check on a phone myself; what was checked instead is listed above (served-file checks, node checks, template render in node, frame-brightness measurements). Roger opening it on his phone is the real check: http://next-xus.biz/full-federation-v2.html
- Note: the new poster (glowing city, 29 s) differs from the v1 tile's alt text, which describes the old 1 s frame (hand touching the cube). v1 on main does not use `video-header.jpg` at all (it uses `main-logo.jpg`), so nothing live changes for v1; the local v1 working copy's alt text is stale only. Left as is.
