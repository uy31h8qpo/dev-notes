# Accessibility Checklist

Quick reference for reviewing components.

## Semantic HTML
- Use native elements (`button`, `a`, `input`) where possible.
- Keep heading levels in order (`h1` -> `h2` -> `h3`).

## Keyboard
- All interactive elements reachable with Tab.
- Visible focus indicator, never `outline: none` without replacement.
- No keyboard traps; Escape closes dialogs/menus.

## ARIA
- Only use ARIA when native semantics aren't enough.
- `aria-label` for icon-only buttons.
- `aria-live` for dynamic updates, with polite by default.

## Forms
- Labels associated with inputs via `for`/`id`.
- Errors linked with `aria-describedby`.
- Required fields indicated beyond color.

## Images & Media
- Alt text for meaningful images; empty `alt` for decorative.
- Captions/transcripts for audio and video.

## Color & Motion
- Contrast ratio at least 4.5:1 for normal text.
- Don't rely on color alone to convey state.
- Respect `prefers-reduced-motion`.

## Testing
- Check with keyboard only.
- Run axe DevTools or Lighthouse.
- Test with a screen reader (VoiceOver/NVDA).
