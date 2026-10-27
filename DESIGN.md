---
name: Weiterwerk Bildungszentrum
description: Fictional adult education and training centre in the inherited cobalt and warm-paper family
colors:
  ink: "#182b56"
  blue: "#2449d8"
  paper: "#fffaf2"
  sky: "#edf3ff"
  yellow: "#f5df76"
  line: "#d0d7e5"
  muted: "#4b5874"
  white: "#fff"
  blue-hover: "#1935a9"
  funding-panel: "#243a66"
  funding-line: "#526080"
  funding-copy: "#e2e7f2"
  funding-note: "#cbd5eb"
  funding-select-line: "#6e7c9c"
typography:
  display:
    fontFamily: "Bricolage, sans-serif"
    fontSize: "clamp(52px,5.5vw,77px)"
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: "-0.04em"
  headline:
    fontFamily: "Bricolage, sans-serif"
    fontSize: "clamp(36px,3.7vw,53px)"
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: "-0.035em"
  title:
    fontFamily: "Bricolage, sans-serif"
    fontSize: "27px"
    fontWeight: 600
    lineHeight: 1.08
    letterSpacing: "-0.035em"
  body:
    fontFamily: "DM, sans-serif"
    fontSize: "16px"
    fontWeight: 400
    lineHeight: 1.65
  label:
    fontFamily: "DM, sans-serif"
    fontSize: "12px"
    fontWeight: 600
rounded:
  control: "5px"
  surface: "6px"
  mode: "30px"
spacing:
  filter-gap: "7px"
  field-label: "8px"
  module-padding: "22px"
  form-padding: "32px"
  section: "90px"
components:
  button-primary:
    backgroundColor: "{colors.blue}"
    textColor: "{colors.white}"
    rounded: "{rounded.surface}"
    padding: "14px 21px"
  button-primary-hover:
    backgroundColor: "{colors.blue-hover}"
  button-secondary:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.surface}"
    padding: "14px 21px"
  filter-selected:
    backgroundColor: "{colors.ink}"
    textColor: "{colors.white}"
    rounded: "{rounded.control}"
    padding: "10px 15px"
  field:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.control}"
    padding: "10px 13px"
  path-switch:
    backgroundColor: "{colors.white}"
    textColor: "{colors.ink}"
    rounded: "{rounded.surface}"
    padding: "23px 26px"
  funding-guide:
    backgroundColor: "{colors.funding-panel}"
    textColor: "{colors.white}"
    rounded: "{rounded.surface}"
    padding: "30px"
---

# Design System: Weiterwerk Bildungszentrum

## Overview

**Creative North Star: "The next-step switchboard"**

Weiterwerk inherits the portfolio family’s cobalt and navy, warm paper, Bricolage Grotesque display type and DM Sans reading type. This is a code-led implementation with no approved image comp. The north-star phrase below is a descriptive documentation label for the existing family, not a newly approved creative direction.

The adult-training surface pairs approachable, large headlines with a practical course finder. Its defining patterns are a three-path switchboard, ruled expandable programme rows and a dark funding guide. The brand, people, programme content and durations are synthetic; the training photograph is AI-generated, with a visible credit above the photograph. Consultation creates a browser-local preview only.

**Key Characteristics:**
- Cobalt actions and navy text on warm paper.
- Large compact display type with calm reading copy.
- Goal selection, filters and native expandable programme rows.
- Restrained motion, explicit demo disclosures and local font assets.


## Colors

### Primary
Cobalt (`blue`) carries the primary actions, emphasized heading lines, logo mark, step numbers, selection caret and light-surface keyboard focus. Its darker hover sibling is reserved for primary-button hover.

### Secondary
Navy (`ink`) anchors text, selected category filters and the dark funding section. The funding panel, its border and select border use the related blue-grey tokens rather than introducing another visual family.

### Tertiary
Warm yellow (`yellow`) marks the offer strip, funding heading, links, text selection and focus inside the funding section. The source also sets yellow focus for links within consultation copy.

### Neutral
Warm paper (`paper`) is the canvas; white supports controls and compact panels; pale sky (`sky`) groups modules and consultation. Muted text and pale rules separate information without heavy framing. Funding copy and notes use dedicated light blue-grey tokens for reading against navy. Frontmatter values preserve the source’s CSS palette.

## Typography

**Display Font:** local Bricolage Grotesque, registered as `Bricolage`, with sans-serif fallback; 600 and 700 font files are present. Headings use 600.
**Body Font:** local DM Sans, registered as `DM`, with sans-serif fallback; 400 and 600 are present.

Compact, tightly tracked headings give the friendly family its character; body copy remains open and readable. The frontmatter records desktop role defaults, not every contextual override. Programme titles are 28px desktop, 25px below 1100px; form headings are 29px. Hero introduction is 18px desktop and 16px at narrower sizes. Body paragraphs cap at 70ch, with hero introduction at 39ch and consultation copy at 36ch. Small notes range from 10–12px, form labels use the label role, and buttons use 14px/1.4 at weight 600. There is no fixed mathematical type scale.

## Layout

