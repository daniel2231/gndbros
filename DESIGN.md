---
name: GNDBros Landing
description: A signal-red, editorial landing page for a 36-member Korean airsoft crew built around "No tactic, Best tactic."
colors:
  black: "#0a0a0a"
  paper: "#f2f1ee"
  muted: "#a8a8a4"
  signal-red: "#FB434B"
  deep-red: "#FB434B"
  rule: "rgba(242, 241, 238, 0.17)"
  image-surface: "#181818"
  red-hover: "#ff685e"
typography:
  display:
    fontFamily: "Bebas Neue, Arial Narrow, sans-serif"
    fontSize: "clamp(4.8rem, 8.2vw, 8.5rem)"
    fontWeight: 400
    lineHeight: 0.82
    letterSpacing: "-0.015em"
  headline:
    fontFamily: "Bebas Neue, Arial Narrow, sans-serif"
    fontSize: "clamp(4rem, 9vw, 9.2rem)"
    fontWeight: 400
    lineHeight: 0.82
    letterSpacing: "-0.01em"
  title:
    fontFamily: "Bebas Neue, Arial Narrow, sans-serif"
    fontSize: "clamp(3.2rem, 6vw, 6rem)"
    fontWeight: 400
    lineHeight: 0.82
  body:
    fontFamily: "Sora, Arial, sans-serif"
    fontSize: "0.95rem"
    fontWeight: 400
    lineHeight: 1.7
  label:
    fontFamily: "Sora, Arial, sans-serif"
    fontSize: "0.68rem"
    fontWeight: 700
    lineHeight: 1
    letterSpacing: "0.14em"
  korean:
    fontFamily: "IBM Plex Sans KR, Noto Sans KR, sans-serif"
    fontWeights: "400, 500, 600, 700"
    lineHeight: "1.75 body / 0.98–1.05 display"
rounded:
  none: "0"
  circle: "50%"
spacing:
  page-gutter: "clamp(1.2rem, 3vw, 3.4rem)"
  section-y: "clamp(5rem, 11vw, 10rem)"
  nav-y: "1.25rem"
  button-padding: "0.75rem 1rem"
  compact-gap: "0.65rem"
components:
  button-primary:
    backgroundColor: "{colors.signal-red}"
    textColor: "{colors.black}"
    rounded: "{rounded.none}"
    padding: "{spacing.button-padding}"
    height: "2.9rem"
    typography: "{typography.label}"
  button-secondary:
    backgroundColor: "{colors.black}"
    textColor: "{colors.paper}"
    rounded: "{rounded.none}"
    padding: "{spacing.button-padding}"
    height: "2.9rem"
    typography: "{typography.label}"
  nav-cta:
    backgroundColor: "{colors.signal-red}"
    textColor: "{colors.black}"
    rounded: "{rounded.none}"
    padding: "0.65rem 0.8rem"
    typography: "{typography.label}"
  field-card:
    backgroundColor: "{colors.paper}"
    textColor: "{colors.black}"
    rounded: "{rounded.none}"
    padding: "1.2rem 1.1rem 1.4rem 0"
---

# Design System: GNDBros Landing

## Overview

**Creative North Star: "The Signal in the Fog"**

GNDBros is shipped as an editorial campaign page for a crew you stumble into at dusk: near-black field notes, a signal-red accent, condensed campaign lettering, and one human image carrying the atmosphere. The page is deliberately personality-led rather than club-like. Its voice is young, expressive, lightly irreverent, and comfortable with a little visual noise.

The system uses hard edges, oversized type, sparse copy, and movement as identity. Black and paper sections alternate like a zine or field report; red appears as the signal that marks action, emphasis, and invitation. The composition stays generous and cinematic on large screens, then collapses into a single readable column on narrow screens.

**Key Characteristics:**

- Signal-red emphasis against a near-black / warm-paper field.
- Bebas Neue display type paired with Sora utility copy.
- Square controls, 1px rules, a clipped hero seam, and one circular motion stamp.
- Human, direct copy grounded in the team's Notion introduction and FAQ.
- Motion that is expressive by default and explicitly collapses under reduced-motion preferences.

## Colors

The palette is intentionally tight: near-black for the world, warm paper for the field section, muted gray for secondary information, and signal red for calls to action and emphasis.

### Primary

- **Signal Red**: The high-energy action color used for the hero emphasis, primary buttons, section accents, animated rail, active-looking arrows, and the invitation close.

### Secondary

- **Deep Red**: The darker red used where the paper section needs the same signal with stronger contrast.

### Neutral

