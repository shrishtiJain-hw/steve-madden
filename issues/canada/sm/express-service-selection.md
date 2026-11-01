# Express shipping label failed under an incompatible service

**Country:** Canada\
**Brands:** SM\
**Status:** Label generated; operating guidance acknowledged\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

A valid shipping address still produced a label-generation failure.

## Expected behavior and requirement

The selected carrier service must match the requested Express shipping option.

## RCA and evidence

I confirmed the address was correct. The order used 1–3 Business Days instead of the required Express option. Changing the selection to 1–2 Business Days generated the label successfully.

## Documented actions

1. I checked the address and shipping-service selection.
2. I changed the method to the appropriate Express selection and confirmed label generation.
3. I explained the correct selection for future Express shipments; customer service acknowledged the guidance.

## Outcome and remaining work

The affected label was generated successfully. The resolution was configuration/selection correction rather than an address edit.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Validate carrier-service compatibility before requesting a label.
- Retest the intended service without reissuing an already-valid label.

## Evidence basis

My September 15 RCA in “ACTION REQUIRED… Label Issue.”
