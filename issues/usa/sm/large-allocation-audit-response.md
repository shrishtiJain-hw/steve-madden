# Large allocation response failed database indexing

**Country:** Usa\
**Brands:** SM\
**Status:** Allocator-side deployment reported; order brokered\
**Contribution:** Investigation participant; upstream team fix reference

## Issue and business impact

A multi-item order remained unbrokered despite available fulfillment options.

## Expected behavior and requirement

Allocation should complete when several products and candidate locations generate a large audit response.

## RCA and evidence

The allocator owner reported that the large API audit response failed database indexing. Product/location combinations enlarged the stored response. This was a separate failure from the old-UPC examples in the same conversation.

## Documented actions

1. I participated in the broader unbrokered-order investigation.
2. The team separated the multi-item allocation failure from catalog-identity failures.
3. The allocator owner reported a deployment for the oversized-response scenario, and the customer confirmed the specific order brokered.

## Outcome and remaining work

A targeted order recovery and upstream deployment were reported. The exact code change and broad post-deployment regression results are not available in the mails.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Include large baskets and many candidate locations in allocator tests.
- Prevent audit persistence failure from silently blocking fulfillment decisions.

## Evidence basis

Allocator-owner RCA and customer confirmation in “UNF order with inventory not brokering,” September 28–29.
