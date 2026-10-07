---
name: Cheng Porchheng, Rirekisho
description: A backend engineer's portfolio set as the Japanese JIS resume form, printed in one green ink with one red seal.
colors:
  ink: "#0B6E4F"
  ink-2: "#2E5E4C"
  paper: "#EAF3EE"
  rule: "#98BCAB"
  tint: "#DCE9E2"
  text: "#16181D"
  text-2: "#3A4741"
  seal: "#D7263D"
  night-desk: "#04140E"
  night-paper: "#0F201A"
  night-band: "#174B3A"
  night-ink: "#5CC79A"
  night-ink-2: "#8FD0B3"
  night-rule: "#244D3D"
  night-tint: "#152D24"
  night-text: "#E4EEE9"
  night-text-2: "#AFC3BA"
  night-seal: "#FF5C6C"
typography:
  form-title:
    fontFamily: "Shippori Mincho B1, Shippori Mincho, Hiragino Mincho ProN, serif"
    fontSize: "44px"
    fontWeight: 800
    lineHeight: 1
    letterSpacing: "0.42em"
  display:
    fontFamily: "Schibsted Grotesk, Zen Kaku Gothic New, Hiragino Sans, sans-serif"
    fontSize: "clamp(34px, 4.6vw, 60px)"
    fontWeight: 700
    lineHeight: 1.05
    letterSpacing: "-0.028em"
  headline:
    fontFamily: "Schibsted Grotesk, Zen Kaku Gothic New, Hiragino Sans, sans-serif"
    fontSize: "22px"
    fontWeight: 700
    lineHeight: 1.3
    letterSpacing: "-0.012em"
  title:
    fontFamily: "Schibsted Grotesk, Zen Kaku Gothic New, Hiragino Sans, sans-serif"
    fontSize: "18px"
    fontWeight: 600
    lineHeight: 1.35
  data:
    fontFamily: "Schibsted Grotesk, Zen Kaku Gothic New, Hiragino Sans, sans-serif"
    fontSize: "17px"
    fontWeight: 600
    lineHeight: 1.6
    fontFeature: "tnum, lnum"
  body:
    fontFamily: "Schibsted Grotesk, Zen Kaku Gothic New, Hiragino Sans, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.6
  body-long:
    fontFamily: "Schibsted Grotesk, Zen Kaku Gothic New, Hiragino Sans, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.72
  label:
    fontFamily: "Shippori Mincho B1, Shippori Mincho, Hiragino Mincho ProN, serif"
    fontSize: "14px"
    fontWeight: 700
    lineHeight: 1.35
    letterSpacing: "0.08em"
  label-en:
    fontFamily: "Schibsted Grotesk, Zen Kaku Gothic New, Hiragino Sans, sans-serif"
    fontSize: "12px"
    fontWeight: 500
    lineHeight: 1.35
  control:
    fontFamily: "Schibsted Grotesk, Zen Kaku Gothic New, Hiragino Sans, sans-serif"
    fontSize: "15px"
    fontWeight: 600
rounded:
  none: "0px"
  hairline: "2px"
  control: "4px"
spacing:
  cell-y: "12px"
  cell-x: "20px"
  block-body: "24px 28px 28px"
  block-gap: "34px"
  block-gap-mobile: "24px"
  sheet: "44px 52px 56px"
  sheet-mobile: "22px 16px 30px"
  history-year: "88px"
  history-month: "60px"
components:
  button-primary:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    typography: "{typography.control}"
    rounded: "{rounded.control}"
    padding: "0 20px"
    height: "48px"
  button-secondary:
    backgroundColor: "transparent"
    textColor: "{colors.ink}"
    typography: "{typography.control}"
    rounded: "{rounded.control}"
    padding: "0 20px"
    height: "48px"
  button-secondary-hover:
    backgroundColor: "{colors.tint}"
  band-action:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "0 14px"
    height: "38px"
  band-tab:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    rounded: "{rounded.none}"
    padding: "0 20px"
    height: "60px"
  band-tab-current:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.ink}"
  form-cell-label:
    textColor: "{colors.ink}"
    typography: "{typography.label}"
    padding: "12px 16px"
    width: "150px"
  block-head:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.paper}"
    padding: "12px 20px"
  history-row-hover:
    backgroundColor: "{colors.tint}"
