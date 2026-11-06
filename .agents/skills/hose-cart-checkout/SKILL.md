---
name: hose-cart-checkout
description: Implement and refine cart and checkout flows for the gardening-hose store in bruno-angular. Use for cart state, quantity controls, totals, shipping display, and checkout handoff.
---

# Cart and checkout

Use this skill for cart behavior and the steps between selecting a hose and placing an order.

## Cart behavior

- Store the selected product variant with each cart line so the customer can review hose length, diameter, color, and fittings before checkout.
- Support quantity changes and item removal, and clearly show when the cart is empty.
- Calculate displayed line totals and subtotals from numeric amounts. Format them with the product's explicit currency; do not mix currencies in one cart.
- If a backend exists, treat its price, availability, tax, discount, and shipping calculations as authoritative. Client-side totals are for display only.
- Do not promise shipping dates, free shipping, tax amounts, or stock availability unless the data source supports them.

## Checkout boundaries

- Follow the payment provider and backend already chosen by the project. If neither is configured, build only the requested interface or a clearly labeled demo flow; do not imply that an order or charge was placed.
- Never collect or store raw card numbers, security codes, or payment credentials in Angular state, local storage, logs, or source files. Use the provider's approved hosted checkout or secure client integration when one is selected.
- Keep customer information limited to fields required by the chosen checkout. Do not persist addresses or contact details in browser storage unless the user explicitly requests that behavior.
- Show a clear order review before the final purchase action, including the selected variants, quantities, item totals, and any shipping or tax values supplied by the backend.

## Usability

- Make quantity and remove controls keyboard accessible and give them labels that identify the affected product.
- Preserve cart contents while users move between storefront and cart, using the persistence approach already present in the app.
- Provide clear loading, validation, and recoverable error states without discarding the cart.

