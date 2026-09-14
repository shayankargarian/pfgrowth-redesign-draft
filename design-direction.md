# Design direction: PF Growth redesign prototype

Modern growth-finance product site. Clarity first. Product-sharp, not heritage wealth.

## Mood
Forward tech with Apple-like restraint: large type, generous whitespace, calm surfaces, one clear hero claim. Still sharper modern fintech for growth debt founders (confident numbers, geometric sans, high contrast). Not PE brochure. Not family-office parchment. Not private-credit desk.

Think product marketing clarity over finance ornament. Fewer cards, more breathing room. Accent used sparingly as signal, not chrome everywhere.

## Colour
| Token | Hex | Use |
| --- | --- | --- |
| Void | `#0A0A0B` | Primary dark background |
| Panel | `#141416` | Elevated dark surfaces |
| Line | `rgba(255,255,255,0.08)` | Hairline borders on dark |
| Snow | `#F5F5F7` | Light sections (cool Apple grey-white) |
| Ink | `#1D1D1F` | Text on light |
| Accent | `#2997FF` | Primary CTA / links (electric blue, restrained) |
| Accent deep | `#147CE5` | Hover |
| Mute | `#86868B` | Secondary text |
| Signal | `#30D158` | Success / positive fit (sparingly) |

Contrast: body on Snow or Void ≥ 7:1. Accent buttons: white text on Accent, or dark text only if contrast holds. No warm copper. No parchment. No neon lime wash.

## Type
- **Display:** Inter (tight, product UI) or SF-adjacent geometric sans via Inter + Space Grotesk for wordmark only.
- Prefer one strong family: **Inter** for UI and display (Apple-like clarity). Optional Space Grotesk for logo only.
- Scale: hero 2.75-4.25rem; section 1.75-2.25rem; body 1.0625rem / 1.5; meta 0.8125rem.
- Tracking tight on large display (−0.04em). Hierarchy by size/weight; colour second.

## Layout and hierarchy
- Mobile-first. Side padding 20-24px. Section gaps 80-120px (more air).
- Sticky compact header + “Talk to us” pill.
- Hero: one claim, short lede, primary CTA, secondary text link. Fit strip immediately below.
- Prefer product-hero blocks and short proof rows over dense six-card grids.
- Cards: thin hairlines, almost no shadow, calm hover (border only).
- Phone composition is source of truth.

## Motion
- ≤160ms opacity/transform on interactive states only.
- No glow stacks, no parallax, no auto carousels.
- Honour `prefers-reduced-motion: reduce`.
- Focus rings: 2px Accent offset, always visible.

## Accessibility
- Skip link, landmarks, ≥44px targets, visible labels.
- Australian English. No em dashes.
- DRAFT badge + noindex on every page.

## What we are not
- Not institutional PE / family office / private-credit desk.
- Not Fraunces + copper + warm paper.
- Not loud neon fintech chrome.
- Not Elementor clone or logo zoo.

## Prototype notes
Static HTML/CSS/JS. HubSpot unwired. Footer draft watermark retained.
