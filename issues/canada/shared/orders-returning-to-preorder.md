# Available-stock orders returned to preorder hold

**Country:** Canada\
**Brands:** SM, DV\
**Status:** October incident recovered; later manual holds distinguished\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Orders with warehouse inventory entered preorder parking instead of routing promptly for fulfillment.

## Expected behavior and requirement

New orders should be evaluated against available warehouse stock before entering preorder hold.

## RCA and evidence

My October 10 update attributed the October 8–9 incident to a temporary delay between order synchronization and inventory checks and reported updated sync rules. Later examples were different: broker history showed a manual move into preorder parking, which the business confirmed.

## Documented actions

1. I reported re-evaluation of the affected October 8–9 orders against current stock and their release for fulfillment.
2. I monitored the order flow with the team over the holiday weekend and confirmed expected behavior.
3. The follow-up investigation checked broker history and distinguished intentional manual holds from recurrence of the original issue.

## Outcome and remaining work

The original incident was reported recovered. Later manually held orders were accepted by the business as intentional, rather than evidence that every preorder entry was a defect.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Compare import, stock-evaluation, and hold timestamps.
- Record the actor and reason for parking changes.
- Monitor fresh-order routing separately from deliberately held older orders.

## Evidence basis

My October 10 and October 12 updates and October 16–19 follow-ups in “open orders going back on pre-order.”
