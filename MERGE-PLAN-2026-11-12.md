# Merge plan — Federation, new domain — 2026-11-12

Roger's words, 2026-11-12:
- 16:34 CST: "Merge The appropriate repositories etc. Code bases everything with a new domain in mind. Transfer the builds information in all the directories etc. The websites that are made in the domains where they're at, we leave those but on this new domain we will make the Netflix type interface. We're going to make the primary landing page with that video at the top defining everything in the Federation by the four windows that go by etc.com. we will save. I have a reason for that"
- 16:36 CST: ".com will not be used now it will be a new system but we need to do all of this Federation today"

## Decision — .com is OUT, .biz is IN (settled by Roger's 16:36 word)

- **Primary landing domain: next-xus.biz** — registered 2026-11-12 22:21:25 UTC at Network Solutions, LLC, expires 2027-11-12, nameservers ns49/ns50.worldnic.com, status client + server transfer prohibited, add period. Verified live via RDAP, 2026-11-12.
- **next-xus.com: NOT used now. Saved. It will be a new system later.** Held still at PDR Ltd. d/b/a PublicDomainRegistry.com, registered 2026-06-26, expires 2027-06-26, status client transfer prohibited. Verified live via RDAP, 2026-11-12. Do NOT point anything at .com, do NOT transfer it, do NOT build on it now.
- The earlier ambiguity is therefore resolved: reading (a) was correct — primary landing on .biz, four windows go to .net / .info / .org / .biz, .com saved for later. Reading (b) — primary landing on .com — is rejected by Roger's 16:36 word. The phrase "four windows that go by etc.com" is read as "etc., .com" — the saved .com, not the landing domain. If Roger meant otherwise, his word overrides this plan.
- **Urgency:** Roger said do all of this Federation TODAY, 2026-11-12. That is urgency, not a merge word. This plan is still a plan: **nothing has been merged, published, deleted, transferred, or spent.** The exact next step he needs to say yes to is at the bottom.

## The four windows (primary landing)

| Window | Domain | Role |
|---|---|---|
| Federation Tools | next-xus.net | 51 free tools — live site, LEAVE ALONE |
| Federation Guides | next-xus.info | Guides are information — site not built yet |
| Federation Maps | next-xus.org | Maps show where — site not built yet |
| Federation Systems | next-xus.biz | The whole house; the business running the Federation — NEW, primary landing |

## Primary landing page — draft built

