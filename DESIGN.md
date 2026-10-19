---
name: Lord 4L Barber
description: Quiet-luxury barbershop landing — charcoal ground, one gold accent, Playfair Display over Inter, bronze hairlines, flat depth.
colors:
  ground: "#111110"
  surface: "#1a1917"
  surface-2: "#242220"
  ink: "#f5f2eb"
  ink-soft: "#a8a196"
  gold: "#c9a45c"
  gold-soft: "#e0c58c"
  gold-deep: "#a5823e"
  rule: "#35302a"
typography:
  display:
    fontFamily: "Playfair Display, Georgia, Times New Roman, serif"
    fontSize: "clamp(2.7rem, 5.4vw, 4.75rem)"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "-0.015em"
  headline:
    fontFamily: "Playfair Display, Georgia, Times New Roman, serif"
    fontSize: "clamp(1.9rem, 3.4vw, 2.9rem)"
    fontWeight: 600
    lineHeight: 1.04
    letterSpacing: "-0.01em"
  brand:
    fontFamily: "Playfair Display, Georgia, Times New Roman, serif"
    fontSize: "1.3rem"
    fontWeight: 600
    lineHeight: 1
    letterSpacing: "0.01em"
  title:
    fontFamily: "Playfair Display, Georgia, Times New Roman, serif"
    fontSize: "1.375rem"
    fontWeight: 500
    lineHeight: 1.15
    letterSpacing: "-0.005em"
  price:
    fontFamily: "Inter, Segoe UI, Arial, sans-serif"
    fontSize: "1.0625rem"
    fontWeight: 700
    lineHeight: 1.4
    letterSpacing: "0.02em"
    fontVariantNumeric: "tabular-nums"
  body:
    fontFamily: "Inter, Segoe UI, Arial, sans-serif"
    fontSize: "clamp(1rem, 1.15vw, 1.0625rem)"
    fontWeight: 400
    lineHeight: 1.65
  body-sm:
    fontFamily: "Inter, Segoe UI, Arial, sans-serif"
    fontSize: "0.9375rem"
    fontWeight: 400
    lineHeight: 1.55
  caption:
    fontFamily: "Inter, Segoe UI, Arial, sans-serif"
    fontSize: "0.8125rem"
    fontWeight: 600
    lineHeight: 1.5
    letterSpacing: "0.08em"
  label:
    fontFamily: "Inter, Segoe UI, Arial, sans-serif"
    fontSize: "0.75rem"
    fontWeight: 700
    lineHeight: 1.2
    letterSpacing: "0.12em"
    textTransform: "uppercase"
rounded:
  sm: "0.25rem"
spacing:
  xs: "0.75rem"
  sm: "1rem"
  md: "1.5rem"
  lg: "1.75rem"
  xl: "2rem"
components:
  button-primary:
    backgroundColor: "{colors.gold}"
    textColor: "{colors.ground}"
    rounded: "{rounded.sm}"
    padding: "1rem 1.7rem"
    typography: label
  button-primary-hover:
    backgroundColor: "{colors.gold-deep}"
    textColor: "{colors.ground}"
    rounded: "{rounded.sm}"
    padding: "1rem 1.7rem"
    typography: label
  button-ghost:
    backgroundColor: "transparent"
    textColor: "{colors.gold-soft}"
    rounded: "{rounded.sm}"
    padding: "1rem 1.7rem"
    typography: label
---

# Design System: Lord 4L Barber

## Overview

**Creative North Star: "Cadeira à Meia-Noite"**

The page is the chair under a single shop lamp after dark: a charcoal ground, warm ivory type, and exactly one gold line that carries every action. "Cadeira à Meia-Noite" names the whole system — calm, expensive-by-attitude rather than by price, confident without noise. The visitor should feel a dark, well-run room before reading a word: the shop's own animated mark is the only moving object, and the gold is reserved for the one thing to do.

