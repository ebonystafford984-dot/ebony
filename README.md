# Ebony's Portfolio

This site has Home, Projects / Work, and About / Contact pages, with a shared responsive stylesheet.

## Milestone 2 Accessibility and Visual Design

### Accessibility fixes

- Added a keyboard-accessible skip link to each page so visitors can bypass repeated navigation and move directly to main content.
- Changed keyboard focus outlines to high-contrast navy on light surfaces and white on the navy navigation header.
- Added visible labels, required-field instructions, and autocomplete hints to every contact form field.
- Grouped the contact fields in a fieldset with a legend so assistive technology announces their shared purpose.
- Added inline validation messages, `aria-invalid` states, and a live status message so form errors are announced and easy to locate.
- Kept the form's success message honest by explaining that message delivery is not connected and no message is sent.

### WAVE results

WAVE was run on the published Home, Projects / Work, and About / Contact pages before these changes; each page showed 0 errors, 0 contrast errors, and 0 alerts. Run WAVE again on the updated published pages after this change set is uploaded.

### WCAG AA contrast

Text and focus colors were checked with the [WebAIM Contrast Checker](https://webaim.org/resources/contrastchecker/); every listed text pairing passes WCAG AA for normal text.

| Foreground | Background | Ratio | Result |
| --- | --- | ---: | --- |
| `#243342` body text | `#FBF4E8` cream | 11.8:1 | Pass |
| `#FBF4E8` header text | `#17324D` navy | 12.0:1 | Pass |
| `#FFFFFF` navigation and button text | `#17324D` navy | 13.1:1 | Pass |
| `#17324D` active and hover text | `#D7A43B` gold | 5.78:1 | Pass |
| `#80500E` section headings | `#FBF4E8` cream | 6.25:1 | Pass |
| `#754500` links | `#FBF4E8` cream | 7.36:1 | Pass |
| `#9B1C1C` validation errors | `#FBF4E8` cream | 7.45:1 | Pass |
| `#526477` form borders | `#FFFFFF` white | 6.09:1 | Pass (UI component) |
| `#17324D` keyboard focus outline | `#FBF4E8` cream | 12.0:1 | Pass |

### Intentional visual design

- **Proximity:** Project cards keep each title, description, and link together, while spacing separates each card from its neighbors.
- **Similarity:** Repeated navy headings, gold accents, rounded cards, and shared typography create a consistent visual system across the pages.

### Contact form behavior

The About / Contact form validates name, email address, and message fields in the browser. It demonstrates accessible error feedback, but does not send or store messages because no delivery service is configured.
