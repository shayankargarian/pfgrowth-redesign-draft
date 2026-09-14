# Design direction: PF Growth redesign prototype

One-page mood for a premium growth-finance web experience. Distinctive, not a generic SaaS template.

## Mood
Calm authority meets founder urgency. Think private credit desk crossed with a well-edited tech journal: dense enough to feel serious, airy enough to read on a phone at 390px. Warm copper light on deep ink. No neon gradients, no purple blobs, no stock “handshake on glass table.”

## Colour
| Token | Hex | Use |
| --- | --- | --- |
| Ink | `#0B1220` | Primary background, text on light |
| Slate | `#1A2436` | Cards, elevated surfaces |
| Mist | `#E8EDF5` | Light section backgrounds |
| Paper | `#F7F5F1` | Warm off-white (paper, not sterile grey) |
| Copper | `#C47A3A` | Primary accent, links, key CTAs |
| Copper deep | `#9A5A28` | Hover / pressed |
| Fog | `#8B95A8` | Secondary text (must still pass AA on Ink) |
| Signal | `#2F6F5E` | Success / positive fit cues |

Contrast intent: body text on Paper or Mist at least 7:1; Copper buttons use dark text or ensure AA on Copper-on-Ink outlines. Never grey-on-grey for critical copy.

## Type
- **Display:** Fraunces (soft serif with optical sizing). Headlines only. Slightly condensed tracking on large sizes.
- **UI / body:** Source Sans 3 (or system-ui fallback). High x-height for mobile.
- Scale (mobile base 16px): display 2.25-2.75rem; section 1.5rem; body 1rem / 1.6; meta 0.8125rem.
- Hierarchy by size and weight first; colour second. Avoid all-caps walls.

## Layout and hierarchy
- Mobile-first: single column, 20-24px side padding, generous section gaps (64-96px).
- Sticky compact header with logo wordmark + “Talk to us” pill.
- Hero: one claim, one subclaim, one primary CTA, one secondary text link.
- “Fit strip” early: three scannable numbers (ticket, revenue, structures).
- Cards with thin hairline borders on Slate/Paper, not heavy drop shadows.
- Desktop: widen measure, optional two-column for criteria; keep phone composition as source of truth.

## Motion (restrained)
- Prefer opacity/transform under 200ms on interactive states only.
- No autoplaying carousels; no counter animations that fight reduced-motion.
- Honour `prefers-reduced-motion: reduce` (disable non-essential transitions).
- Focus rings always visible (2px Copper offset), never removed.

## Accessibility (WCAG-minded)
- Semantic landmarks: header, nav, main, footer.
- Skip link to main content.
- Tap targets ≥ 44px.
- Form labels visible (not placeholder-only).
- Error text in prose + aria.
- Decorative SVG only; no hotlinked client photography required.
- Australian English spelling in UI copy.

## What we are not
- Not a clone of the current Elementor skin.
- Not another indigo-gradient fintech landing page.
- Not a logo zoo on the homepage.

## Prototype implementation notes
Static HTML/CSS/JS. Shared `css/styles.css` and `js/main.js`. SVG marks for regions and icons. Draft watermark in footer: “Redesign prototype for review. Not the live pfgrowth.com site.”