- **Near Black**: The default page field, dark hero copy panel, dark button surface, and footer text contrast.
- **Warm Paper**: The light field section, primary light text, and image-stamp lettering.
- **Dust Gray**: Supporting copy, metadata, navigation links, and the scroll cue.
- **Rule White**: A translucent paper rule used for dark-section borders and dividers.
- **Image Surface**: The fallback dark gray behind the hero photograph.
- **Soft Red**: The brighter hover state on the fixed navigation CTA.

### Named Rules

**The Signal Rule.** Red marks movement, emphasis, or an invitation; it is not a general-purpose fill for every element.

## Typography

**Display Font:** Bebas Neue (with Arial Narrow, sans-serif fallback) for English
**Body Font:** Sora (with Arial, sans-serif fallback) for English
**Korean Font:** IBM Plex Sans KR (with Noto Sans KR, sans-serif fallback) for Korean copy and display roles
**Label/Mono Font:** Sora is also used for all labels; there is no separate mono face.

**Character:** Bebas Neue supplies the compressed, poster-like voice and lets headlines occupy the page as graphic shapes. Sora keeps supporting copy, metadata, navigation, and actions contemporary and legible. When the language toggle is set to Korean, IBM Plex Sans KR replaces the English faces for both display and body roles. Korean headings use a heavier weight with relaxed leading and `word-break: keep-all` so the block retains the same assertive poster character without collapsing the vertical rhythm.

### Hierarchy

- **Display** (400, `clamp(4.8rem, 8.2vw, 8.5rem)`, `0.82`): Hero statement, uppercase, with the key phrase colored by the signal accent.
- **Headline** (400, `clamp(4rem, 9vw, 9.2rem)`, `0.82`): Section titles such as “Different build.” and “Our rhythm.”
- **Title** (400, `clamp(3.2rem, 6vw, 6rem)`, `0.82`): Field-card headings; the invitation uses a larger `clamp(5rem, 12vw, 13rem)` display treatment.
- **Body** (400, `0.95rem`, `1.7` where explicitly set): Introductory and explanatory copy, generally constrained to roughly 24–46ch.
- **Label** (700, `0.68rem`, `0.14em`, uppercase): Navigation, section indices, kicker text, card metadata, footer text, and button labels. Some labels tighten or widen tracking between `0.08em` and `0.2em` according to role.

### Named Rules

**The Two-Voice Rule.** Use the condensed display face for the statement and the geometric body face for the explanation; do not let utility copy compete with the headline voice.

## Layout

The page is a vertical campaign sequence: fixed navigation, full-viewport split hero, moving statement rail, dark team introduction, open differentiation list, light newcomer guidance, a two-column FAQ, red Instagram invitation, and a compact footer.

The desktop hero is a two-column grid with `minmax(340px, .82fr)` for the copy panel and `minmax(0, 1.18fr)` for the image. Both hero columns are at least `100svh` tall. The copy panel uses the page gutter (`clamp(1.2rem, 3vw, 3.4rem)`) and a clipped black wedge that reaches into the image. The rest of the page uses the same gutter and vertical section padding of `clamp(5rem, 11vw, 10rem)`.

Content density alternates between sparse editorial copy and full-width structural rows. The intro uses a `.8fr / 1.2fr` grid with a fluid gap up to `12rem`; the crew list uses four columns for index, role, note, and arrow; the field uses three equal cards with 1px dividers. The fixed navigation compresses from `1.25rem` vertical padding to `.8rem` after `scrollY > 24`.

At `max-width: 780px`, the hero becomes a column, the wedge disappears, and the image follows the copy at `60svh` minimum height. Hero details stack, the scroll cue disappears, intro content becomes one column, crew notes hide, field cards stack, the invitation becomes one column, and the footer stacks from row to column. Navigation links hide while the CTA remains. The image focal point shifts from `61%` to `62%` horizontally.

The shipped hero image is `assets/gndbros-field.png` (PNG, 1983 × 793). It fills its frame with `object-fit: cover`, uses `object-position: 61% center` on desktop and `62% center` on mobile, and is treated with `saturate(.82)` and `contrast(1.08)`.

## Elevation & Depth

This is a flat, graphic system rather than a shadow-based one. There are no box shadows. Depth comes from alternating tonal fields, 1px rules, the fixed grain overlay, a low-opacity image gradient, the translucent blurred scrolled navigation, the clipped hero seam, and motion responses such as lift, translate, scale, and the rotating stamp.

### Named Rules

**The Flat-By-Default Rule.** Keep surfaces crisp and unshadowed; use tonal contrast, rules, clipping, and state motion to separate layers.

## Shapes

Controls, cards, sections, and navigation surfaces are square (`0` radius). The one circular silhouette is the `5.8rem` image stamp with a `50%` radius. Borders are generally 1px. The hero copy panel has a polygonal clipped wedge rather than a rounded seam, and the page keeps the field-card and crew-row geometry open to the viewport rather than enclosing it in cards.

