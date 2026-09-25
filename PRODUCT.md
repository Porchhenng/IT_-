# Product

<!-- impeccable:product-schema 1 -->

## Platform

web

## Users

**Primary (confirmed):** reviewers at Japanese IT companies, reading the site as part of a **full-time job application**. The owner said the site is "meant to be sent to Japanese IT companies for reviews," so visitors arrive because they were sent the link and are evaluating Cheng as a candidate. They are not browsing to discover him. Whether they read the Japanese or the English version is not confirmed.

**Secondary (confirmed):** international and remote employers hiring backend or API developers.

Cambodian employers and recruiter-first screening were offered as audiences and not selected.

Job to be done: judge from the page alone whether this junior backend developer's experience and skills fit, and decide whether to move forward.

## Product Purpose

A personal portfolio site for Cheng Porchheng, a junior backend developer in Phnom Penh. It exists to get him reviewed and considered by Japanese IT companies and other international employers. Success is a reviewer coming away with an accurate picture of what he has built, what he knows, and how to reach him.

## Positioning

A Cambodia-based backend developer working **inside the country's national payment infrastructure**: currently a backend engineer at the **National Bank of Cambodia (NBC)**, Cambodia's central bank, and previously the builder of KHQR/ABA payment-gateway flows for a Khmer-language multi-vendor e-commerce platform.

Central-bank payment-infrastructure experience at this career stage is the part an overseas junior developer's portfolio could not truthfully copy. *The KHQR specifics are drawn from the site's own content; the NBC role was confirmed directly by the owner.*

## Operating Context

- The page is sent directly to reviewers, who read it alongside the CV (`CHHENG_PORCHHENG_CV.pdf`).
- Reviewers are overseas. Cambodian context (KHQR, Bakong, ABA, PayWay, CDC, CADT) cannot be assumed known to them.
- **Current employment (confirmed by the owner, missing from the site entirely): Backend Engineer, National Bank of Cambodia (NBC), since August 2026.** The work is test and performance engineering against Bakong, Cambodia's national payment system: building **load-testing applications for the Bakong public API**, and **Appium-based automated testing for the Bakong mobile application**. The Biz Solution role has **ended**; the site's "May 2026 – Present" for it is now wrong.
- Owner has **graduated** from CADT. **Degree title as awarded, confirmed by the owner 2026-09-21: "Bachelor of Computer Science", with Software Engineering named on the diploma as the major.** Write it out in full. Never abbreviate to **"BSc"**: that expands to *Bachelor of Science*, a different award from a *Bachelor of Computer Science*, and the site and CV both carried that error until 2026-09-21. The correct abbreviation would be BCompSc, rejected as too obscure for the audience. The owner asked for BSc, was shown the mismatch against his school's own degree description, and chose the full form. Do not reintroduce "BSc". The site's "expected 2023–2026" wording at `index.html:641`, and its Japanese counterpart in the `ja` translation table, are now stale and must be corrected to reflect completion.
- **The Japanese text has never been reviewed by a fluent speaker.** The owner lists his own Japanese as intermediate (raised from beginner 2026-09-21), which is not a level at which to self-certify copy sent to native readers who are judging him professionally. The JA translation table in `index.html` is therefore unverified copy being sent to native readers who are judging him professionally. Treat it as a known risk, not as finished content.

## Capabilities and Constraints

- Static single-file site: `index.html`, no framework, no build step, no package manager.
- Existing functions to preserve: EN/JA language switch, light/dark theme, CV download, `mailto:` contact, LinkedIn link. Khmer is not offered.
- Owner's stated language levels on the site: Khmer native, English advanced, **Japanese intermediate (raised from beginner by the owner, 2026-09-21)**.
- **Japanese IT Pathway Program, 2025–2027, ongoing (confirmed by the owner 2026-09-21).** A joint venture between the **American University of Phnom Penh (AUPP)** and **NEXTMAKE Inc.** Recorded under Education, not certifications, and it is the credential that speaks most directly to the primary audience. The owner first named MPTC as a partner and then corrected it to NEXTMAKE Inc.; whether MPTC is also involved was never resolved, so the site and CV name only AUPP and NEXTMAKE.
- Owner's core stack, from the site: NestJS, Vendure, FastAPI, GraphQL/REST, Redis, PostgreSQL, Docker; FCM and AWS CloudWatch; KHQR/ABA and PayWay integrations. Add from the NBC role: **load testing and Appium mobile test automation**.

**Client anonymization (confirmed by the owner).** The client product name **"Easy Eazy" is removed from the site** and replaced with the generic description **"a multi-vendor e-commerce platform"** (EN) / the equivalent in the JA copy. It appears at `index.html` in the `exp1` bullet and in the `ja` translation table. The technical substance of that work — KHQR/ABA payment integration, Vendure, Redis, FCM, AWS CloudWatch — is what carries the credential; the client's brand name adds nothing a reviewer needs. Do not reintroduce it, and do not replace it with an invented product name: the phrase is the description itself, with no name at all.

