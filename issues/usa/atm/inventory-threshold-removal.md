# Inventory availability reduced by an item threshold

**Country:** Usa\
**Brands:** ATM\
**Status:** Threshold removed; customer confirmed both systems\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

The customer saw physical inventory in HotWax but expected more inventory to be sellable in Shopify.

## Expected behavior and requirement

Apply the business-approved threshold consistently to Online ATP and published Shopify availability.

## RCA and evidence

The documented example had five units before a one-unit threshold, leaving Online ATP and Shopify inventory at four. This was an availability-rule decision rather than evidence of a failed inventory transmission.

## Documented actions

1. I checked the inventory configuration and showed that both systems agreed after the threshold.
2. I asked the customer to confirm whether the threshold should be removed.
3. Following confirmation, I reported the threshold removed. The customer confirmed the updated availability in both HotWax and Shopify.

## Outcome and remaining work

The requested availability change was completed and acknowledged. It does not imply that thresholds should be removed for other products.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Confirm intended safety and threshold policy per item before changing availability.
- Compare computed Online ATP with Shopify after the next sync.

## Evidence basis

“Removing Threshhold,” September 8–9, 2026.
