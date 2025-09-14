# Workshop Booking — UI/UX Enhancement (Prototype)

This branch contains a mobile-first UI/UX enhancement for the original FOSSEE `workshop_booking` site. It is implemented using plain HTML, Bootstrap 5 and a tiny amount of vanilla JavaScript. The goal is to improve readability, navigation, and speed on small screens while keeping the original site structure intact.

## Design principles
**Mobile-first**: I have focused on improving readability by choosing layout and content prioritized for small screens; navigation collapses into a simple navbar and CTAs are prominent.
**Clarity & hierarchy**: Short headings, compact paragraphs, chips and stat cards to surface the most important info.
**Accessible & fast**: Large tap targets, visible focus outlines, native controls (date input), minimal JS and CDN-only CSS for quick load.
**Progressive enhancement**: Works without JavaScript at basic level; JS adds smooth scrolling and optimistic UI interactions.

## Responsiveness & testing
- Designed for narrow widths (320–480px), tablet and desktop breakpoints tested.
- Uses Bootstrap grid and utilities to switch from stacked (mobile) to side-by-side cards (tablet/desktop).
- Tested with keyboard navigation and screen-reader friendly `aria` attributes for dynamic updates.

## Trade-offs
- **Bundle size vs functionality**: Using Bootstrap CDN keeps development quick and small; for stricter performance budgets a custom CSS build would reduce bytes further.
- **Prototype vs backend integration**: The quick booking form is a UI prototype — real booking requires backend endpoints and security (CSRF, validation).
- **Animations**: Kept minimal to avoid jank on low-end devices.

## How to integrate
- Replace the site’s homepage template with `index.html` or adapt component markup into your Django templates.
- Hook the form to the existing backend APIs; keep ARIA live regions for success/error messages.
