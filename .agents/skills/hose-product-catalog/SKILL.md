---
name: hose-product-catalog
description: Model, edit, and present gardening-hose products and variants for the bruno-angular store. Use when working on catalog data, product attributes, filters, or specification copy.
---

# Hose product catalog

Use this skill for catalog schemas, product data, product cards, detail pages, and hose-specific filters.

## Product data

- Inspect existing types and data before adding a schema. Keep product and variant concepts aligned with the current code.
- Where the source provides them, represent product identity and purchase facts separately: SKU, brand, product name, category, variant, price, currency, and availability.
- Useful hose attributes include length, inside diameter, material, color, fitting type, included accessories, and intended use. Store units explicitly or normalize values to a documented unit before comparing them.
- Keep variant-specific details such as length, color, or included fittings attached to the variant the customer selects.
- Preserve source attribution for product claims when the project has it.

## Accuracy

- Never infer pressure ratings, drinking-water safety, UV resistance, kink resistance, temperature limits, fitting compatibility, warranty, or country of origin from a product name or image.
- Do not turn missing specifications into zero, “standard,” or a positive claim. Represent unknown data as absent and omit the corresponding filter or badge.
- Keep price amounts numeric and currencies explicit. Avoid parsing formatted price strings for calculations.
- If catalog information is incomplete or contradictory, identify the fields that need confirmation instead of silently choosing values.

## Discovery

- Build filters from available, normalized catalog values rather than hard-coded assumptions.
- Make comparisons useful to a buyer: compare equivalent units and the same attribute across products.
- Keep search, category, filters, sort order, selected variants, and result counts coherent when the catalog changes.