The centered container is at most 1220px wide with 48px side gutters. At 1100px gutters become 32px, and at 600px they become 20px. The desktop hero uses 1.03fr/1fr columns and a 55px gap; its photo is 355px tall, object-fit cover, with the final crop at center 25%. The caption is in normal flow above the photo. The white switchboard overlaps the image by 56px with 36px left and -12px right margins.

Regular sections have 90px vertical padding. Section headings use 1.2fr/1fr columns and a 100px gap. Funding and consultation use two columns with 100px and 110px gaps respectively; the journey uses three equal columns separated by 45px. The FAQ places a narrower heading beside the disclosure list. Programme summaries allocate a flexible title, 175px metadata, 115px mode and 26px icon, separated by 27px; open details use two equal columns.

At 1100px columns tighten, summary metadata narrows and several gaps become 55px. At 850px navigation becomes a menu, the finder stacks category filters above the format selector, regular section padding becomes 65px, and the hero remains two columns. At 600px the hero, headings, funding, consultation, journey, FAQ and programme details stack; category filters become a two-column grid. Programme metadata and mode sit beneath the title, with the plus spanning their right side. Regular section padding becomes 53px; the photo becomes 280px tall and the switchboard overlaps by 35px with a 14px left inset. The last offer-strip phrase is hidden below 850px. Footer items stack below 600px.

## Elevation & Depth

Most surfaces are flat, separated by background bands, thin rules and restrained borders. Only the overlapping switchboard (`0 10px 24px #182b5609`) and mobile navigation (`0 12px 24px #182b5610`) have subtle shadows. Neither programme rows nor the consultation form lift on hover.

## Shapes

Small, gently rounded rectangles define buttons, imagery and panels using the surface radius. Fields and filter buttons use the control radius. Learning-mode tags are pill-like with the mode radius, while journey numbers are circles. Programme and FAQ rows use one-pixel horizontal rules rather than individual card frames. Arrow and plus SVGs use a 1.7 stroke with round joins and caps; open disclosures rotate the plus 45 degrees.

## Components

### Buttons and filters
Primary buttons use cobalt and white with a 54px minimum height and 24px internal gap. Secondary buttons use white, navy and a pale border, with sky hover. Category buttons are at least 44px high; the selected filter uses navy and white and exposes `aria-pressed`. Unselected hover uses sky. The reset action clears category and learning mode, then returns focus to the all-programmes filter.

### Inputs and consultation preview
Native selects and the resizable textarea have a 48px minimum height, pale border and white surface. Labels sit above their fields. The consultation form is white with a pale border and surface corners; its submit fills the width. Submitted values render as text in a sky-coloured preformatted preview that wraps long content. The message is optional with a 2000-character limit. The disabled submit is enabled after JavaScript initializes; without JavaScript, the preview remains disabled and explains the requirement. No request is transmitted.

### Navigation
Desktop navigation is a small inline row with underlined hover and a ruled consultation action. Below 850px it becomes an absolutely positioned paper panel at top 88px. The menu exposes `aria-expanded` and `aria-controls`; links close it, and Escape closes it and restores focus to the menu button. The locale button switches DE/EN text and accessible labels, updates the document language/title/description, persists the language locally and reflects it in the URL.

### Switchboard and programme disclosures
Three ruled goal links select a course category, reset the learning format and navigate to the finder. Category and format filters update the result count in a polite live region and show an explicit empty/reset state. Native programme details retain duration, study pace and mode in the summary. Expanded content separates audience text and consultation action from a sky module panel. The consultation action preselects that programme in the form. FAQ uses the same native disclosure and rotated-plus vocabulary.

### Funding and learner journey
The navy funding band pairs a yellow heading with a blue-grey bordered guide. A native situation selector updates contextual guidance in a polite live region; its disclaimer retains the individual-eligibility and fictional-provider distinction. The journey is an ordered three-step list with cobalt number circles and ruled tops, becoming a vertical sequence on mobile.

### Focus and motion
A 3px cobalt outline with a 5px offset marks buttons, links, selects, textarea and summaries; funding and consultation-copy focus use yellow as specified in source. A skip link becomes visible on focus. Decorative SVGs are hidden from assistive technology and the image alternative explicitly identifies an AI-generated scene. Arrow hover moves 3px only on hover-capable devices. Under no-preference motion, arrow/plus transforms last 180ms, button/filter colour changes last 180ms and detail entry lasts 240ms. Filter updates settle visible results over 230ms using the inherited ease. Reduced motion disables CSS animation/transitions and the JavaScript filter animation. There are no repeated section entrance effects.

## Do's and Don'ts

### Do:
- Do preserve the inherited cobalt/navy, warm-paper and local Bricolage/DM font family.
- Do keep duration, study schedule and learning format visible in collapsed programme rows.
- Do retain visible focus, native disclosure controls, live result announcements and reduced-motion handling.
- Do disclose synthetic programmes and AI imagery, and keep consultation preview wording explicit.

### Don't:
- Don’t replace the course finder with a repeated promotional-card grid.
- Don’t place the AI credit over faces; keep the implemented caption above the photograph.
- Don’t imply real accreditation, funding entitlement, bookable courses or transmitted enquiries.
- Don’t add repeated entrance effects to the section sequence.