**Nothing else is masked (confirmed by the owner).** ABA Bank, KHQR, PayWay, Odoo, Vendure, Biz Solution Co., Ltd., the Council for the Development of Cambodia, and the National Bank of Cambodia all stay named. They are the verifiable technical and employment record, and with no repositories, demos or metrics on the page, that specificity is the only thing carrying credibility. Do not generalize them in a later pass.

**Binding disclosure limit (confirmed by the owner).** The NBC work may be described using **public information only**: the employer's name, the role, and the kind of engineering, in general terms. No internal system names, no payload shapes, no architecture detail, no internal metrics. The Bakong *public* API is publicly documented, so describing load testing against it is acceptable; anything internal to the bank is not. When in doubt, say less. A central bank's confidentiality expectations are real, and a disclosure mistake here costs more than a weak portfolio does.

**Content removal (confirmed by the owner).** The **Angkor Social Innovation Park research fellowship is removed from the site** (currently `index.html`, the second card under Projects, with its `ja` translations and the Research / Blockchain / FinTech tags). The earlier instruction to keep it separate from the NBC/Bakong work is superseded: it is not separated, it is gone. Do not reintroduce it, and do not build any "researched Bakong, then joined the bank that runs it" narrative from it.

**Project removal (confirmed by the owner, 2026-09-21).** The **post-quantum cryptography messenger is removed from the site** as well: "remove pqc just keep all work experience." Do not reintroduce it, and do not add any other personal project without asking.

Consequence: **the site has no Projects section at all.** It carries four employment entries (NBC, Biz Solution junior, Biz Solution intern, CDC), skills, credentials and contact — employment only. The page therefore has no research, writing, or personal-project credential, and the ML-KEM / FIPS 203 work no longer appears anywhere. This is the owner's explicit choice, not an oversight.

**Open decisions (not answered; do not assume):**
- **Biz Solution end date.** NBC started **August 2026** (confirmed). The Biz Solution end date is still unstated; if the roles ran back to back it is July 2026, but that is an inference and a job application must state it exactly.
- **NBC job title wording.** Recorded as "Backend Engineer" from the owner's own phrasing; the official title on his contract was not confirmed.
- **CV spelling.** The CV file is named `CHHENG_PORCHHENG_CV.pdf` ("Chheng"), which disagrees with the confirmed name below. The CV's own text was not checked (no PDF text extractor available in that session).
- **Status for Japan-based or Japan-facing roles.** Relocation, visa or work authorization, remote/timezone availability and target start date are unstated. The site says only "open to backend & API development opportunities." The owner is applying full time to Japanese companies, so these are the questions a reviewer there will ask first.
- **Public street address.** The site prints a full street address; whether that stays is undecided.

## Brand Commitments

- **Name (confirmed by the owner):** Cheng Porchheng in Latin script. In Japanese: チェン・ポーチェン. **As of 2026-09-21 the katakana is in use** — the owner asked for it directly ("use my japanese name when translate"). It appears in the JA byline, the JA `<title>`, the JA meta description and the JA footer. The `name` field in the About record shows both — `チェン・ポーチェン (Cheng Porchheng)` — so a reviewer can match it to the Latin name on the CV.
- Nothing else is confirmed as binding. The copy currently on the site is the working baseline.

## Evidence on Hand

- **Written content only.** Confirmed by the owner: "the contents written is basically it." The site's content is in `index.html`: **four roles** (NBC backend engineer, Biz Solution junior developer and backend intern, CDC API & web intern), **no projects**, skills, three Cisco certifications plus Solid Edge Associate, and languages.
- **NBC copy updated 2026-09-25** from the owner's own git history of the benchmark platform, kept within the disclosure limit: kind of engineering, stack and principles only, with no internal names, architecture, metrics or commit counts. Superseded note below:
- **The NBC role has no written copy yet.** It exists only as the facts recorded above and must be written from scratch, within the disclosure limit. This is the single biggest content gap on the site: its strongest credential is the one thing currently missing.
- **CV:** `CHHENG_PORCHHENG_CV.pdf`.
- **Photos:** `pf.jpeg` (1290×2293, used as the avatar), `IMG_8347.jpeg` (4032×3024, unreferenced), `_MG_2004.png` (a Canon CR2 raw file with a `.png` extension, unreferenced).
- **Confirmed absent; future work must not fabricate:** public repositories, live demos, screenshots, metrics or performance numbers, testimonials, case studies, and client or customer proof.

## Product Principles

1. **Say only what was built.** With no metrics, repos or demos to lean on, credibility comes from specific, truthful writing. Every claim traces to content the owner supplied; nothing is invented, and generic filler is cut.
2. **Japanese is the primary reading path, not a toggle.** The site is sent to Japanese companies as a job application, so the JA view is the one that decides the outcome. It must be complete (title, meta, every tag and chip, `lang` correctness) and it must eventually be proofread by a fluent speaker.
3. **Explain the local context.** Overseas reviewers may not know Cambodia's payment landscape, so terms like KHQR and Bakong are made legible without assuming familiarity.
4. **Built to be sent, not discovered.** The page must stand alone for a reviewer who has never heard of the owner, and should get to the substance fast.
5. **Levels are stated honestly.** Language levels and status claims stay accurate to the owner's own account.
