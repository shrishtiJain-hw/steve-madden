# Mexico order-type change to stop automatic invoicing

**Country:** Mexico\
**Brands:** SM, DV\
**Status:** Production configuration and business confirmation recorded\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

The Mexico business required a change in order processing so the affected e-commerce orders were no longer automatically invoiced.

## Expected behavior and requirement

Apply the agreed order-type configuration to both SM-MX and DV-MX and verify its invoicing effect downstream.

## RCA and evidence

The correspondence records a configuration requirement rather than a diagnosed service failure. The exact order-type values are not reconstructed where they were not present in the reviewed messages.

## Documented actions

1. I confirmed the configuration moved to production for both brands.
2. The business checked orders from the effective date and later confirmed automatic invoicing had stopped.

## Outcome and remaining work

The production change and its business effect were confirmed. No broader tax or invoicing-policy claim is made.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Test one new eligible order per brand.
- Separate existing historical orders from post-change behavior.

## Evidence basis

My September 28 deployment update and October 8 business confirmation in “Change order type for Mexico.”
