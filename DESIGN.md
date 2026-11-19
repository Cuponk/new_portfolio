---
name: Justin Aitken — Portfolio
description: A straight two-column developer portfolio where the path statement and the work lead.
colors:
  ground: "oklch(0.985 0.004 220)"
  surface-raised: "oklch(1 0 0)"
  ink: "oklch(0.22 0.015 240)"
  ink-body: "oklch(0.40 0.014 240)"
  ink-muted: "oklch(0.50 0.012 240)"
  rule: "oklch(0.90 0.006 230)"
  rule-strong: "oklch(0.82 0.008 230)"
  accent: "oklch(0.47 0.10 165)"
  accent-ink: "oklch(0.38 0.09 165)"
  accent-soft: "oklch(0.945 0.03 165)"
  data-negative: "oklch(0.62 0.085 45)"
typography:
  display:
    fontFamily: "Schibsted Grotesk, ui-sans-serif, system-ui, sans-serif"
    fontSize: "clamp(2.5rem, 4.2vw, 3.25rem)"
    fontWeight: 600
    lineHeight: 1.05
    letterSpacing: "-0.035em"
  headline:
    fontFamily: "Schibsted Grotesk, ui-sans-serif, system-ui, sans-serif"
    fontSize: "1.375rem"
    fontWeight: 600
    lineHeight: 1.25
    letterSpacing: "-0.02em"
  title:
    fontFamily: "Schibsted Grotesk, ui-sans-serif, system-ui, sans-serif"
    fontSize: "1.1875rem"
    fontWeight: 500
    lineHeight: 1.4
    letterSpacing: "-0.01em"
  body:
    fontFamily: "Schibsted Grotesk, ui-sans-serif, system-ui, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 400
    lineHeight: 1.65
  body-sm:
    fontFamily: "Schibsted Grotesk, ui-sans-serif, system-ui, sans-serif"
    fontSize: "0.875rem"
    fontWeight: 400
    lineHeight: 1.5
  label:
    fontFamily: "Schibsted Grotesk, ui-sans-serif, system-ui, sans-serif"
    fontSize: "0.8125rem"
    fontWeight: 600
    letterSpacing: "0.06em"
  figure:
    fontFamily: "Red Hat Mono, ui-monospace, SF Mono, Menlo, monospace"
    fontSize: "2.5rem"
    fontWeight: 500
    lineHeight: 1
    letterSpacing: "-0.04em"
    fontFeature: "tnum"
  meta:
    fontFamily: "Red Hat Mono, ui-monospace, SF Mono, Menlo, monospace"
    fontSize: "0.8125rem"
    fontWeight: 400
    fontFeature: "tnum"
rounded:
  hair: "2px"
  chip: "4px"
  control: "6px"
  control-group: "8px"
  panel: "12px"
  pill: "999px"
spacing:
  xs: "0.25rem"
  sm: "0.5rem"
  md: "0.75rem"
  base: "1rem"
  lg: "1.5rem"
  heading-gap: "1.75rem"
  item: "2.25rem"
  section: "clamp(4.5rem, 8vw, 6rem)"
  gutter: "clamp(1.5rem, 5vw, 4rem)"
components:
  status-pill:
    backgroundColor: "{colors.accent-soft}"
    textColor: "{colors.accent-ink}"
    typography: "{typography.body-sm}"
    rounded: "{rounded.pill}"
    padding: "6px 12px 6px 10px"
  badge:
    backgroundColor: "{colors.accent-soft}"
    textColor: "{colors.accent-ink}"
    rounded: "{rounded.pill}"
    padding: "2px 8px"
  stack-chip:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.ink-body}"
    rounded: "{rounded.chip}"
    padding: "2px 8px"
  text-link:
    textColor: "{colors.ink}"
  text-link-hover:
    textColor: "{colors.accent-ink}"
  segmented-control:
    backgroundColor: "{colors.ground}"
    rounded: "{rounded.control-group}"
    padding: "3px"
  segmented-button:
    textColor: "{colors.ink-muted}"
    rounded: "{rounded.control}"
    padding: "8px 14px"
  segmented-button-active:
    backgroundColor: "{colors.surface-raised}"
    textColor: "{colors.ink}"
  demo-panel:
    backgroundColor: "{colors.surface-raised}"
    rounded: "{rounded.panel}"
  nav-link:
    textColor: "{colors.ink-muted}"
    typography: "{typography.label}"
  nav-link-active:
    textColor: "{colors.ink}"
---

# Design System: Justin Aitken — Portfolio

## Overview

**Creative North Star: "The Plain Ledger"**

A daylight page that reads like a well-kept record: a near-white ground with the faintest cool tint, near-black ink, and one deep green that marks only what is interactive or what carries data. The form is the category-standard developer portfolio played straight: a sticky left column holding identity, status, in-page navigation and social links, and a wider right column where the path prose and the work lead. Nothing is staged; credibility comes from finish, alignment and honest labels.

Density is calm and editorial. Structure is drawn with hairline rules and whitespace, not boxes; the only true container on the page is the projection explainer, which earns its panel because it is an instrument rather than a section. Type does almost all the hierarchy work with a single grotesk across every role, while a monospace face is reserved for the things a reader scans as data: dates, stacks and numbers.