---

# Design System: Cheng Porchheng, Rirekisho

## Overview

**Creative North Star: "The Filled-In Rirekisho"**

The page is a 履歴書, the JIS resume form a Japanese reviewer handles every working day, printed in one saturated green ink on pale green stock and filled in with a typed grotesk. Every surface is a part of that form: name cells, a photo box, a year and month history table, ruled free-text fields, fixed-field boxes. Nothing is a card, a hero or a skills grid. The reviewer should recognise the document before reading a word of it.

Density is the form's density: tight ruled cells, labels in small Mincho, values at reading size. Hierarchy comes from the frame (2px outer, 1px inner rules, solid green header bars), not from scale jumps or color. Red appears once, as the 在職中 seal pressed on the current post. Dark mode is the same form at night: a deep green sheet with the ink lifted so it still reads.

The world refuses the developer-portfolio arrangement (hero, cards, skills grid) and the earlier API-reference costume.

**Key Characteristics:**
- One green ink prints every frame, rule, label and header bar; one red seal is spent once.
- Two voices: Shippori Mincho B1 prints the form, Schibsted Grotesk fills it in.
- Every label is bilingual: Japanese always, English beneath for English readers, hidden in JA.
- Square frames, ruled tables and dotted or dashed separators carry all structure.
- The sheet sits on a green desk, lifted by a single soft paper shadow.

## Colors

A monochrome green print on green-tinted paper, with near-black typed entries and a single red stamp.

### Primary
- **Form Ink** (ink): the one printing ink. Frames, rules (mixed with paper), Mincho labels, header bars, the section band, the desk behind the sheet, primary buttons, period dates and the plus/minus marks. In light mode the desk, ink and band are the same value by design.
- **Faded Ink** (ink-2): English sub-labels under the Japanese ones, and the current tab's English line.

### Secondary
- **Seal Vermilion** (seal): the 在職中 stamp on the current role, and nothing else. Night value is night-seal.

### Neutral
- **Form Stock** (paper): the sheet, the text on green bars and buttons, the cut-out current tab.
- **Printed Rule** (rule): every 1px inner rule, dotted detail separator and ruled writing line. Canonical source is `color-mix(in oklab, ink 40%, paper)`; 30% at night.
- **Field Tint** (tint): row hover, table header fill and secondary button hover. Canonical source is `color-mix(in oklab, ink 7%, paper)`; 9% at night.
- **Typed Black** (text): the filled-in entries: name, organisation, values, bold emphasis.
- **Typed Grey-Green** (text-2): roles, bullet prose, furigana, secondary table cells.
- **Night Desk / Night Paper / Night Band** (night-desk, night-paper, night-band): the dark theme splits the band off the ink so the bar stays dark while the ink lightens to night-ink.

### Named Rules
**The One Ink Rule.** Everything printed on the form is the ink color or a mix of it with paper. No second structural hue, no grey borders, no blue links.

**The Single Seal Rule.** Red is the seal and only the seal: one stamp, on the current post, per page. It never colors text, buttons, errors or hover states.

**The Typed Entry Rule.** Content a person "wrote in" is text or text-2, never ink. Ink is reserved for what the form printed.

## Typography

**Display Font:** Shippori Mincho B1 (with Shippori Mincho, Hiragino Mincho ProN, serif)
**Body Font:** Schibsted Grotesk (with Zen Kaku Gothic New, Hiragino Sans, sans-serif)
**Label/Mono Font:** Zen Kaku Gothic New for the furigana line; Yuji Syuku, subset to 在職中, for the seal only.

**Character:** A printed Japanese form in a fine Mincho, completed in a crisp, slightly condensed grotesk. The contrast between printed and typed is the whole hierarchy.

