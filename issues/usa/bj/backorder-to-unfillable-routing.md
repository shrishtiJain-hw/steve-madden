# BJ backorder styles routed into Unfillable

**Country:** Usa\
**Brands:** BJ\
**Status:** New-order configuration fixed; backlog correction underway\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Orders for BJ backorder styles entered Unfillable instead of a hold queue, exposing them to inappropriate auto-cancellation.

## Expected behavior and requirement

Recognized backorder items should enter the correct parking queue with the appropriate PO association and cancellation handling.

## RCA and evidence

A configuration problem caused the incorrect route. A separate glove example had no PO in HotWax, so the system could not recognize it as a preorder. The missing-PO case should not be treated as the same failure mechanism.

## Documented actions

1. I coordinated the investigation and reported the configuration fix live.
2. My update confirmed new BJ backorder orders were now held correctly.
3. I documented backlog work: move applicable lines out of Unfillable, clear their auto-cancel dates, and complete PO linking where applicable.
4. I explained the missing-PO exception and asked the business to flag styles launched before their PO arrives.

## Outcome and remaining work

The new-order behavior was reported corrected. Backlog processing was still underway in the final update and must not be marked fully complete.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Test new orders both with and without a qualifying PO.
- Verify old affected lines separately, including cancel dates and PO links.
- Confirm the business distinction between preorder and backorder terminology.

## Evidence basis

My October 19 resolution update in “BJ Unfillable Order Issue.”
