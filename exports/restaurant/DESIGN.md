---
version: "alpha"
name: restaurant
description: "A neutral starting brand. Replace this with the brand's own description."
colors:
  background: "#ffffff"
  foreground: "#0a0a0a"
  card: "#ffffff"
  card-foreground: "#0a0a0a"
  popover: "#ffffff"
  popover-foreground: "#0a0a0a"
  primary: "#171717"
  primary-foreground: "#fafafa"
  secondary: "#f5f5f5"
  secondary-foreground: "#171717"
  muted: "#f5f5f5"
  muted-foreground: "#696969"
  accent: "#f5f5f5"
  accent-foreground: "#171717"
  destructive: "#bc0013"
  border: "#e5e5e5"
  input: "#e5e5e5"
  ring: "#a1a1a1"
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
  md: 0.625rem
---

# restaurant

## Overview

Calm, neutral and legible. Color is reserved for actions and status.

## Colors

- primary: the main action color. Use it for one action per view.
- destructive: irreversible actions and errors only.
- muted / muted-foreground: secondary surfaces and supporting text.
- success, warning, info: status only (badges, alerts, inline messages), never for actions.

## Typography

Geist for everything. Display style for page titles, body style for content.

## Layout

- Use the spacing scale only (multiples of 4px through Tailwind utilities).
- One primary action per view; secondary actions use outline or ghost buttons.
- Body text stays under 75 characters per line.

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
