# Accessibility Checklist

Quick reference from a11y review. Use for new components and pages.

## Semantic HTML
- Use one `h1` per page.
- Use landmarks: `header`, `nav`, `main`, `footer`.
- Use native buttons/links instead of `div` with click handler when possible.

## Keyboard
- All interactive elements focusable and operable via keyboard.
- Visible focus indicator: `:focus-visible`.
- No keyboard traps.
- Skip link to main content.

## Alt Text & Media
- Decorative images: empty `alt`.
- Informative images: descriptive `alt`.
- Video/audio transcripts or captions.

## ARIA
- Prefer native HTML over ARIA.
- Use `aria-label` only when no visible label.
- `aria-live` for dynamic updates.

## Color & Contrast
- Text contrast >= 4.5:1 (large text >= 3:1).
- Don't rely on color alone to convey state.
- Test with forced colors/high contrast mode.

## Forms
- Label every input.
- Associate label with `for`/`id`.
- Error messages linked with `aria-describedby`.
- Instructions not just placeholder.

## Testing
- Keyboard only.
- Screen reader: NVDA/VoiceOver.
- Zoom 200%, 400%.
- Lighthouse/axe scan.

Remember: accessibility is a requirement, not a feature.