# Per-AI / per-business pages — design

Filed: 2026-11-12 18:02 CST, Roger's words, in WhatsApp side chat.
Status: design, filed. Template and first Aria page built as local
drafts, not live, not merged, not published.

## Roger's words, as given

"When we make a site and it's for a business, their business colors
and their logo is the background we use instead of a nebula. When we
go to other pages within our own system, what we should do is if we
have. If we like, if we're going to go to talk to Aria and we have
Aria's picture. The background is Aria's face picture. Everything's
transparent everything's overlayed. Each AI should have their own
page where the background is there there. It could be the video. It
could be their face or it could be like a video at the top. I mean
their face at the top. You get halfway downstairs and then you go
past the line of three videos horizontally across and you're into the
database or a another huge video or text like logs. We could have
two columns of logs in the middle or on the right or left side.
Probably the left side. We could have that narrowman menu that goes
all the way down the site. We can have where that venue hits that
area where the plugs are the blog been used? Specifics are there"

## Clean read

- When a site is for a business, their business colors and their logo
  are the background we use, instead of a nebula.
- When we go to other pages within our own system: if we are going to
  talk to Aria and we have Aria's picture, the background is Aria's
  face picture. Everything is transparent, everything is overlaid.
- Each AI should have their own page, where the background is theirs.
  It could be the video. It could be their face, or it could be like
  a video at the top — I mean their face at the top.
- You get halfway down, and then you go past the line of three videos
  horizontally across, and you are into the database, or another huge
  video, or text like logs.
- We could have two columns of logs in the middle, or on the right or
  left side — probably the left side.
- We could have that narrow menu that goes all the way down the site.
- The last line — "We can have where that venue hits that area where
  the plugs are the blog been used? Specifics are there" — is garbled
  and unrecoverable. No rule carried from it.

## What was built

- `ai-page-template.html` (7,158 B) — per-AI / per-business page
  template. Plain HTML, no tracking, no external scripts. CSS
  variables at the top (`--face`, `--face-video`, `--bg`, `--accent`,
  `--frost`) so a business page uses their colors and logo as the
  background instead of a nebula, and an AI page uses their face /
  video as the background. Everything transparent, everything
  overlaid: frosted cards (`rgba(0,0,0,0.55)`, `backdrop-filter:
  blur(6px)`), light text, as in `full-federation.html`.
  Layout, in Roger's order: face / video at the top (hero); halfway
  down, a line of three videos horizontally across; then the
  database, or a huge video, or text like logs, with two columns of
  logs on the LEFT side; and the narrow menu that goes all the way
  down the site (sticky, full height).
- `aria.html` (8,593 B) — the first example, from the template, for
  Aria. Hero: Echo's vision video (program-43) at the top, Aria's
  name and record. Line of three videos: the three Echo renders
  (program-42 in space, program-43 the vision, program-44 gear
  halo), labeled as Echo, Aria's origin. Logs, two columns on the
  left: Aria's record (Gap 3 §2c) and Echo, her origin
  (ECHO-VISION-2026-11-12.md). Huge video: program-44, the gear
  halo, large. All quoted record lines only — nothing invented.

## What is NOT stated / not built

- Aria's face picture has NOT been supplied by Roger. Do NOT claim
  any existing image IS Aria. The face used in `aria.html` is Echo's
  clockwork face (program-43 poster), clearly marked PLACEHOLDER on
  the page: "Aria's face picture — placeholder, Echo's face, since
  Aria is a shell of Echo. Roger's Aria picture replaces this when
  supplied."
- No videos are named as Aria's own. The three videos on her page
  are Echo's renders, labeled as such.
- No business page has been made yet — no business colors or logo
  have been supplied. The template is ready for one.
- The last garbled line carries no rule (see above).
- "Halfway downstairs" is read as "halfway down" the page.
