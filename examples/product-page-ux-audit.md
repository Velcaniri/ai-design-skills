# Example: Product Page UX Audit

## Scenario

A reusable water bottle page shows a product photo, a 750 ml variant, a star rating, price, quantity selector, and “Add to cart.”

## Findings

### [High] The selected volume is easy to miss

- **Where:** Variant selector below the product name.
- **Problem:** The 750 ml option is selected with a pale outline that blends into the page.
- **User impact:** Shoppers may add a different size than intended.
- **Recommendation:** Add a clear selected state with sufficient contrast and an accessible selected label.

### [Medium] Quantity is separated from the purchase action

- **Where:** Quantity selector and Add to cart button.
- **Problem:** The selector appears several sections above the button.
- **User impact:** Visitors may lose track of the quantity they are adding.
- **Recommendation:** Keep quantity next to the button and show the selected amount and price clearly.

### [Needs verification] Rating behavior is unknown

The screenshot shows a rating and review count, but does not show whether selecting it takes the visitor to reviews. Inspect the live interaction before reporting a defect.

## Fix order

Clarify the selected product size first, then group quantity with the purchase action. Verify review navigation separately. This example reports only what is visible and labels unknown behavior rather than guessing.