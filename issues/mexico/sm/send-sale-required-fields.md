# PredictSpring send-sale feed failed required-field checks

**Country:** Mexico\
**Brands:** SM\
**Status:** Field-level findings shared; retests requested\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

A Mexico staging send-sale order failed downstream checks for Style, CustomerNo, and ShipState.

## Expected behavior and requirement

Validate each reported field against the actual emitted file and normalize source identifiers consistently.

## RCA and evidence

My findings showed three different situations: the product lacked an SKU, the inbound state abbreviation differed from the configured mapping, and CustomerNo was present despite being reported missing. A single generic missing-fields RCA would conceal these differences.

## Documented actions

1. I compared the source product and PredictSpring payload with the warehouse brokered output.
2. I explained the blank Style and ShipState separately.
3. I supplied the feed and asked Mule to investigate why its present CustomerNo value was rejected.
4. QA created additional test orders for end-to-end retesting.

## Outcome and remaining work

The diagnostic breakdown is documented. Successful downstream processing of all new tests was still pending.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Validate SKU presence before export.
- Use an agreed state-code normalization contract.
- Capture the exact file and field parsed downstream when a nonblank value is rejected.

## Evidence basis

My October 30 mail in “MX STG PS sendsale test,” corroborated by the related Codex investigation.
