# Casa Yeshúa — Mazunte

## what this is

Casa Yeshúa is a community space in Mazunte (oaxaca) running a Sunday "Full Experience" gathering, a 6-month rainy-season journey starting now.

**Sunday rhythm:**
- 3:00 — ice bath + workshop (Playtime — vocal + movement games)
- 5:00–7:00 — ecstatic dance (DJ Ur Magic)
- 7:00 — community dinner (vegan / vegetarian)
- 8:00–8:30 — singing circle (guided by Félix)

**Pricing tiers:**
- $350 full experience (best value)
- $250 ice bath + workshop + dance
- $150 ecstatic dance only ($100 locals)
- $150 dinner + singing circle
- $100 singing circle only

**Vibe:** "come as you are. leave more alive." sober conscious space. vegan/vegetarian. respect · presence · connection. dark/gold poster aesthetic, flower of life motif, embers + rain.

**Asset:** the official poster is at `assets/poster.jpeg` — extract copy, vibe, palette, structure from it.

## the goal

build a single-page conversion site that makes someone want to show up Sunday. ticket-tier picker / RSVP, schedule, location, "what to bring", a clear CTA. mobile-first. ships fast.

**don't buy a domain yet** — jordi will pick later. for now just deploy to a subdomain on `astralintegration.studio`. the staging path on hetzner is `~/sites/casa-yeshua/`, served via a caddy block at `casa-yeshua.astralintegration.studio` (add the block per `~/.claude/projects/-Users-astral/memory/reference_namecheap.md` step 5).

## use this template

start from: `~/sites/main/templates/earthy-academy/` (on hetzner — `ssh astral`).

it's the dark earthy template originally used for ShivEnergetics. fits Casa Yeshúa's aesthetic well (gold ink on dark earth, serif display, warm woody palette). pull it down, adapt copy + colors for Casa Yeshúa, keep the editorial luxury structure.

```bash
ssh astral 'cat ~/sites/main/templates/earthy-academy/index.html' > ./index.html
```

## basecamp project — already created

