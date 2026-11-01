# Changed product UPC blocked Fenix brokering

**Country:** Usa\
**Brands:** SM\
**Status:** Orders brokered through a temporary upstream workaround\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Orders stayed unfillable even though inventory existed for the product’s current UPC.

## Expected behavior and requirement

Order-line identity, catalog identity, and allocator inventory should refer to the same sellable variant.

## RCA and evidence

I supplied request and response evidence showing Fenix evaluated an old UPC and returned an out-of-stock error while Shopify and HotWax held the current UPC. The team separately found stale product mappings. Correcting OMS display data alone did not update the allocator’s old order context.

## Documented actions

1. I shared API evidence demonstrating that requests were sent and the response referenced the old identifier.
2. I coordinated product-mapping cleanup discussion with catalog and allocation owners.
3. The allocator owner temporarily duplicated inventory under the unused UPC to release the blocked orders. The customer confirmed brokering.

## Outcome and remaining work

Operational recovery was confirmed. The inventory duplication was explicitly a teammate’s temporary workaround, with a long-term solution still required. Planned product deletion is not claimed as completed.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Design an explicit identifier-migration policy for outstanding orders.
- Reconcile temporary allocator stock and eliminate any duplicate availability.
- Verify the permanent correction with an order created before the UPC change.

## Evidence basis

“UNF order with inventory not brokering,” September 24–30, 2026.
