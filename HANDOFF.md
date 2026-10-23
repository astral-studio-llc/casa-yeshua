## casa-yeshua.md

# Casa Yeshúa — handoff

**date:** 2026-05-04
**stage:** 4 — flagship build (deployed)
**session:** casa-yeshua (tmux)

## current state

- **site live:** https://casa-yeshua.astralintegration.studio
- **repo:** https://github.com/astral-studio-llc/casa-yeshua (pushed, up to date)
- **basecamp:** project 47122720 created but folders NOT yet populated (8-folder structure still needed)
- **dispatch board:** stage 4, github + site links set

### what was built

full single-page site reframed from "sunday event page" to "living sanctuary with daily rhythm":
- hero with flower of life logo, rain effect, five pillars (movement · music · art · ritual · nourishment)
- about section: sober conscious space, hilltop sanctuary
- full-bleed dinner scene image break (golden illustration from their IG)
- daily morning reset section with vinyasa photo card (8-10am, $350/$250, hosts rotate)
- weekly calendar grid (mon-sun, all events/facilitators/prices from their IG schedule posters)
- atmospheric session image break (ts'unun en la guitarra)
- sunday full experience timeline (ice bath 3pm → ecstatic dance 5pm → dinner 7pm → singing circle 8pm)
- pricing: sunday tiers ($350/$250/$150/$150/$100) + daily morning tier ($350/$250)
- essentials (what to bring / commitments)
- stay with us (dorms, yoga shala, kitchen, conscious travelers)
- location with google maps embed + directions (next to falafel loco, opposite organic market)
- CTA: whatsapp primary, instagram secondary, google maps tertiary
- footer with all contact links

### assets

9 images from instagram saved to `assets/gallery/`:
- dinner-scene.webp / dinner-scene-en.webp (golden dinner illustration — spanish/english)
- morning-vinyasa.webp (earth vinyasa forest meditation)
- atmospheric-session.jpg (ts'unun guitarist in forest)
- poi-sunset.webp (silhouette with poi at ocean sunset)
- weekly-schedule.jpg / weekly-schedule-2.webp (two weekly schedule grids, content reference)
- vocal-yin-yoga.webp (monique renee event poster)
- xul-ha.webp (handpan duo event poster)
- poster.jpeg (original sunday full experience poster — in assets/ root)

screenshots at `~/bucket/casa-yeshua-screens/` (desktop + mobile).

## key decisions

1. **reframed from sunday-only to daily sanctuary** — the IG images revealed a full 7-day program. the site now reflects this, not just the sunday event.
2. **hero says "Casa Yeshúa" not "Sunday Full Experience"** — the brand is the sanctuary, sunday is the anchor event within it.
3. **tagline: "a sanctuary of embodied living"** — pulled from their own branding on every poster.
4. **five pillars: movement · music · art · ritual · nourishment** — from their branding materials.
5. **no domain purchased** — staging only at astralintegration.studio subdomain.
6. **whatsapp confirmed as primary CTA** — +52 273 100 9561, verified from linktree.
7. **instagram handle has a dot** — @casayeshua.mazunte (not @casayeshuamazunte).
8. **location: "next to falafel loco, opposite the organic market"** — from their dinner poster.
9. **used earthy-academy as starting template** then did a full rewrite — only the color tokens and font choices survived.

## contacts

- **whatsapp:** wa.me/522731009561
- **instagram:** @casayeshua.mazunte
- **linktree:** linktr.ee/casayeshua
- **facebook:** facebook.com/Mitotecali/
- **google maps:** maps.app.goo.gl/poa29qrSEPzytVFi7
- **no email found publicly**
- **~~984 142 5227~~** — NOT casa yeshua's number (was from a CI workshop listing for Mitotecali). discard.

## people

- **Yeshúa** — founder/host, teaches morning vinyasa
- **DJ Ur Magic** — ecstatic dance DJ (sundays 5-7pm)
- **Félix** — singing circle guide (sundays 8pm)
- **Ts'unun (en la guitarra)** — atmospheric guitar sessions (wednesdays 7:30pm, $150)
- **Lela** — morning reset host (multiple days)
- **Milena** — morning reset host (multiple days)
- **Kyla** — danza del alma (saturdays 10:30am, $200/$100)
- **Jacob Kishère** — men's circle (mondays, conscious donations)
- **Irene Sposetti** — contact improvisation (tuesdays 11am)
- **Maitreya** — shamanic drum journey ($300)
- **Monique Renee** — vocal yin yoga (collab with SVR)

## what's next

1. **basecamp folders** — project 47122720 needs the 8-folder structure populated + visibility flips + feedback-rounds template. scripts exist at /tmp/bc_*.mjs.
2. **cold reach (stage 5)** — draft outreach message for jordi to send to yeshúa. the site IS the artifact. channel: probably instagram DM or whatsapp.
3. **schedule data could go stale** — the weekly calendar is hardcoded from april schedule posters. needs a way to update (or a note that it's seasonal).
4. **videos not used** — 3 videos from IG downloads not incorporated (2.2M, 24M, 843k mp4s). could add a short ambient video bg to hero if desired.
5. **hostelworld link** — could add a direct booking link for the hostel side. not found in current assets.

## what to avoid

- **don't buy a domain** — jordi hasn't confirmed yet
- **don't send messages to yeshúa** — draft only, jordi sends
- **don't trust the phone number 984 142 5227** — it's from a different listing (Mitotecali CI workshop), NOT casa yeshua
- **weekly schedule changes frequently** — don't treat the calendar grid as permanent truth. it's from specific weeks in march/april 2026
- **basecamp folders default to team-only** — MUST flip visibility after creating. always audit with bc_audit.mjs
- **don't send HTML in basecamp campfire lines** — gets escaped to literal text


---