### Hierarchy
- **Form Title** (Mincho 800, 44px, line-height 1, tracking 0.42em): 履歴書 only, with negative right margin equal to the tracking. 36px under 900px, 32px under 720px.
- **Display** (Grotesk 700, clamp(34px, 4.6vw, 60px), 1.05, tracking -0.028em): the name in the 氏名 cell. 30px on phones.
- **Headline** (Grotesk 700, 22px, 1.3, -0.012em, balanced wrap): the heading inside an opened history row. 20px in JA with no tracking and keep-all breaking.
- **Title** (Grotesk 600, 18px, 1.35): the organisation in each history row.
- **Data** (Grotesk 600, 17px, tabular lining figures): year and month cells.
- **Body** (Grotesk 400, 16px, 1.6): values in cells and rows. Long bullets use 1.72 at 68ch; summary prose runs to 72ch on ruled lines.
- **Label** (Mincho 700, 14px, 1.35, tracking 0.08em, ink): the printed Japanese field name. Wider tracking (0.3em to 0.7em) for centred section and closing marks such as 職歴 and 以上.
- **Label EN** (Grotesk 500, 12px, 1.35, ink-2): the English gloss beneath each Japanese label.
- **Control** (Grotesk 600, 15px; 13px inside the band): buttons and toggles.

### Named Rules
**The Printed and Typed Rule.** Mincho is the form; Grotesk is the applicant. Never set a filled-in value in Mincho or a printed field name in Grotesk.

**The Bilingual Label Rule.** Every printed label is a Japanese line in Mincho with an English gloss beneath it. In the JA view the gloss is removed, never translated into the Mincho line.

**The Tabular Date Rule.** Every year, month and period uses tabular lining figures so the history columns align.

## Layout

A single sheet, max 1180px, centred on the desk with 36px/28px of desk showing around it. The sheet pads 44px 52px 56px.

The form head is a two-column grid: name cells on the left, a 200px photo column on the right with a 36px gap. Cells are a 150px label column against a fluid value column. Below it, the section band runs full sheet width (negative margins) and pins to the top on scroll. The history is a three-column table: 88px year, 60px month, fluid entry; the two column rules run through every row, including expanded detail. Opened rows split into prose and a 300px facts box with a 40px gap. Blocks below the table stack with 34px gaps; certifications and languages pair at 1.5fr : 1fr.

Breakpoints: at 1060px the detail stacks; at 900px the pair stacks, the photo column narrows to 150px and labels to 120px; at 720px the sheet goes edge to edge (no desk, no shadow, 16px gutters), the photo moves into the name cells as a 96px cell, history columns shrink to 54px and 36px, the expanded detail covers the year and month rules, key/value rows stack, and the band shows one line per tab in the reader's language only. Print drops the band and controls and opens every row.

## Elevation & Depth

Flat paper on a desk. The sheet is the only lifted object; everything on it is printed flat and separated by rules. Two secondary shadows exist: the pinned band casts a short shadow onto the sheet beneath it, and the photo sits on the sheet like a pasted print. Paper tooth is a faint fractal-noise grain over the sheet (multiply at 0.5 opacity; screen at 0.35 in dark).

### Shadow Vocabulary
- **Sheet** (`box-shadow: 0 1px 2px rgba(3,40,28,.28), 0 24px 48px -18px rgba(3,40,28,.55)`): the paper on the desk. Night uses black at 0.5 and 0.8. Removed on phones and in print.
- **Pinned band** (`box-shadow: 0 10px 18px -14px rgba(3,40,28,.6)`): the sticky section band only.
- **Pasted photo** (`box-shadow: 0 1px 1px rgba(0,0,0,.18), 0 6px 14px -6px rgba(3,40,28,.45)`): the applicant photo only.

### Named Rules
**The One Sheet Rule.** Only the sheet lifts off the desk. Blocks, tables and rows on it never take a shadow; they take a frame.

## Shapes

Square everywhere the form is printed: sheet, cells, tables, blocks, header bars and tabs have 0 radius. Frames are 2px solid ink on the outside, 1px rule inside. Separators carry meaning: dashed between furigana and name and around the photo box, dotted above opened detail, solid elsewhere. Free-text fields draw the form's own writing lines as a repeating 1px rule every 31px (29px on phones). The only round forms are printed rings (7px bullet rings, 5px skill separators, both 1.5px ink outlines) and the seal. Interactive controls take a 4px radius (2px inside the segmented control) so they read as things to press, not fields of the form.

