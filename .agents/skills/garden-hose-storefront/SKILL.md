---
name: garden-hose-storefront
description: Build and refine the bruno-angular gardening-hose storefront, including its Angular pages, navigation, responsive layout, and product discovery. Use for storefront UI work in this repository.
---

# Garden hose storefront

Use this skill when implementing the customer-facing storefront in this repository.

## Project context

- The app is Angular 22 with standalone components and Tailwind CSS 4 through PostCSS.
- The root component is `src/app/app.ts`; its template and styles are `src/app/app.html` and `src/app/app.css`.
- Global Tailwind setup lives in `.postcssrc.json` and `src/styles.css`. Use utility classes in Angular templates and keep component CSS for styles that are awkward or unclear as utilities.
- Extend the existing app structure and visual language. Split out components when a page or repeated section becomes easier to understand that way.

## Storefront behavior

- Make hose length, inside diameter, material, connection type, and intended use easy to compare when those facts are available.
- Support a straightforward path from browsing to a product detail page and adding a selected product or variant to the cart.
- Make filters and sorting understandable, reversible, and usable on narrow screens.
- Keep product names, prices, selected variants, and availability consistent wherever they appear.
- Do not invent product specifications, compatibility claims, pressure ratings, warranty terms, or delivery promises. Use supplied catalog data or clearly mark missing information for the project owner.

## Interface quality

- Use semantic HTML, visible focus states, labeled controls, useful empty states, and readable contrast.
- Ensure the main browse and purchase flow works with a keyboard and on mobile-sized screens.
- Keep calls to action specific, such as “Add to cart” or “Choose length.” Avoid fake urgency, fabricated review counts, or unsupported savings claims.
- Keep the page focused on selecting the right hose and compatible fittings; avoid unrelated garden products unless the user asks to expand the catalog.

