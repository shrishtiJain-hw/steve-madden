# Next Day orders imported as Standard

**Country:** Usa\
**Brands:** ATM\
**Status:** Configuration live; staging import confirmed\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Expedited ATM orders entered OMS as Standard, putting the promised shipping service at risk.

## Expected behavior and requirement

Recognize both the established Overnight service and a custom Shopify Admin shipping value of Next Day.

## RCA and evidence

The Next Day shipping configuration was missing for ATM. Import could not resolve that label and fell back to Standard. QA identified custom shipping entered in Shopify Admin as the source of the new value.

## Documented actions

1. I identified the missing shipping configuration and reported the fallback behavior.
2. I confirmed the Next Day mapping had been added and requested a staging order.
3. QA confirmed a custom Next Day staging order imported successfully. I subsequently confirmed the configuration was live in production.

## Outcome and remaining work

New orders were covered by the configuration change. The already-shipped examples were intentionally left unchanged. This import mapping fix is separate from the downstream carrier-code fix.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Test Ground, 2nd Day, Overnight, and custom Next Day values.
- Check imported service and outbound carrier code independently.

## Evidence basis

“ATM Next Day Orders,” September 25–October 2, 2026. The mailbox also contains an assignment notification for the related issue.