Motion is small and functional: one long ease-out curve drives every data change and the nav-rule growth, and all of it collapses under reduced-motion. The system rejects AI-glow theatrics (neon, glowing networks, gradients) and the hero + skills grid + equal-card-row template.

**Key Characteristics:**
- Two-column sticky-intro layout that collapses to one column at 900px.
- One accent hue (deep green, 165) used for links on hover, focus, status and data marks.
- Hairline rules as structure; one shadowed panel on the whole page.
- One sans family for all text; mono only for dates, stacks and figures.
- Pills for status, rounded-4px chips for stacks, 12px corners only on the demo panel.

## Colors

A cool, near-neutral daylight palette with a single deep green accent and one warm data colour.

### Primary
- **Ledger Green** (`accent`): the one interactive and data hue. Focus outlines, link underlines on hover, the status dot, positive factor bars, the projection interval band (at 28% opacity) and the caret.
- **Deep Ledger Green** (`accent-ink`): green as text. Link text on hover, status-pill and badge text, the median tick on the projection scale, selection text.
- **Mint Wash** (`accent-soft`): the tint behind green text: status pill, "In progress" badge, mobile contact pill, text selection.

### Secondary
- **Clay** (`data-negative`): negative factor bars in the projection explainer only. A data colour, never text, never UI chrome.

### Neutral
- **Daylight Ground** (`ground`): page background, the segmented-control well, the projection track, the demo footnote band.
- **Paper White** (`surface-raised`): the demo panel, the active segment, stack chips; anything that sits one step above the ground.
- **Ink** (`ink`): headings, the name, link text at rest, strong text in prose, figures.
- **Body Ink** (`ink-body`): running prose and descriptions; the default body colour.
- **Muted Ink** (`ink-muted`): dates, nav labels at rest, social icons at rest, axis labels, footnotes, colophon.
- **Hairline** (`rule`): every divider and chip/panel border.
- **Strong Hairline** (`rule-strong`): link underlines at rest, the zero line in factor bars, the scrollbar thumb.

### Named Rules
**The One Green Rule.** Green appears only where something is interactive, focused, or is data. It never decorates a heading, a section or a background block.

**The Wash-Under-Ink Rule.** Green text always sits on Mint Wash or Daylight Ground, and Mint Wash always carries Deep Ledger Green text, never Ledger Green or Ink.

## Typography

**Display Font:** Schibsted Grotesk (with ui-sans-serif, system-ui, -apple-system, Segoe UI, sans-serif), self-hosted at 400/500/600
**Body Font:** Schibsted Grotesk
**Label/Mono Font:** Red Hat Mono (with ui-monospace, SF Mono, Menlo, monospace), self-hosted at 400/500, always with tabular numerals

**Character:** A sturdy, slightly newsy grotesk carries the whole voice, tightened at large sizes; a quiet mono marks the scannable facts so dates and numbers line up.

### Hierarchy
- **Display** (600, clamp 2.5rem to 3.25rem, line-height 1.05, -0.035em): the name only.
- **Headline** (600, 1.375rem, 1.25, -0.02em): the featured project title. The contact sentence uses the same size at weight 500 with line-height 1.4 and -0.015em.
- **Title** (500, 1.1875rem, 1.4, -0.01em): the role line under the name. Secondary project titles use this size at 600; timeline-row titles step down to 1.0625rem at 600 with a 400-weight Body Ink second line.
- **Body** (400, 1.0625rem, 1.65): prose and project descriptions, capped at 38rem (the intro lede at 22rem).
- **Body Small** (400, 0.875rem to 0.9375rem): timeline descriptions, links rows, demo copy, status pill.
- **Label** (600, 0.8125rem, 0.06em, uppercase): section headings. The in-page nav uses the same treatment at weight 500.
- **Figure** (Red Hat Mono 500, 2.5rem, line-height 1, -0.04em, tabular): the projected median in the demo.
- **Meta** (Red Hat Mono 400, 0.8125rem; stack chips at 0.75rem; axis labels at 0.6875rem): dates, tech stacks, ranges, factor values.

### Named Rules
**The Mono-Means-Data Rule.** Red Hat Mono is set only on dates, tech-stack names and numbers. Prose, headings and buttons are always the grotesk.

**The Small-Caps-Are-Headings Rule.** Uppercase tracked text is reserved for section headings and the section nav. It is the heading itself, never a label stacked above another heading.

## Layout

A centred shell, max 76rem wide, with a fluid gutter (clamp 1.5rem to 4rem) and a 5fr / 7fr two-column grid separated by a fluid gap (clamp 3rem to 6rem). The left column is a full-viewport sticky intro (name, role, lede, status, nav, social pinned to the bottom with `margin-top: auto`); the right column scrolls. Both columns share the same top inset (clamp 4rem to 6.5rem by viewport height) so the name and the first section heading align.

Vertical rhythm: sections are separated by a fluid section space (clamp 4.5rem to 6rem); a section heading sits 1.75rem above its content; list items are 2.25rem tall in padding; timeline rows 1.5rem. Measures are capped at 38rem for reading text.