## Components

### Buttons

- **Character:** Compact, uppercase action markers with enough border and tracking to read as editorial labels.
- **Shape:** Square, `0` radius, inline-flex, `2.9rem` minimum height, `.75rem 1rem` padding, `.65rem` icon gap.
- **Primary:** Signal-red fill with near-black text; used for “Meet the crew” and the fixed “Join the noise” CTA.
- **Secondary:** Transparent / dark field with warm-paper text and a 1px warm-paper border; the “Our rhythm” action turns red on hover or focus.
- **Hover / Focus:** Buttons translate upward `3px`; secondary buttons shift border and text to red; the nav CTA uses the brighter red hover fill and a `2px` lift. All retain the browser’s native focus outline because the shipped CSS does not suppress it.

### Cards / Containers

- **Field cards:** Three open columns on warm paper explain equipment rental, free-form clothing, and optional game participation. Each uses a 1px divider and square geometry; on mobile they become stacked rows.
- **Crew rows:** Four full-width informational rows cover activities, member backgrounds, equipment knowledge, and beginner friendliness. Each pairs an oversized label with supporting detail and a Lucide icon.
- **FAQ:** Ten native `details` elements form a compact two-column disclosure grid on desktop and a single column on mobile.

### Navigation

- **Desktop:** Fixed, full-width, transparent at rest, with the GNDBROS mark at left and two anchor links plus a red CTA at right. The nav is `z-index: 10`.
- **Scrolled:** At more than 24px scroll, the nav compresses vertically, gains an `rgba(10,10,10,.88)` background, the shared translucent rule, and `backdrop-filter: blur(12px)`.
- **Mobile:** The “The crew” and “The field” links hide below `780px`; the brand and CTA remain.
- **Accessibility:** The header has a labeled primary nav, the brand has an explicit home label, and decorative SVGs are `aria-hidden`. Link targets are in-page anchors except for the mail and Instagram actions.

### Marquee

- **Style:** Full-width signal-red rail with dark text, 1px dark-section rules, and the repeated team line “No tactic. Best tactic. 36 brothers.”
- **Motion:** The track is `width: max-content` and translates left over `22s` linearly and infinitely. The rail is labeled “GNDBros is not a club” for assistive technology, although the repeated visual items remain in the DOM.

### Hero Image / Stamp

- **Image:** One human team image occupies the right side of the desktop hero and the lower half of the mobile hero. The image has an accessible alt description; the dark gradient is decorative.
- **Stamp:** A 1px paper circle at the lower-right of the image, set to `5.8rem` square, with uppercase text and an `18s` linear infinite rotation. It is `aria-hidden` because it is atmospheric rather than content-bearing.

### Motion and Accessibility

- Scroll-linked reveal items begin at `opacity: 0` and `translateY(22px)`, then enter over `700ms` with `cubic-bezier(.2,.75,.2,1)` when an `IntersectionObserver` sees `14%` of the element. Each item is unobserved after becoming visible.
- Hero children rise in sequence over `850ms` with delays of `90ms`, `180ms`, and `270ms`. The image scales to `1.025` on hover. Smooth scrolling is enabled globally.
- Under `prefers-reduced-motion: reduce`, animations and transitions collapse to `.01ms`, smooth scrolling is disabled, reveal content is immediately visible, and the page remains usable without motion.

## Do's and Don'ts

### Do:

- **Do** preserve the near-black, warm-paper, and signal-red relationship as the primary visual language.
- **Do** keep display headlines condensed, uppercase, and spatially dominant while body copy remains in Sora.
- **Do** use square geometry, 1px rules, open rows, and restrained grain rather than rounded card stacks or drop shadows.
- **Do** keep calls to action anchored to the shipped destinations: `#crew`, `#field`, `#faq`, `#join`, and `https://www.instagram.com/gndbros_airsoft/`.
- **Do** preserve the image asset path `assets/gndbros-field.png` unless the replacement keeps the same human, misty-field role and receives equivalent alt text.
- **Do** honor reduced-motion preferences and retain visible keyboard focus behavior.

### Don't:

- **Don't** turn the crew into a formal roster, military brochure, or generic tactical club surface.
- **Don't** introduce rounded buttons, card shadows, or a new pastel palette that competes with the signal-red system.
- **Don't** add team facts beyond the connected Notion source or invent individual roster and event details.
- **Don't** remove the semantic landmarks, image alt text, labeled navigation, decorative SVG hiding, or native focus outline behavior.
- **Don't** make motion a prerequisite for comprehension; the static state must still communicate the same hierarchy.
