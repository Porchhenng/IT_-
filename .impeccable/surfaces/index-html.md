---
version: 1
slug: "index-html"
primary_target: "index.html"
related_targets: []
---

## Scope and visitor mode

Single-file static site `index.html` (no framework, no build step, no package manager). Visitor mode: **Persuade**. There is no artifact to stand inside; the proof is written record, and the visitor arrives to decide.

## Audience, job, action, proof

A reviewer at a Japanese IT company opens the link sent with a full-time job application, alongside the CV. They have never heard of him and may be screening in HR before an engineer sees it. Primary action: reply, download the CV, or pass it on internally with a yes. Proof is written content only (PRODUCT.md, Evidence on Hand); nothing may be invented.

## Chosen direction: Rirekisho, in full colour (branch design/rirekisho)

From the direction round recorded in `.impeccable/decision/direction-1141fbff.json` (option `model-pick`, Impeccable's pick; the roll dealt Station Signs, built on `design/station-signs`). The user asked for this one built as its own branch, 2026-10-07. Code-led; no comp.

**Thesis:** the page is the JIS 履歴書 the reviewer reads every working day, filled in and printed in one green ink. It replaces the API Reference world on `main` wholesale.

**Composition:** one long form on a green desk, read top to bottom. Head: 履歴書 title and 現在 date, name cells (ふりがな, 氏名, 現職, 現住所, 連絡先) and the 写真 box (`cv-photo-print.jpg`). A pinned green band carries the section headings (学歴・職歴, 自己PR, 特技・スキル, 免許・資格, 連絡先) plus language, theme and CV. Then the history table, year | month | entry, newest first (職歴 above 学歴, a deliberate departure from the form's chronological order so NBC leads), closed by 以上. Each role opens in place; NBC is open on arrival. Below: 自己PR and 本人希望 on ruled writing lines, skills as ruled rows, certifications and languages as two ruled tables.

**Bilingual labels:** printed labels always show Japanese; English sits under it in EN mode and disappears in JA mode. Content swaps by `data-i18n`.

**Months left blank** on the education rows: the record gives years only. Do not fill them.

## Memorable moment

The **在職中 seal**: one red SVG hanko with an ink-wear filter, pressed with a single stamp animation on the NBC row once fonts load. Red is spent only there. Reduced motion shows it already pressed.

## Boundaries and anti-goals

No second accent colour, no extra motion, no chips or cards. Old hashes (#nbc, #biz, #ecommerce, #cdc) open the matching row. No invented metrics, repos, demos, months or claims; no visa or relocation claim (a comment reserves the 本人希望 slot).

## States and ranges

Four roles, three education rows, 34 skill entries in six groups, four certifications, three languages. States: language (Japanese by browser detection, choice persisted), theme, rows open or closed (Open all / Close all), no-JS (every row open, seal visible), reduced motion, print (band hidden, all rows open). Below 720px the photo moves inside the form beside ふりがな and 氏名, the band shows one language switch and a short CV button, and an open role's detail spans the full width.

## Unresolved decisions (a builder must not invent these)

1. **NBC job title as it appears on his contract.** Recorded as "Backend Engineer" from his own phrasing only.
2. **What the NBC entry may say**, checked against his employer's actual rules. Public information only (PRODUCT.md).
3. **Visa, relocation, remote availability, start date.** Unsettled; the 本人希望 row reserves the place.
4. **Japanese proofreading.** Never read by a fluent speaker. New form vocabulary on this branch (現職, 所属, 職種, 期間, 対象, 範囲, 技術, 製品, 決済, 利用先, 資格名, 発行・区分, 本人希望, 連絡, 入学 / 卒業 / 受講開始) is also unreviewed.
5. **Street address**: the site shows city only (Phnom Penh, Cambodia); keep as is unless the owner asks.
6. **CV filename and the name inside the PDF.**
