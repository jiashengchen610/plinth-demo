---
version: "alpha"
name: restaurant
description: "A lively, welcoming Chinese restaurant brand: festive like a New Year table, rooted in real Chinese craft rather than takeaway clichés."
colors:
  background: "#fdfcf7"
  foreground: "#1e1311"
  card: "#ffffff"
  card-foreground: "#1e1311"
  popover: "#ffffff"
  popover-foreground: "#1e1311"
  primary: "#cb3904"
  primary-foreground: "#fdfcf7"
  secondary: "#d0f1e1"
  secondary-foreground: "#043726"
  muted: "#f4ede8"
  muted-foreground: "#685a55"
  accent: "#fbe6b3"
  accent-foreground: "#43260a"
  destructive: "#9b0f1b"
  border: "#e6dcd4"
  input: "#dfd5ce"
  ring: "#db6241"
  success: "#0a7e3a"
  success-foreground: "#fafafa"
  warning: "#b97500"
  warning-foreground: "#1f1306"
  info: "#116bb5"
  info-foreground: "#fafafa"
typography:
  display:
    fontFamily: Geist
    fontSize: 2rem
    fontWeight: 600
    lineHeight: 1.15
    letterSpacing: -0.02em
  body:
    fontFamily: Geist
    fontSize: 0.875rem
    fontWeight: 400
    lineHeight: 1.5
rounded:
  md: 0.875rem
---

# restaurant

## Overview

Fun, authentic and generous. The recognisable thing is the orange-red (vermilion lacquer) against paper white, lifted by touches of yellow gold, the way red and gold meet on lanterns and red envelopes. Green (jade) brings calm to quieter areas so the red stays special.

## Colors

- primary (orange-red, vermilion lacquer): the one main action per view, such as "Book a table" or "Order now". Also for small festive details like a price tag or a seal-style mark.
- accent (yellow gold): highlights and hover states, chef's specials, festive badges. Use it on small areas, never as a page background.
- secondary (green, jade): calm supporting surfaces such as dietary info, opening hours and secondary buttons.
- background (paper white) and foreground (warm ink): the base of every page. Dark mode uses deep ink surfaces with brighter orange-red and gold.
- muted / muted-foreground: menu descriptions, footnotes and supporting text.
- destructive (deep red): errors and irreversible actions only, such as cancelling a booking. It is darker than primary; always pair it with clear text or an icon so it is never mistaken for the main action.
- success, warning, info: status only (booking confirmed, limited availability, opening-hours notice), never for actions.

## Typography

- ZCOOL KuaiLe for display: page titles, section titles and dish category headings. Playful and hand-made, and it supports Chinese characters.
- Noto Sans SC for everything else: menus, prices, forms and body text. Clear at small sizes, with matching Chinese glyphs so bilingual dish names sit together.
- Show dish names in Chinese and English when known; Chinese first or above, English below in the body style.

## Layout

- Marketing site: generous hero with real food photography, then menu, story, location and booking.
- Use the spacing scale only (multiples of 4px through Tailwind utilities).
- One primary action per view ("Book a table" or "Order now"); secondary actions use outline or ghost buttons.
- Keep the booking or order action reachable on every page; on phones, a sticky bottom bar with 44px touch targets.
- Menus are scannable: dish name, short description and price on one row on desktop, stacked on phones.
- Body text stays under 75 characters per line.

## Shapes

- Friendly rounded corners (base radius 0.875rem) on cards and buttons, like lacquer trays and dumpling edges.
- Use smaller radius on inputs and tags, larger on hero images, so not every surface looks the same.
- Shadows are soft and used for lifted things only (menus, dialogs), not on every card.

## Components

- Build new UI from existing components first; create a new component only when none fits.
- Every component has a spec (<name>.spec.md) and one story per variant and state.

## Do's and Don'ts

- Do use semantic tokens (bg-primary, text-muted-foreground), never raw values.
- Do keep text contrast at 4.5:1 or more in every brand and mode.
- Don't give every surface the same radius and shadow; vary them by hierarchy.
- Don't put an all-caps label above every heading.
- Don't number sections (01, 02, 03) unless the content is a real sequence.
- Don't accent a single word in a headline with a different color or weight.
- Do use real Chinese characters for dish names and section labels, checked by a fluent reader.
- Do keep orange-red to one main button per view.
- Don't use "chopstick" or "wonton" novelty fonts that imitate brush strokes with Latin letters.
- Don't fill large areas with orange-red and yellow gold together; one leads, the other accents.
- Don't use dragons, pandas or lanterns as generic decoration; use imagery of the real food and room.
- Don't use destructive red for prices, specials or promotions.
