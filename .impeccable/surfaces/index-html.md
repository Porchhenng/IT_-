---
version: 1
slug: "index-html"
primary_target: "index.html"
related_targets: []
---

## Scope and visitor mode

Single-file static site `index.html` (no framework, no build step, no package manager). Visitor mode: **Persuade**, deliberately not the portfolio default of Experience — there is no artifact to stand inside, the proof is written explanation, and the visitor arrives to decide.

## Audience, job, action, proof

A reviewer at a Japanese IT company opens the link sent with a full-time job application, alongside the CV. They have never heard of him and may be screening in HR before an engineer sees it. Primary action: reply, or pass it on internally with a yes. Success is a reviewer who can say what he builds and what he is responsible for after about a minute.

Proof is **written content only** — no repos, demos, screenshots, metrics or testimonials exist, and none may be invented (see PRODUCT.md, Evidence on Hand). Credibility comes from specificity.

## Chosen direction: The API Reference

Locked by the user on the surface decision page (seed key `0258526b`, scope surface, mode persuade; dealt 4/3/5, lead index 4 = "The Transaction Spine"; the user chose the **IMPECCABLE'S PICK** card instead). Round resolved **code-led** — no image generation on this machine, so no comp is owed and the ambition lives in the direction contract.

The incumbent visual world is **inherited, not replaced**: cream `#F6F1E7`, ink `#181511`, one blue `#2952E3`, terminal `#171410`, and the existing token and theming architecture all stand. This round decided composition only.

**Structural thesis:** the HTTP motif stops being decoration laid over a conventional portfolio and becomes the page's actual grammar. The site is the reference documentation for the developer. It refuses the arrangement every other application in that inbox uses: hero, project cards, skills grid, contact.

**Composition:** three-pane documentation layout — resource rail (left), request pane (centre), response pane (right). Selecting a resource swaps the panes without a page load.

**First viewport:** the rail with the NBC resource open; the name is a byline in the rail header, not a hero. The reviewer meets the work first, the face second.

**Rail order** (resource-oriented, not section-oriented — each system is its own resource, with employer/role/dates as fields inside it; this also puts the strongest work forward even where the job title was "intern"):

1. **NBC / Bakong** — load testing, Appium; public information only
2. **E-commerce / KHQR** — an ordinary pane, not a depth pane (see Memorable moment)
3. **Biz Solution** — Odoo, PayWay, Redis
4. **CDC** — NestJS scheduling API, Next.js LCD portal
5. Skills, credentials, contact

**How the form answers its own risk:** a non-engineer screening first may not read documentation. Every real API reference opens with an introduction, so `GET /about` answers in plain prose, in the reader's language, who he is and what he is available for. The fix is native to the form rather than bolted on.

**The NBC thinness problem and its resolution:** NBC opens the page but is the pane he can say least about. The way out is that the NBC work targets a **public, documented** API. A load test's substance is the shape of the test itself — virtual users, ramp profile, assertions on response time, pass/fail thresholds — plus the Appium mobile flow. None of that discloses bank internals. **The user must still approve that pane's content.**

**Disciplines carried from challengers that lost the round** (named, not smuggled; the user may strike either):
- From the character sheet: the four-views treatment — one system shown as request path, data model, failure path and monitoring, instead of one prose paragraph.
- From the bolted book: one reserved accent, spent only on the element under load, never scattered.

## Memorable moment

~~The KHQR resource showing a payment moving through its states, with the webhook as the thing that decides it.~~ **Struck by the user, 2026-09-21:** asked whether to build it generically, from real payloads, or not at all, he chose *"Skip KHQR depth for now."* KHQR is an ordinary resource pane.

**Resolved 2026-09-21 by `overdrive`: the memorable moment is "The Live Request."** The user chose it from three directions (the others: a canvas load-test instrument on the NBC pane, rejected as unlabellable against the invented-metrics ban; and pure motion choreography). The page stops imitating an API reference and behaves like an API client.

- Selecting a resource is a request. The response pane shows `200 OK` with a latency, the record streams in field by field under a sweeping scan line, and the `GET`/`POST` verb flies from the rail item into the endpoint header via View Transitions.
- **Every number is measured, never authored.** Latency is `performance.now()` from the click to the frame where the last record field finished painting, so it varies with the machine, the browser and the field count. The opening request uses `t0 = 0` (navigation start), making the first number the real time from opening the link. This is what keeps the moment inside PRODUCT.md's ban on invented metrics; a future edit must not swap in a fixed or random number.
- A **session log** accumulates at the foot of the response pane, so a reviewer who reads every resource ends holding a request log of their own reading. Capped at the last 6 entries; shared across panes; re-labelled on language switch (`Session log` / `セッションログ`).
- Repeat visits resolve instantly and are marked `· cached` (`· キャッシュ`), which is both true to HTTP and the thing that stops the effect becoming tiresome on the eighth click.
- The send button logs `202 Accepted`: the mail client took the message, which is all the page can honestly claim.

Degradation, all verified: no JS renders all eight resources with no lifecycle UI at all (it is JS-built); `prefers-reduced-motion` skips the stream, the morph and the scan but keeps the status and log; below 900px the rail verb is `display:none`, so `morphTo` detects the missing source element and falls back to the existing stagger.

## Boundaries and anti-goals

**Untouched:** colour tokens and theming architecture, the no-flash theme init, the `prefers-reduced-motion` block, CV download, `mailto:` contact, LinkedIn link.

**Anti-goals:** no invented metrics, repos, demos or endpoint specifics; no fabricated employer payloads; no five decorative `200 OK` badges; no claim about visa or relocation until the user settles it; no "researched Bakong, then joined the bank that runs it" narrative (the fellowship is removed — see PRODUCT.md).

## States and ranges

Eight resources (about, NBC, e-commerce/KHQR, Biz Solution, CDC, skills, credentials, contact); four roles; **no projects** (PQC removed by the owner 2026-09-21); 34 skill chips across six groups; four certifications; three languages. States: language (**Japanese by browser detection**, English switch, choice persisted), theme, selected resource, no-JS fallback where every resource renders and the rail degrades to anchor links, reduced motion.

## Interaction and layout

Rail selection drives both panes. On mobile the three panes stack and the rail becomes a top selector — this is what fixes the current side-by-side collapse below 900px. Every control reaches a 44px target. Real headings replace the `<span class="path">` section titles. Motion is one orchestrated transition on resource change, not scattered hover effects.

## Build state at handoff

**The three-pane API Reference structure and the Live Request lifecycle are both built (2026-09-21).** Verified over Chrome DevTools Protocol at 1440×900 and 390×844, light/EN and dark/JA, plus a `prefers-reduced-motion: reduce` pass and a scripting-disabled pass: 0 console errors, 0 runtime exceptions, 0 horizontal overflow at 390px, record rows fully opaque under reduced motion, no lifecycle UI at all without JS. Detector after the pass: 4 findings, all pre-existing inherited fonts (Inter ×1, Space Grotesk ×3); none introduced. Note the detector ran **DEGRADED** (its HTML/CSS parser modules are not installed on this machine), so it fell back to regex and did not evaluate custom properties, selector matching or computed contrast — treat that count as an undercount, not a clean bill of health.

One regression was found and fixed during verification: giving `.res-inner` `position:relative` below 1180px (needed as a containing block for the scan line) re-activated the base rule's `top:78px` sticky offset and pushed the whole response pane down 78px. It now carries `top:auto`. Do not drop that.

**Items 1–9 below are BUILT (2026-09-21) and verified in a headless Chromium pass at 1440×900 and 390×844, light/EN and dark/JA.** PRODUCT.md is written and current. The critique snapshot is at `.impeccable/critique/2026-09-21T03-13-35Z__index-html.md` (19/32, 1×P0, 2×P1) and predates these fixes.

Root cause found during the build, beyond what item 8 named: `body{animation:page-fade-in … both}` ended on `transform:translateY(0)`, so the identity transform persisted and made `body` the containing block — the "fixed" sidebar and `.top-controls` scrolled away **on desktop too** (measured sidebar `y:-1293` at `scrollY 1293`). The entrance animation is now opacity-only; do not reintroduce a transform on `body` or `.wrap`.

Also built alongside item 1: `Appium` and `Load Testing` chips in Skills → Tools & Platforms (PRODUCT.md records both as part of the NBC stack). Mobile now has a fixed top bar for the language/theme controls and a horizontal nav rail replacing `nav{display:none}`.

Measured after the pass, at both widths and both themes: no horizontal overflow; status text 4.74:1 (light) / 7.9:1 (dark); POST badge 4.85 / 6.67; `--on-accent` on accent 6.16 / 6.64; all mono content ≥12px; every control ≥44px on mobile. Detector: 12 findings, all pre-existing (inherited fonts ×3, the deferred bounce easings ×6, layout transitions ×3) — none introduced.

**Built scope — "corrections and ordering", explicitly not the structural redesign:**

1. Add the NBC entry (Backend Engineer · National Bank of Cambodia, **Aug 2026 – Present**) at the top of Experience, EN + JA.
2. Biz Solution junior role: `May 2026 - Present` → **`May 2026 - July 2026`** (confirmed), and switch its bullets to past tense. JA: `2026年5月 - 現在` → `2026年5月 - 2026年7月`.
3. Remove the Angkor Social Innovation Park fellowship card and its `i18n-proj2-*` JA entries.
4. Replace the client name "Easy Eazy" with **"a multi-vendor e-commerce platform"** (no substitute name), EN + JA.
5. Fix the stale graduation line at `index.html:641` and its JA counterpart — he has **graduated**, so `expected 2023–2026` is wrong.
6. Fix the three-way identity hedge (`Backend Developer` / `Junior web developer` / `junior web developer focused on backend`) — he is now a **backend engineer at a central bank**; one accurate line replaces all three, in `i18n-role`, `i18n-whoami`, the lede, `<title>` and the meta description.
7. Remove the "enterprise-grade" buzzword (2 hits, EN; also in the JA lede and JA exp0).
8. **P0 — mobile layout break:** `.wrap` is `display:flex` and the `@media (max-width:900px)` block at `index.html:519-539` never sets `flex-direction:column`, so sidebar and main shrink side by side (measured 133px sidebar, 6330px tall, at 390px). Also: `nav{display:none}` with no replacement, `.top-controls` becomes `position:absolute` and scrolls away, lang buttons 29px tall, social icons 20×24, theme button 39×37.
9. **P1 — contrast:** white on dark-mode accent `#7C96FF` is **2.74:1** and hits `.send-btn`, `.cv-btn:hover`, `.tag:hover`. Add an `--on-accent` token (dark ink ≈ `#0E1330` in dark mode). Green `#1E9E6B` is **3.03:1** as 11px status text on cream and **3.10:1** on the POST badge — darken the light-mode green to ≈ `#147A52` and raise mono text to ≥12px.

Deferred P2s, out of this pass: heading structure (one h1, no h2; sections are spans, card titles are divs), and the decoration/false-affordance cleanup (five infinite animations, bounce easing ×6 at lines 181/259/278/415/440/508, glow and halo, hover states on non-links).

## Unresolved decisions — a builder must not invent these

1. **NBC job title as it appears on his contract.** Recorded as "Backend Engineer" from his own phrasing only.
2. **What the NBC pane may say**, checked against his employer's actual rules. Disclosure is **public information only** (PRODUCT.md carries the binding limit).
3. **KHQR example payloads** for the depth pane — needed before the API Reference restructure can be built; nothing confidential.
4. **Visa, relocation, remote availability, start date.** Unsettled; the layout reserves a place and the page says nothing until he decides.
5. **Japanese proofreading.** The JA text has never been read by a fluent speaker and it is the primary reading path for the primary audience. Highest-risk item on the site.
6. **Street address** at `index.html:654-656` (and the `i18n-address` JA entry) — keep, reduce to city, or drop.
7. **CV filename** `CHHENG_PORCHHENG_CV.pdf` ("Chheng" vs the confirmed "Cheng"), and whether the name inside the PDF matches. The PDF's text was never checked — no extractor on this machine.
8. ~~**Katakana usage.**~~ **Resolved 2026-09-21:** the owner asked for it and チェン・ポーチェン is now the JA byline, title, meta description and footer.
