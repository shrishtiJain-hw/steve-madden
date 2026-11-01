# Send-sale shipping charges and tax in outbound feeds

**Country:** Usa\
**Brands:** SM\
**Status:** Staging feeds reviewed; production move requested\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

The send-sale flow carried shipping charges in the source order but required clarification on their representation as outbound feed items.

## Expected behavior and requirement

Preserve the approved shipping-charge item and tax through Store Fulfilled feed generation.

## RCA and evidence

My review confirmed shipping amount in the PredictSpring payload and OMS. Later testing addressed a missing shipping-item representation. The thread records acceptance to proceed, rather than a final deployed-state receipt.

## Documented actions

1. I compared the source payload, OMS charges, and outbound feed.
2. I asked the team to clarify the dedicated shipping item and shared staging test feeds.
3. QA supplied shipping-tax examples, and the receiving stakeholder requested moving the change to production.

## Outcome and remaining work

Staging review and a production-move request are documented. A request to deploy is not evidence of completed production deployment.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Test standard and expedited service charges including shipping tax.
- Reconcile order charges to their dedicated feed item without double-counting.

## Evidence basis

My September–October replies in “Send Sales.”