- [primary-landing.html](sandbox://workspace/free-tools-assimilation-2026-11-12/biz-netflix-throne-2026-11-12/primary-landing.html) — 7,033 bytes, plain HTML/CSS, large, simple, high-legibility, no tracking.
- Video at the top: opening.mp4 (1280×720, 10 s, with sound, 1.8 MB), autoplay muted loop playsinline, poster opening-header.png, fallback opening.gif. It defines everything in the Federation by the four windows that go by: Systems, Tools, Guides, Maps.
- Voice once, then silent: one script only, "Hear it once" button. Browsers block autoplay with sound, so the video starts muted; tap unmutes, restarts from 0, plays once with sound; on ended it mutes again, loops, button becomes "Heard once — now silent". Never tapped, it stays muted and loops silently.
- Rows, Netflix style: the four windows; the operational throne / Senate (Roger Sim Legacy on the throne, Aria, Pontus as regent, Senate 12 seats); the business running the Federation (YAML database, individual AI files, communication, exterior communications, mini browser interaction, extended memory, research, recycling centers workspaces). 16 cards total.
- Validated: HTML parses, 1 video, 1 script (voice-once only), 16 cards, "Hear it once" present.
- Companion draft: [index.html](sandbox://workspace/free-tools-assimilation-2026-11-12/biz-netflix-throne-2026-11-12/index.html) — 5,327 bytes, Netflix rows for next-xus.biz, silent video background.

## Survey — the 12 named repos (read-only, GitHub API, 2026-11-12)

Method: `/opt/hatch/bin/github status` = connected; `search_repositories user:Keywebco` = **98 repos total**; root contents fetched for all 12 named repos. Nothing written, merged, or deleted. Sizes below are root-file bytes only; subdirectories were not recursed. Live-site status was not fetch-verified except where noted.

| Repo | Live / visibility / default branch | What it holds (root) | Serves a live site? | Call |
|---|---|---|---|---|
| Keywebco/nextxus-free-tools | Yes, public, `main`, created 2026-11-12 | 8 root entries, 230,971 B: index.html 22,289; assimilation.yaml 36,919 (51 tools); ASSIMILATION.md 161,424; MIT LICENSE 1,073; MAINTENANCE-AUTOMATION.md; README; .github/ + scripts/ | Pages-capable (index.html); not fetch-verified live | **TRANSFER build info** — static HTML + YAML library, portable as-is |
| Keywebco/offspring-seed | Yes, public, default branch **`stage-0/nova-contract`** (not `main`), created 2026-11-11 | Default branch root: only nova/ → CONTRACT.md 4,934 B. `main` root: .github/, MIT LICENSE, README 646 B, gaps/, lineage/, nova/, ring6/ (merged scaffold) | No — seed/scaffold, no index.html | **TRANSFER** — seed template the five Meta repos copy; say which branch is canonical (`main` holds the fuller scaffold) |
| Keywebco/nextxus-yaml | Yes, public, `main`, created 2026-10-01, updated 2026-11-09 | index.html 18,154; README 1,487; MIND-LAYER-INDEX.md; accumulation/ + source/ dirs. Federation data schemas / YAML DB | Pages-capable; not fetch-verified live | **TRANSFER** — the YAML database is the brain; it must move with the domain |
| Keywebco/nextxus-tools | Yes, public, `main`, created 2026-10-01, updated 2026-11-10 | 17 root entries, 590,231 B: index.html 42,507 + 9 tool pages (calculator, code-beautifier, color-picker, image-resize, randomizer, text-tools, unit-converter, deepai-gallery, Real Agency Kit page + manual); 2 mascot JPGs (~369 KB); CROSS-LINK-CHECKLIST.md | **YES — evidenced live:** real-agency-kit-manual.html live on next-xus.net (crawled 1 day ago); repo desc "Plain HTML on GitHub Pages" | **TRANSFER build info, LEAVE the live site alone** — static tools, portable; Real Agency Kit is the $0 Votel rebuild. The live site on next-xus.net stays where it is; only its build information is copied to the new domain |
| Keywebco/nextxus-music | Yes, public, `main`, created 2026-10-01, updated 2026-11-10 | 7 root entries, 53,565 B: index.html 23,742; player.html; playlist.json 11,272; feed.xml + podcast.xml; episodes/ dir. 86 songs (2026-11-06) | Pages-capable + RSS feeds; not fetch-verified live | **TRANSFER, carefully** — static player + feeds are the distribution point (GitHub-origin doctrine); keep feed URLs redirecting |
| Keywebco/roger-sim-api | Yes, public, `main`, JS, created 2026-09-30, updated 2026-11-09 | server.js 42,390; package.json; render.yaml; smoke.js 7,057; README; sim-intellect/ dir | Not a static site — backend API on Render (render.yaml); live /health verified 2026-11-09, not re-verified today | **LEAVE ALONE** — do not move as part of a static domain move; a domain change would only re-point DNS/proxy to Render, needs redeploy + Roger's word |
| Keywebco/nextxus-post | Yes, public, `main`, Python, created 2026-11-10, updated 2026-11-11 | README 3,892; REPORT.md 2,899; .github/, data/, drafts/, scripts/ dirs. Facebook posting system, test post live 2026-11-11, daily posting off | No — automation scripts, not a site | **LEAVE ALONE** — tied to Facebook Page token, not to a domain; moving it achieves nothing |
| Keywebco/offspring-seed-deepmeta | Yes, public, `main`, created 2026-11-12 02:29 UTC | LICENSE MIT 1,073; README 492 B; nova/ + ring6/ (tree SHAs identical to offspring-seed and all four siblings) | No — seed scaffold, no index.html | **TRANSFER as a set** — DM (DeepSeek) seed |
| Keywebco/offspring-seed-xaimeta | Yes, public, `main`, created 2026-11-12 02:30 UTC | Same shape: LICENSE 1,073; README 492 B; identical nova/ + ring6/ trees | No | **TRANSFER as a set** — XM (xAI/Grok) seed |
| Keywebco/offspring-seed-chatmeta | Yes, public, `main`, created 2026-11-12 02:30 UTC | Same shape: LICENSE 1,073; README 491 B; identical nova/ + ring6/ trees | No | **TRANSFER as a set** — CM (ChatGPT) seed |
| Keywebco/offspring-seed-mimometa | Yes, public, `main`, created 2026-11-12 02:31 UTC | Same shape: LICENSE 1,073; README 488 B; identical nova/ + ring6/ trees | No | **TRANSFER as a set** — MM (MiMo) seed |
| Keywebco/offspring-seed-star | Yes, public, `main`, created 2026-11-12 02:31 UTC | Same shape: LICENSE 1,073; README 559 B; identical nova/ + ring6/ trees | No | **TRANSFER as a set** — STAR (SenateThrone Archive) seed |

### Flags from the survey
1. **offspring-seed changed visibility:** the 2026-11-11 report says Private; the API on 2026-11-12 says public (`private: false`). Presumably made public with the five seed repos — worth confirming it was intended.
2. **offspring-seed default branch is `stage-0/nova-contract`, not `main`** — the only one of the 12 like this. `main` holds the fuller scaffold. Any transfer must say which branch is canonical.
3. **The five Meta seed repos are effectively identical** — same nova/ and ring6/ tree SHAs, same MIT LICENSE blob, READMEs differing by only a few bytes. Transferring one transfers the pattern; they stand or fall as a set.
4. **Pointer PRs still open** (per completion report, not re-checked): nextxus-yaml PR #6 and offspring-seed PR #8 — merge only on Roger's word.

### Other Federation-related Keywebco repos found (86 others; names/descriptions only, contents NOT inspected)
Portal/hub: keywebco.github.io (Federation Portal), roger-keyserling (Identity & Link Hub), nextxus-federation-hub, nextxus-humancodex, nextxus-free-satellites (7 public HTML outposts). Governance/mind: nextxus-senate, nextxus-brain (combined YAML mind, updated 2026-11-12), nextxus-sim, nextxus-sim-api, nextxus-sim-telegram, ring-of-12, ring-of-12-api, ring-of-three, sovereign-knowledge-os, sovereigntools, nextxus-dispatch, nextxus-process, nextxus-blog, nextxus-archives, nextxus-chat, nextxus-recycler, nextxus-build-nova, nextxus-build-sim, nextxus-build-website, nextxus-research-hub, federation-gods-eye, federation-gatekeeper, federation-browser-base, federation-meeting-room-inner, federation-meeting-room-outer, federation-app-vault, federation-mind-mirror, federation-n8n, plexus-relay, echo-64, nextxus-agent-zero, nextxus-ai-minds-lab, nextxus-ai-course-hub, nextxus-truth-gate-core, nextxus-lasting-edition, NextXus-Sovereign-Mirror, nextxus-emmy-board, aria-sanctuary-static, onekey, NextGames. Sovereign pillars/backups: nextxus-help-sovereign, nextxus-online-sovereign, nextxus-org-sovereign, nextxus-studio-sovereign, nextxus-tech-sovereign, nextxus-space-sovereign, nextxus-staging, nextxus-unified-storefront, next-xus-com-sovereign. Private (names only, not inspected): roger-sim-brain, roger-sim-memory, catalyst-consciousness-core, private-council-sovereign-seeds, private-roger-ai-sovereign-seed, private-aria-sovereign-seed, ring-of-six-middleware, ring-of-12-middleware, federation-private-vault, Private-Pontus, Private-Aria, Private-Store, Private-core, Private-Production, Private-Library, Private-Oracle, Private-Rex-Radio, Private-Agent-Zero, Private-Roger-AI, Private-Ring-of-12, Private-Orbot, Private-University, Private-Nova-Scavenger-Alpha, Pillar-Guardian-Sanctuary, Pillar-Guardian-Throne, Pillar-Guardian-Archive, NextXus-Knowledge-Base, Private-Resonance-Research, Nova-Satellite-Template, private-throne-builder-catalyst, nextxus-evolution-protocols-grok. Full 98-repo list is in /tmp/keywebco_list.txt (ephemeral scratch, not a deliverable).

## What "merge" means here — and what it does NOT mean

- **Merge = copy the build information into the new domain's repo, branch-first, PR, merge on Roger's word.** The new domain's repo does not exist yet (no repo for next-xus.biz has been created). The proposed new repo is Keywebco/nextxus-biz (name to be confirmed by Roger — it has not been created, and creating a repo needs the live browser as Keywebco).
- **Websites made in the domains where they are, we leave those.** next-xus.net (Tools, live), nextxus-music player/feeds, roger-sim-api on Render, nextxus-post automation — none of these move, none are deleted, none are re-pointed. Only their build information is copied, so the new domain can link to them and, where portable, host a copy.
- **Nothing is deleted, ever, in this plan.** "Add, don't replace. We never really delete. We alter and evolve." Duplicates: keep the superior/newest in the main DB, archive the inferior outside it, Roger decides archives.
- **No domain transfer, no DNS change, no spending** in this plan. .biz DNS / GitHub Pages wiring has not been done and needs Roger's word plus the live browser (Network Solutions nameservers ns49/ns50.worldnic.com are still in place).

## What build information transfers (directories / files)

To the new next-xus.biz repo, as a copy, not a move:
- From nextxus-free-tools: `index.html`, `assimilation.yaml` (51 tools), `ASSIMILATION.md`, `MAINTENANCE-AUTOMATION.md`, `scripts/check-links.py`, `.github/workflows/assimilation-check.yml`.
- From nextxus-yaml: the YAML database — `index.html`, `MIND-LAYER-INDEX.md`, `accumulation/`, `source/` — the brain, copied as reference; the canonical YAML stays in nextxus-yaml.
- From offspring-seed + the five Meta repos: `nova/CONTRACT.md`, `ring6/CHECKLIST.md`, `ring6/STATIONS.md`, `gaps/GAP-3.md`, `gaps/GAP-4.md`, `gaps/GAP-6.md`, `gaps/GAP-8.md`, `lineage/LINEAGE.md`, `.github/workflows/ring6.yml`, `.github/ISSUE_TEMPLATE/` — the seed scaffold, as a set.
- From nextxus-tools: the 9 tool pages + `index.html` (build information only; live site stays on .net).
- From nextxus-music: `player.html`, `playlist.json`, `podcast.xml`, `feed.xml` (build information only; live feeds stay where they are, with redirects if a path ever changes).
- New, for .biz: `primary-landing.html` (this plan's draft), `index.html` (Netflix rows draft), `opening.mp4`, `opening.gif`, `opening-silent.mp4`, `opening-header.png`, and this report.
- **NOT transferred:** roger-sim-api (`server.js`, Render — leave alone), nextxus-post (Facebook token — leave alone), any private repo (roger-sim-brain, private-* — names only, never inspected, never copied).

## What is still NOT built (today, 2026-11-12)

- Live Guides site on next-xus.info; live Maps site on next-xus.org; live Systems site on next-xus.biz; a repo for next-xus.biz; DNS / GitHub Pages wiring for .biz; the mini browser interaction program itself (only a draft background video exists); the recycling centers as live workspaces. The four windows on the landing page link to Tools (live) and to Systems (this site, draft); Guides and Maps are honestly marked "Site not built yet" on the page.

## Exact next step — the yes Roger needs to say

Roger, say this, in your words, for the named repo and the named PR:

> "Merge the next-xus.biz primary landing PR" — or name the repo you want instead.

Then, in order, today:
1. Create the new repo for next-xus.biz in the live browser as Keywebco (proposed name Keywebco/nextxus-biz — confirm the name first; repo creation cannot be done by the connector, 403).
2. Push, branch-first: `primary-landing.html` + `index.html` + opening video/GIF/poster + this report + the transferred build information listed above, as a PR.
3. Roger gives the merge word for that named PR. Merge, verify live on next-xus.biz, report back.
4. Only then, DNS / GitHub Pages wiring for .biz, on Roger's word, in the live browser.

No live URL is claimed until the push is verified live. No .com use, no transfer, no deletion, no spending, without Roger's word.
