# Contact updates blocked during Shopify fulfillment

**Country:** Canada\
**Brands:** SM, DV\
**Status:** Source-system update guidance confirmed by customer\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Attempts to add shipping contact information through OMS failed once an order was already in Shopify fulfillment.

## Expected behavior and requirement

Update customer shipping details in the authoritative source and allow the downstream synchronization to propagate them.

## RCA and evidence

The reviewed example was already in fulfillment, restricting the attempted contact update from HotWax. My guidance was to edit the shipping contact directly in Shopify. Later examples used the same source-first approach.

## Documented actions

1. I identified the fulfillment-state restriction for the affected order.
2. I directed the user to make the shipping-contact correction in Shopify Admin.
3. Customers confirmed the advised source update fixed the original example and later contact-update requests.

## Outcome and remaining work

The advised path restored the affected workflow. No universal promise about every post-fulfillment address mutation is made.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Check fulfillment state before deciding which system can accept an edit.
- Verify the downstream contact sync and label prerequisites after the source correction.

## Evidence basis

“label to fix,” September 3, and October Canada phone-update follow-ups.