- ID: **47122720** ([Casa Yeshúa] Astral Labs — Client Build)
- URL: https://3.basecamp.com/6078170/projects/47122720
- created PLAIN (template_id endpoint 404'd) — NEEDS the standard folder structure ADDED:
  - 00 Project Overview
  - 01 Discovery
  - 02 Scope & Contract
  - 03 Brand & Assets (drop poster + photos here)
  - 04 Build Documentation (TEAM-ONLY — keep team-only)
  - 05 Feedback
  - 06 Launch & Handoff
  - 07 Phase 2 / Expansion
  - 08 Feedback rounds (with template doc + how-to — use `bc_setup_feedback.mjs` pattern)

**critical visibility gotcha** — every new folder + doc defaults to `visible_to_clients: false`. clients see nothing. immediately flip via `PUT /buckets/{id}/recordings/{rec_id}/client_visibility.json {"visible_to_clients": true}` after creating. only `04 Build Documentation` stays team-only.

audit at the end with `node /tmp/bc_audit.mjs`. fix script: `/tmp/bc_fix_visibility.mjs`.

## github repo

create a repo under `astral-studio-llc` org (free tier). probably named `casa-yeshua`. push the site files there. enable github pages OR keep deployment via hetzner caddy + a simple deploy script. mirror the pattern used for `astral-studio-llc/ema-ozina` and `astral-studio-llc/nube-de-agua`.

## must-read references (memory files)

before doing anything destructive or external, read:
- `~/.claude/projects/-Users-astral/memory/reference_basecamp_workflow.md` — basecamp API, helper scripts at `/tmp/bc_*.mjs`, gotchas
- `~/.claude/projects/-Users-astral/memory/reference_namecheap.md` — domains + cloudflare + caddy. global CF key (cfk_KuQyjEnzUQ...) uses X-Auth-Email/X-Auth-Key headers, NOT Bearer. needed for email routing.
- `~/.claude/projects/-Users-astral/memory/reference_email_forwarding.md` — forwardemail.net is the easy path (DNS-only, no verification); CF native needs the global key + verification click
- `~/.claude/projects/-Users-astral/memory/feedback_per_project_docs.md` — write good per-project docs; port reusable patterns into `reference_<archetype>_skill.md` later

## helper scripts already present

these were built during the mend-a-mano session. reuse, don't rewrite:
- `/tmp/bc_post.mjs` — post message to message board (HTML)
- `/tmp/bc_chatline.mjs` — post line to campfire (PLAIN TEXT only — basecamp escapes HTML in chat lines)
- `/tmp/bc_doc.mjs` — read a doc, download an upload by ID
- `/tmp/bc_setup_feedback.mjs` — create the `08 Feedback rounds` folder + 2 docs
- `/tmp/bc_audit.mjs` — walk every project's vault and print folder+doc visibility
- `/tmp/bc_fix_visibility.mjs` — flip folders client-visible (keeps 04 team-only)
- `/tmp/bc_visibility.mjs` — flip a single recording's visibility
- `/tmp/bc_create_project.mjs` — create a basecamp project (used today; template_id path doesn't work, falls back to plain)
- `/tmp/shoot.mjs` — puppeteer-core full-page screenshots (chrome at /Applications/Google Chrome.app)

## CTA / contact (confirmed 2026-05-01)

**whatsapp (CONFIRMED):** +52 273 100 9561 — wa.me/522731009561 (from their public linktree, jordi-verified)
**instagram (CONFIRMED):** @casayeshua.mazunte (NOTE THE DOT — instagram.com/casayeshua.mazunte/)
**linktree:** linktr.ee/casayeshua
**facebook:** facebook.com/Mitotecali/
**google maps:** https://maps.app.goo.gl/poa29qrSEPzytVFi7?g_st=ac (google place id: 0x85b9290061fca121:0x1d270f8e29336af6)
**no email found publicly.** no website existed before ours.

the poster QR code points to the google maps pin (decoded by jordi).

**site CTA:** primary = whatsapp wa.me link, secondary = instagram, tertiary = google maps "find us"
**~~984 142 5227~~** — this was from a CI workshop listing for Mitotecali, NOT Casa Yeshua's number. discard.

## venue: Mitotecali / Casa Yeshua

- address: Avenida Principal, 70947 Mazunte, Oax.
- also described as: Buganvilias / Calle Principal, across from the organic Sunday market
- google maps: maps.app.goo.gl/poa29qrSEPzytVFi7
- hilltop location, 2 min from downtown, 7 min from beach

## also a hostel

Casa Yeshua is NOT just a Sunday event — it's also a **hostel** listed on Hostelworld:
- dorms + camping
- yoga shala
- shared kitchen, bar, 24h security
- check-in 15:00-22:00
- tagline: "A wellness-focused sanctuary for conscious travelers"
- emphasizes intentional community living over party atmosphere
- better tagline from their linktree: "A living sanctuary for movement, music and ritual, where daily morning practices and communal meals create a retreat-like space for reconnection."

## people

- **Yeshua** — host/founder of Casa Yeshua. also runs a small organic restaurant ("Yeshua") in Mazunte — dinner only, dish of the day. no last name found.
- **DJ Ur Magic** — ecstatic dance DJ (5-7 PM). no online presence found.
- **Felix** — singing circle guide (8-8:30 PM). no online presence found.
- **King Kwa Zulu** — DJ/MC who has performed at the space. based in San Cristobal. email: kingkwazulu@gmail.com, IG: @kingkwazulu. not on the current Sunday poster.

## NOT the same as Ecstatic Sunday

Ecstatic Sunday (@ecstaticsunday) is a separate event at Villa Punto de Equilibrio, Zapotal. Different organizers, venue, timing (12-7 PM), and pricing (250/150 MXN). Casa Yeshua is a distinct event at Mitotecali in Mazunte proper.

## rocket.chat

post all updates to `#prospects` (this is a prospect-tier project). ssh astral '~/bin/rc-post.sh prospects "[CASA-YESHUA] ..."'

## the rhythm we promised clients

every client project gets the `08 Feedback rounds` folder. the rhythm:
1. client duplicates the template doc per round
2. renames it ("Round 2 — colors and shop")
3. fills in + drops attachments inline (voice notes welcome)
4. pings the campfire chat: "round X ready"
5. we apply, ship, reply

mirror this on Casa Yeshúa.

## priorities (in order)

1. read the memory references above
2. populate basecamp project 47122720 with the 8 folders + welcome message + visibility flips + feedback-rounds template + audit
3. pull the earthy-academy template, copy to `~/sites/casa-yeshua/`
4. customize: copy from poster, palette adjustments (keep dark gold), schedule section, pricing tiers, "what to bring" + "sober space" trust markers, RSVP CTA
5. add caddy block for `casa-yeshua.astralintegration.studio` and reload (no domain purchase)
6. create github repo `astral-studio-llc/casa-yeshua`, push
7. screenshot the site (puppeteer), drop in `~/bucket/casa-yeshua-screens/`
8. ping #prospects with the deliverables
9. ASK jordi about: contact channel for RSVP (whatsapp? insta? form?), invite list for basecamp (no client emails on the poster — need them from him before inviting anyone to basecamp)

## DO NOT
- buy a domain yet
- guess contact info
- skip visibility flips after creating folders/docs (clients see nothing)
- send HTML in campfire chat lines (gets escaped to text)
- run `templater.mjs --help` (it's not a real CLI flag, the script auto-creates a project on import)