## Components

### Buttons
Plain, inked and square-shouldered; they read as stamped instructions on the form.
- **Shape:** gently squared corners (4px), 48px tall, 0 20px padding, 15px semibold, 16px icon with a 10px gap.
- **Primary:** solid ink with paper text. Hover deepens toward typed black (ink 86% with text).
- **Secondary:** transparent with a 1.5px ink border and ink text. Hover fills with tint.
- **Focus:** 2px solid outline in text color, 3px offset, on every interactive element; on-band color inside green bars.
- **Phones:** buttons in an action row grow to share the width.

### Band Controls
- **Language switch:** a segmented pair inside a 1px border (on-band 45% into band), 4px outer and 2px inner radius. The pressed option is solid paper with ink text. On phones only the language you can switch to is shown.
- **Theme button:** 44px square, same border, moon or sun stroke icon.
- **Download CV:** solid paper on the green band with ink text, 38px tall; shortens to "CV" on phones.

### Cards / Containers
There are no cards. Containers are form blocks.
- **Corner Style:** square (0).
- **Background:** paper, inside a 2px ink frame.
- **Head:** a solid ink bar with the bilingual label in paper, 12px 20px padding.
- **Shadow Strategy:** none (see The One Sheet Rule).
- **Internal Padding:** 24px 28px 28px; 18px 14px 22px on phones.

### Navigation
The section band is the form's heading strip, pinned while reading. Each tab stacks the Mincho label over the English gloss, 60px tall, 20px side padding. Hover lifts the band 12% toward paper. The current section is cut out of the band: paper background, ink text, as if opening onto the sheet below. On phones the tab row scrolls with soft edge masks and drops to one language line.

### History Table (signature)
Year, month and entry in fixed columns with continuous vertical rules and a solid ink header row. Group rows (職歴, 学歴) are centred, widely tracked Mincho. Job rows are full-width buttons: hover fills with tint, a plus mark loses its upright on open (0.35s), and the detail opens by animating grid rows from 0fr to 1fr over 0.5s on the expo-out curve. The table closes with 以上 set right. Education rows are plain lines with no toggle.

### Facts Box
A fixed-field box beside opened detail: 1px rule frame, an 84px Mincho key column in ink, 14px values in text.

### Form Cells and Rows
Label column in Mincho ink, value column in Grotesk text, 1px rule between. Links in values underline at 1px in rule color, offset 4px, and darken to ink on hover. Skill rows list items inline, separated by small ink rings.

### Seal
A red circular 在職中 stamp in Yuji Syuku, 82px (58px on phones), rotated -9deg, multiply-blended into the paper, with an SVG ink filter that roughens the edge and drops grain from the fill. It presses once on load (0.66s overshoot) and is static under reduced motion.

## Do's and Don'ts

### Do:
- **Do** print every frame, rule and label in the one ink; derive rules and tints by mixing ink into paper (40% and 7%; 30% and 9% at night).
- **Do** give every new field a bilingual label: Mincho Japanese over a 12px Grotesk English gloss.
- **Do** build new content as a part of the form: a ruled block with an ink head bar, a key/value row, or a history row.
- **Do** frame blocks with 2px ink outside and 1px rule inside, square cornered.
- **Do** keep numerals tabular and lining in every date and table column.
- **Do** use the expo-out curve (cubic-bezier(.16,1,.3,1)) for opening and closing, and 0.18s to 0.2s ease for hover fills.
- **Do** keep JA typesetting strict: line-break strict, keep-all on headings, no Latin tracking on Japanese headings.

### Don't:
- **Don't** use red for anything but the single seal on the current post.
- **Don't** add a second structural color, grey borders or blue links.
- **Don't** arrange content as a hero, cards or a skills grid; the page is a form, not a portfolio template.
- **Don't** put shadows on blocks, rows or buttons; only the sheet, the pinned band and the photo cast one.
- **Don't** round the form's frames, cells or tables; radius belongs to controls only (4px).
- **Don't** set typed content in Mincho or printed labels in Grotesk.
- **Don't** use gradients except to draw ruled writing lines and scroll-edge fades.
