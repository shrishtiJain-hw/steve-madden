# Cancelled items remained in fulfillment queues

**Country:** Usa\
**Brands:** SM\
**Status:** Affected examples cleared; store confirmation received\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Cancelled items continued to appear in store fulfillment worklists, creating unnecessary follow-up and risk of acting on obsolete work.

## Expected behavior and requirement

A cancelled line should cease to be actionable in its assigned store queue.

## RCA and evidence

One documented example retained an outdated displayed order state. My update states the order was refreshed and removed. Other examples were confirmed cancelled and absent after verification. The mails do not establish a common technical cause for all stores.

## Documented actions

1. I checked line status, assigned store, and the specific fulfillment tab.
2. For the documented stale-state example, I reported refreshing the order and clearing it from the queue.
3. I requested fresh store/tab screenshots when symptoms persisted and received confirmations that the listed examples were no longer visible.

## Outcome and remaining work

The referenced SM examples were cleared. A separate DV store-queue case remained open and is tracked independently.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Verify the same store and tab as the user before declaring success.
- Compare line status with queue membership after refresh.
- Prevent actions on cancelled lines even if the client display is stale.

## Evidence basis

“STORE 542- Fulfillment order,” “Order Issues,” “ECOMMERCE,” and related October SM queue follow-ups.