The visual language is quiet luxury for a neighborhood barbershop. The ground is near-black, the text is warm off-white, and a single muted gold (#c9a45c) is the only chroma. Depth is made of 1px bronze hairlines and slightly lifted charcoal fields, never shadows. The type does the composing — Playfair Display gives the serif voice, Inter keeps prices, labels and navigation matter-of-fact.

**Key Characteristics:**
- Charcoal-first: a warm near-black ground (#111110) with warm ivory text — never pure #000, never a light page
- Single spot discipline: gold is the only chroma; it means act, link, or here
- Serif display / sans body: Playfair Display headlines against Inter's neutrality
- Flat by law: no shadows anywhere; 1px bronze rules, hairlines and full-bleed fields build the page
- Flush photographs, small controls: media is cut square; only buttons carry a 0.25rem radius
- One arrival curve: everything that moves uses the same settle easing

## Colors

A charcoal palette built on one spot accent and a warm-neutral ramp. Gold is the voice; the charcoals are the room.

### Primary
- **Gold** (#c9a45c): The entire accent system — CTA fill, brand numeral, service prices, links and handles, the animated mark's eyes, focus outline, section-band row highlight. Used sparingly; most of every view is charcoal and ivory.
- **Gold Soft** (#e0c58c): Gold as text on dark — ledger prices, the handle, the italic hero phrase, the "Agendar" nav item. The legible face of the accent.
- **Gold Deep** (#a5823e): The pressed state — button hover/active — one step down, same hue.

### Neutral
- **Ground** (#111110): Page ground. Every screen starts here. A warm near-black, deliberately not #000.
- **Surface** (#1a1917): The lifted field — the services band and the contact colophon — one step up from the ground, still charcoal.
- **Surface 2** (#242220): The second lift, reserved for row and control hover grounds.
- **Ink** (#f5f2eb): Primary text — headlines, body, values. Warm off-white, never #fff.
- **Ink Soft** (#a8a196): Secondary text — decks, descriptions, captions, footer, nav at rest.
- **Rule** (#35302a): 1px bronze hairlines and dividers — the pencil line of the layout, plus photo and control borders.

### Named Rules
**The One Accent Rule.** Gold, Gold Soft and Gold Deep are the only chroma in the system. If a second hue appears, the room is no longer this room.

## Typography

**Display Font:** Playfair Display (Georgia, Times New Roman, serif fallback)
**Body Font:** Inter (Segoe UI, Arial, sans-serif)

**Character:** A high-contrast editorial serif speaking over a neutral grotesque. Playfair Display carries the essay voice — headlines, service names, the wordmark, the drop cap; Inter keeps prices, labels, and navigation matter-of-fact. Italic Playfair 500 is reserved for the one emphasized phrase in the hero deck.

### The Ramp
Nine named steps, each one live in `css/style.css` as a `--type-*` custom property. No role may carry an off-ramp value; if a new size is needed, it earns a name and a place in this list.

| Step | Token | Size | Weight | Tracking | Role |
|---|---|---|---|---|---|
| Display | `--type-display` | clamp(2.7rem, 5.4vw, 4.75rem) | 600 | -0.015em | Hero statement only — one per screen, max 12ch, lh 1 |
| Headline | `--type-headline` | clamp(1.9rem, 3.4vw, 2.9rem) | 600 | -0.01em | Section titles, max 17ch, text-wrap balance, lh 1.04 |
| Brand | `--type-brand` | 1.3rem | 600 | 0.01em | Header wordmark — Playfair, gold numeral |
| Title | `--type-title` | 1.375rem | 500 | -0.005em | Service names, contact details heading, hero subtitle |
| Price | `--type-price` | 1.0625rem | 700 | 0.02em | Prices — tabular figures so columns align |
| Body | `--type-body` | clamp(1rem, 1.15vw, 1.0625rem) | 400 | normal | Hero deck and section intros, lh 1.65 |
| Body small | `--type-body-sm` | 0.9375rem | 400 | normal | Service descriptions, detail copy, lh 1.55 |
| Caption | `--type-caption` | 0.8125rem | 600 | 0.08em | Hero meta line — uppercase fiction |
| Label | `--type-label` | 0.75rem | 700 | 0.12–0.18em | Nav, buttons, ledger labels, footer — the system's texture |

Notes on the steps that carry the hierarchy:
- **Display is capped at 4.75rem** — the hero text column is 43% of the stage, so the high-contrast Playfair at 12ch needs the margin. The hero statement is the only Display instance on the page.
- **Brand is the serif, set as a wordmark** — Playfair 600 with the "4" in gold over a tracked uppercase Inter "BARBER". The brand mark sits beside the logo in a 2.75rem circle.
- **No eyebrows, no kickers.** Sections never open with a small caps label above the title; the headline is the first thing said. The one uppercase texture left is functional: nav, buttons, ledger labels, captions, the brand subtitle.
- **Leading rides the step.** The line-height column above is part of each step. The generic section-paragraph rule is `:where(.section p:not(.section__intro))` so it holds specificity 0 — a default layer; every component declares its step's size *and* leading together and genuinely wins.

### Named Rules
**The Label Rule.** Uppercase with 0.12–0.18em tracking belongs to short functional strings only — nav items, buttons, table labels, captions, the brand subtitle. Never a sentence.

## Layout

A bleed grid. Content lives on a centered stage of `min(100% - 3rem, 1160px)`; the header spreads with a matching `--gutter` formula so brand and nav align with the content edges. Sections breathe with `clamp(4rem, 8vw, 6.5rem)` vertical padding, separated by 1px Rule hairlines — except the services band, which is its own field of Surface and needs no divider.

The hero is a full-bleed grid: the text column starts at the stage's left edge, and the animated mark runs to the right edge of the viewport (`grid-template-columns` with named `[full-start] … [media-end full-end]` lines). The split holds down to 901px. At 900px and below the hero stacks and centres as one: the statement, subtitle, deck, intro and meta each take `margin-inline: auto` under `text-align: center`, and the mark leaves the viewport-height panel behind to become a `4/5` plate capped at `min(100%, 30rem)`, centred beneath the text. The cap keeps the band from stretching to a full-width portrait slab on tablets, and centring the plate means the emblem never reads as pushed to one side — the earlier 55fr/45fr split here kept the mark bleeding to the right edge, which read as off-centre on smaller screens. The services band lifts the page: full-width Surface, the price list set as a printed ledger in two side-by-side columns on desktop (name and description left, tabular price right, an ink-tinted hairline between rows) and collapsing to a single column below 700px. The contact section is a colophon on Surface: intro and CTA left, a definition list of facts right behind a vertical hairline, stacking below 900px. The header collapses to a toggle at 700px — below which brand and nav can no longer share a line with real slack. Below 600px the stage narrows to 1rem gutters.

Spacing rhythm: 0.75rem (label gaps) → 1rem (grid gaps) → 1.5rem (row padding) → 2rem (column gaps) → 2.5–3.5rem (hero text insets). Everything else is fluid clamp().

### Anchors and the sticky bar
Every target section carries `scroll-margin-top: calc(var(--scroll-offset) + var(--scroll-gap))`, where `--scroll-offset` measures the closed sticky header (5.5rem desktop, 4.75rem at ≤700px). Navigation updates `aria-current="true"` on the section under the viewport's mid band, painted as an ivory underline distinct from hover's gold.

## Elevation & Depth

**The Flat-By-Default Rule.** There are no shadows in this system — not on buttons, not on media, not on the header. Depth is built the way a dark room builds it: 1px bronze hairlines, full-bleed color fields (the Surface bands), and the ground/ink contrast itself. Hover states change color or underline, never elevation.

## Shapes

Square media, small controls. The hero's animated mark is cut flush — 0 radius, honest edges. Interactive elements (buttons, the map frame) use 0.25rem; the brand mark is the one circle (2.75rem). Borders are 1px Rule hairlines throughout.

## Components

### Buttons
- **Shape:** 0.25rem corners, uppercase Label type, min-height 3rem, padding 1rem 1.7rem.
- **Primary:** Gold fill, Ground text — "Agendar pelo WhatsApp", the page's only filled CTA, in the contact section. Its label leads with the WhatsApp glyph drawn in currentColor (Ground on the gold fill).
- **Hover / Press:** fill steps to Gold Deep over 180ms; `:active` scales 0.98 over 150ms. Focus gets the global 2px gold outline at 3px offset.

### Masthead (Header)
- Sticky bar, Ground background, 1px Rule border beneath. Brand left — the shop mark in a 2.75rem circle beside the Playfair wordmark (gold numeral over a tracked "BARBER"). Nav right: Label-step links, Ink Soft at rest with transparent underline; hover/focus turns text and underline gold; the current section wears an ivory underline via `aria-current`. The "Agendar" item is gold at rest with no underline — it never wears the "current" bar, so it reads as an action and not a selected section; hover/focus brightens it to Gold Soft with a matching underline. The same WhatsApp glyph — spanning 1.15em and inheriting currentColor — sits ahead of the word. A quiet second CTA that does not fill.
- Links carry a 2.75rem min-height so the tap target clears 44px.

### Hero
- Full-bleed split: the statement (Display), the subtitle (Title step, Playfair) carrying the promise "Mais que um corte: um ritual de presença.", the deck with one Playfair italic phrase, the brand paragraph (`.hero__intro`), and a meta line of hours and address — against the shop's animated logo mark running to the viewport edge as a silent, looping emblem. The split is even (1fr/1fr) so the mark reads as a full half of the spread rather than a panel pushed to the right edge. No CTA and no price ledger live here: the hero promises, the page converts further down. The mark pauses under reduced motion, and the poster frame holds its place before the first video frame. At 900px and below the hero stacks and centres: the text column centres itself (h1, subtitle, deck, intro and meta each `margin-inline: auto` under `text-align: center`) and the mark becomes a `4/5` plate capped at `min(100%, 30rem)`, centred beneath the text, so the emblem is symmetric on every smaller screen instead of a plate pinned against the right edge.

### Service Ledger
- The price list as a printed ledger on the Surface band, split into two columns of five and four rows on desktop and collapsed to a single column below 700px. Each row is a grid of name (Title step) + description (Body small) against the price (Price step, tabular, Gold Soft); the row hairline now does all the separating — the dotted leader is gone, it had nothing left to join. The three graduated services carry a quiet Ink Soft "a partir de" before the number.
- Hover or focus-within fills a row with Gold and flips its text to Ground — the lamp finding one line. Each row carries a horizontal inset (`clamp(0.85rem, 1.8vw, 1.15rem)`) so the gold field never runs flush against the name or the price; the row hairline still spans the full column width.
- The list arrives as a list (see Motion) and is always complete: all nine services render at rest.

### Gallery
- The live Instagram feed, embedded through the client-managed Elfsight widget. It is a protected region: outer spacing only, no chrome restyling, no markup edits. The `@lord.4l` handle above it is the page's own link.

### Contact Colophon
- Surface field, two columns: headline, intro, CTA and status line left; a `<dl>` of facts (telefone, horário, Instagram, endereço) right behind a vertical Rule hairline that becomes a top border when stacked. Each fact label carries a drawn 1.6-stroke line icon (phone, clock, pin, camera) in Gold Soft beside the Ink Soft caps label — the icon anchors the row, the label names it. The map is an `<iframe>` with a 1px Rule border at 0 radius; the address is itself a link — third-party embeds fail silently, so the fallback is the fact, not the frame.

### Collapsible Menu (≤700px)
- **Toggle:** "Menu" label plus two bars in currentColor that rotate into an X. Hover and open take gold.
- **One source of truth:** the state lives only in the toggle's `aria-expanded`; CSS reads that attribute, the script also marks the nav with `data-open`.
- **Progressive enhancement:** `html[data-nav-toggle="ready"]` is written by `script.js`. Without it the toggle stays hidden and the nav renders as an ordinary visible list.
- **Panel:** in flow, not overlaid — it pushes content down; no focus trap. Each label is a full row separated by Rule hairlines; rows settle in with a 40ms stagger. Closing on link click, outside click, and Escape (returning focus to the toggle) keeps the closed header's height as the one `scroll-margin-top` must clear.

## Motion

Motion has one job in Cadeira à Meia-Noite: the room going dark and coming up around the visitor, and the confirmation of what a hand just did. Nothing loops, nothing floats.

### The Focal Moment — *the room settles*
The hero arrives once, in three movements sharing one curve:

- **The veil lifts.** A flat Ground veil (`.hero__media::after`, opacity only) lifts off the animated mark while it settles from `scale(1.045)` — the dark room coming up around the emblem.
- **The statement is pressed.** The h1 reveals through a `clip-path` inset that opens upward from below, like type being pressed into the page.
- Both are compositor-only (`opacity`, `transform`, `clip-path`). No animated filter, blur, or backdrop: the video's poster frame is the LCP and the audience is mobile-first.

The deck, the merged intro paragraph, and the meta line are deliberately outside the choreography — present in the first frame, focus ring included.

### Supporting Motion
- **Service ledger** — the `<ul>` arrives as a list: nine siblings, 40ms apart, 320ms each, total capped at ~640ms. The animation is bound to `[data-revealed]` (set by the observer when the group crosses the fold, with a 5s safety net that force-reveals anything still pending); `[data-reveal]` only marks it as a candidate and pre-hides the rows so the entrance cannot flash. Before JS claims the scene the list is visible in its natural state — no script, no observer, nothing hidden.
- **Menu panel (≤700px)** — each row settles 40ms after the one above, 200ms each. The panel itself is never animated: it lives in flow.
- **Press** — `.action:active` takes `scale(0.98)` over 150ms.

### Rules
- **One curve.** `--ease-settle` (`cubic-bezier(0.16, 1, 0.3, 1)`) for every arrival in the system. No bounce, no elastic, no second curve.
- **The visible default.** Resting state is the finished state: veil at opacity 0, no clip, no transform. Every entrance uses `animation-fill-mode: backwards`, so animations supply the transit and never the truth.
- **Type, never controls.** A `clip-path` may reveal a heading; it may never cover an interactive element.
- **Reduced motion** collapses durations and delays to 0.01ms and drops the smooth scroll. Every animation here ends in the visible state, so the collapse costs movement and nothing else. The hero video is also paused by script under reduced motion — the poster frame stands in for it.

## Do's and Don'ts

### Do:
- **Do** keep grounds charcoal and text Ink; reach for Gold only to act, link, or mark the current place.
- **Do** build depth with 1px bronze rules and full-bleed Surface fields — never with shadows.
- **Do** set media flush: 0 radius, `object-fit: cover`.
- **Do** write labels, nav, and buttons uppercase with 0.12–0.18em tracking — short strings only.
- **Do** set every font-size from a `--type-*` token, and add the step to the Ramp table above before shipping it.
- **Do** honor prefers-reduced-motion: kill smooth scroll, and collapse both transitions and entrance animations to near-zero.
- **Do** reach for the global focus style: 2px Gold outline, 3px offset, on every interactive element.

### Don't:
- **Don't** add shadows, gradients, or blur — the room is lit by the field, not by elevation.
- **Don't** introduce a second chroma or lift the ground to a light page; the charcoal is the brand surface.
- **Don't** put an eyebrow or section number above a headline.
- **Don't** uppercase a sentence or let tracking exceed 0.18em outside the brand subtitle.
- **Don't** round photographs or add radius above 0.25rem to controls (the brand circle is the one exception).

## Recorded Decisions

- **Brand fonts load from the Google Fonts CDN** (`index.html` `<link>` + two `preconnect`s), not from local `@font-face`. Every requested weight is used — Playfair Display 600/500 and italic 500, Inter 400/600/700 — so nothing is wasted. Self-hosting remains available as a deployment decision.
- **The brand mark is the shop's own logo** (`assets/favicon/android-chrome-192x192.png`, the skull-and-pompadour line mark) shown at 2.75rem in a circle beside the wordmark. It reads cleanly on the charcoal ground because the art is light line-work on black.
- **The gallery is a third-party Instagram widget, and it is not ours to redesign.** The embed (`#instagram-feed`, `.elfsight-app-9e4078d3-…`, `platform.js`) is managed by the owner in Elfsight. It is a protected region: never replace it with an in-house grid, never restyle its chrome, never remove the script. The CSS provides only outer spacing on `.instagram-feed`.
- **The hero mark is the animated logo, not a photograph.** Its source is `assets/images/lord4l-animated.webm` with an `.mp4` fallback and a `lord4l-still.webp` poster. It autoplays muted, loops, carries `aria-hidden="true"`, and is paused by script under `prefers-reduced-motion`. The webm is re-encoded to a 1280×1500 VP9 with a real **alpha channel** (`yuva420p`, ~1.0 MB) so the mark floats on the charcoal panel instead of sitting in a black box: the black background of the source art is keyed to transparency with a luminance mask. The `.mp4` fallback cannot carry alpha, so its background is baked to the panel Ground (`#111110`) and blends invisibly; the `lord4l-still.webp` poster (1024×1200, transparent) does the same. The video plays at every width — an earlier `media` query that withheld it below 901px was removed, because phones were showing the still instead of the moving mark. A `<source>` that matches but fails never falls through to the next one, and WebKit answers `"probably"` to `canPlayType` for VP9 yet does not actually decode it, so `script.js` watches for the first frame: if it does not arrive (or the media errors) while the current source is still the webm, the video's `src` is swapped to the mp4, which Safari does play. Where the webm works (Chrome, Android) nothing happens — the first frame arrives and the swap is cancelled.
- **The hero states the promise; the page converts once.** The former "Sobre" paragraph was merged into the hero as `.hero__intro` so the page stops saying the same thing twice, and the redundant hero and services CTAs were removed. A single filled "Agendar pelo WhatsApp" remains, in the contact section, with the nav "Agendar" as the quiet second path (both point to `#contato`).
- **`prefers-reduced-motion` is checked in script as well as CSS.** The ledger observer does not initialize under reduced motion, so the pre-hide attribute is never written and the list renders static — the media query alone would still leave the JS half of the choreography armed.
- **The reveal observer has a 5s safety net.** If `IntersectionObserver` never fires for a group (anchor-loaded page, unusual browser, headless virtual time), the script force-sets `data-revealed` so the entrance may be lost but the content never is.
- **The hero promise is its own subtitle.** "Mais que um corte: um ritual de presença." was the opening sentence of `.hero__intro`; it was lifted to a `.hero__subtitle` (Title step, Playfair, Ink) directly under the h1, and the intro now opens at "A Lord 4L Barber é…". The heading speaks, the subtitle states the promise, the deck and intro carry the argument.
- **The nav CTA wears color, not a bar.** "Agendar" was permanently underlined in gold, which read as the current/selected section; the resting underline was removed so only the gold type signals it, and hover/focus brightens it to Gold Soft. This is distinct from `aria-current`, which the script never assigns to the CTA (`.site-nav__cta` is excluded).
- **Contact facts carry line icons.** Phone, clock, pin and camera icons (authored 24-box SVG, one 1.6 stroke, currentColor, Gold Soft) sit beside the caps labels in `.contact__facts dt`; the label column widened from 7rem to 7.5rem to hold icon plus word.
- **The hero mark is nudged left.** The split moved to an even 1fr/1fr so the animated emblem reads as a full half of the spread instead of a panel against the viewport edge; the text column stays wide enough that the Display h1 keeps its two-line break. On wide screens (≥1441px) the emblem is nudged further inside its panel with `left: -12%`, sliding it toward the text so the gap on the left and the margin on the right read balanced; the exposed band at the right edge shows the Ground, so there is no seam.
- **The mark is offset inside its frame.** `object-position` nudges the emblem within the `cover` crop: `60% center` above 900px (mark a touch left of the panel centre) and `40% center` at 900px and below (mark a touch right of the `4/5` plate centre) — about 13px and 8px of travel, enough to seat the mark without clipping the pompadour or the beard tips.
- **The hero has two widths, and the split ends at 900px.** Above 900px the mark is the full viewport-height panel it always was. At 900px and below the hero stacks and centres as one — the text column takes `text-align: center` with each block `margin-inline: auto`, and the mark becomes a `4/5` plate capped at `min(100%, 30rem)` centred beneath it. This replaced a 641–900px layer that kept the split and bled the mark to the right edge: on smaller screens the plate read as off-centre rather than as half a spread, and centring it removes the ambiguity while the width cap keeps the band from becoming a full-width portrait slab. The centre treatment is one rule block at 900px; the section- and footer-level centring stays at 640px, so tablet body copy keeps its left-aligned, two-column reading.
- **The service ledger is two columns and nine lines.** The shop's full price list (corte, barba, corte e barba, progressiva, relaxamento, luzes, sobrancelha, depilação nasal/ouvido, pézinho) is set as one `<ul>` in a `grid-auto-flow: column` grid with `grid-template-rows: repeat(5, auto)` — five rows left, four right — so the page stops being one long vertical list; below 700px it returns to a single column. The dotted leader was removed: with a description under every name it only floated in the middle of the row with nothing to connect, and the row hairline already separates the entries. The graduated services (progressiva, relaxamento, luzes) carry an Ink Soft "a partir de" before the price, and the reveal step dropped from 70ms to 40ms to keep the nine-line cascade near 640ms.
- **Section titles are freed from the 17ch cap.** "Precisão em cada detalhe." and "Acompanhe nosso trabalho." are short enough to hold one line wherever there is room, so `.section--services h2` and `.section--gallery h2` get `max-width: none`; the rules, weights and colors are unchanged.
- **The WhatsApp glyph rides the two booking CTAs.** The nav "Agendar" and the contact "Agendar pelo WhatsApp" each lead with a `currentColor` WhatsApp SVG (`.icon-whatsapp`, 1.15em): gold in the menu, ground on the gold button. It is a drawn glyph, not a Unicode mark.
- **Contact facts reordered.** Instagram now sits above Endereço in the `<dl>`; the values, labels and line icons are otherwise unchanged.
- **The phone layout centres whole, not just the hero.** At 640px and below every section mirrors the hero's centred axis: `.section__heading`, `.section__intro`, the contact intro (its `17ch` h2 included, so "Vamos renovar seu estilo?" lands on the page axis instead of hanging left of centre), the contact status/colophon and the footer all take `text-align: center` with `margin-inline: auto`; the price ledger drops to a single centred column (name, description and price stacked on the middle axis); and the contact facts centre their icon-plus-label rows. Tablet and desktop keep their left-aligned, two-column layouts.
