# New DV location missing from brokering choices

**Country:** Canada\
**Brands:** DV\
**Status:** Location added; customer confirmed availability\
**Contribution:** Team incident reference; personal implementation not established

## Issue and business impact

A newly opened store was unavailable as an order-brokering option.

## Expected behavior and requirement

A location approved for brokering must reach the integration’s location feed and become selectable in OMS.

## RCA and evidence

The team identified that the new store had not yet been added to the feed. Once added, the customer could see it in the brokering options.

## Documented actions

1. I was included in the support workstream.
2. The team located the missing feed entry and added the new location.
3. The customer confirmed the location appeared as a brokering option.

## Outcome and remaining work

The selection problem was resolved. Actual order allocation and fulfillment at the new location were not demonstrated by that confirmation alone.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Include feed enrollment in new-location readiness checks.
- Test one eligible order after the location becomes selectable.

## Evidence basis

“Brokering facilities not appearing - Dolce Vita Canada,” October 7, 2026.