Responsive: at 900px and below the grid becomes one column, the intro un-sticks, the nav hides, section headings become sticky bars with a 90%-opaque Daylight Ground and an 8px blur, and a fixed "Contact" pill appears top right. At 560px timeline rows stack their date above the content, factor rows wrap the name onto its own line, and the segmented control goes full width.

## Elevation & Depth

Flat by default. Depth is carried by hairlines and by the one-step tonal lift from Daylight Ground to Paper White. The only shadow on the page belongs to the projection explainer: the panel itself, and inside it the active segment of its control.

### Shadow Vocabulary
- **Instrument lift** (`box-shadow: 0 1px 2px oklch(0.22 0.015 240 / 0.04), 0 12px 32px -12px oklch(0.22 0.015 240 / 0.12)`): the demo panel only.
- **Pressed segment** (`box-shadow: 0 1px 2px oklch(0.22 0.015 240 / 0.1), 0 0 0 1px var(--rule)`): the active button in a segmented control.

### Named Rules
**The One Panel Rule.** Sections, projects and timeline entries are separated by hairlines, never boxed. A raised, shadowed panel is reserved for an interactive instrument.

## Shapes

Soft but small. Corners scale with the object: 2px on data bars, 4px on stack chips, 6px on control buttons, 8px on control groups, 12px on the demo panel. Anything that states a status (availability, "In progress", the mobile contact link) is a full pill, and the status dot is a circle. Borders are always 1px hairlines; the projection track is a hairline-bordered pill.

## Components

### Text Links
Quiet ink links that warm to green.
- **Inline:** Ink text, 1px Strong Hairline underline offset 0.22em; on hover the text turns Deep Ledger Green and the underline Ledger Green (0.2s).
- **Action links (links row):** 500 weight, no underline, followed by a 14px stroked northeast arrow that nudges 2px up-right on hover (0.3s ease-out).
- **Focus:** 2px Ledger Green outline, 3px offset, 3px radius, everywhere.

### Status Pill and Badge
- **Status pill:** Mint Wash ground, Deep Ledger Green 0.875rem text, full pill, an 8px Ledger Green dot leading.
- **Badge:** the same colours at 0.75rem, 500 weight, inline after a project title, used for honest status ("In progress").

### Stack Chips
Paper White chips with a Hairline border, 4px corners, Red Hat Mono 0.75rem in Body Ink; wrapped flex row with 6px by 8px gaps.

### Segmented Control
A Daylight Ground well with a hairline border, 8px corners and 3px padding, holding 6px-cornered buttons in 500 0.8125rem Muted Ink. Hover goes to Ink; the pressed button lifts to Paper White with the pressed-segment shadow. State is exposed with `aria-pressed`.

### Navigation
- **Section nav (desktop):** uppercase label links in Muted Ink, each led by a 2rem hairline rule at 55% opacity. Hover and the in-view section (`aria-current`) turn Ink and grow the rule to 4rem at full opacity on the long ease-out (0.45s).
- **Social:** 22px brand icons in Muted Ink, Ink on hover, at the foot of the intro column.
- **Mobile:** nav hides; section headings become sticky frosted bars; a fixed Mint Wash "Contact" pill stays reachable.

### Project Entries
Title row with the title left and a mono date right (baseline aligned, wrapping), description at 38rem, stack chips, then the links row. The featured project ends in a hairline with 3rem below; secondary projects are a hairline-divided list.

### Timeline Rows
Two-column rows (8.5rem mono date, content) divided by hairlines; the title carries the role in Ink and the organisation on a second line in Body Ink at 400.

### Projection Explainer (signature)
The one raised panel: a header strip (title plus segmented control) over a body with a mono median figure, an 80% range, an interval scale (pill track, 28%-opacity green band, Deep Ledger Green median tick, mono axis) and diverging factor bars from a centre zero line (green positive, Clay negative, mono values). A Daylight Ground footnote band labels the data as synthetic. Switching players animates band, tick and bars on the long ease-out (0.6s).

## Do's and Don'ts

### Do:
- **Do** separate sections, projects and rows with 1px Hairline rules and whitespace.
- **Do** keep green for interaction, focus, status and data; text in green is always Deep Ledger Green.
- **Do** set dates, stacks and numbers in Red Hat Mono with tabular numerals, and everything else in Schibsted Grotesk.
- **Do** cap reading measures at 38rem.
- **Do** animate only state and data changes, on `cubic-bezier(0.16, 1, 0.3, 1)`, and drop all transitions under reduced motion.
- **Do** label status honestly with the pill or badge, and label illustrative data inside the component that shows it.

### Don't:
- **Don't** box sections or projects in cards; the raised panel is reserved for an interactive instrument.
- **Don't** add shadows outside the projection explainer.
- **Don't** use neon, glows, gradients or glowing-network imagery.
- **Don't** build the hero + skills grid + equal-card-row template.
- **Don't** put an uppercase label above a heading; uppercase tracked text is the section heading itself.
- **Don't** use Clay for text or UI chrome; it marks negative data only.
