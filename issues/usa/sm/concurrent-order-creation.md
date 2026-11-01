# Duplicate order headers during overlapping import

**Country:** Usa\
**Brands:** SM\
**Status:** Race condition supported; exact creator unresolved\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

The same Shopify order appeared in two OMS order-header records.

## Expected behavior and requirement

Concurrent ingestion paths should converge on one canonical order identity and preserve a reliable Shopify mapping.

## RCA and evidence

The Codex investigation correlated header screenshots and logs. The Maarg new-order decision preceded the other header’s recorded entry by about 0.4 seconds, with both creations overlapping. This supports a race. The exact service that created the first header was not identified, and a missing mapping is not independently proven to be the cause.

## Documented actions

1. I investigated the duplicate header records with Codex.
2. The investigation compared creation timestamps, external identity fields, and creation logs.
3. The conclusion was narrowed after a more precise timestamp check corrected the initial sequence.

## Outcome and remaining work

The diagnosis supports concurrent creation but does not establish a deployed fix or authorize deleting either order.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Trace both creators and their duplicate checks.
- Propose a shared idempotency key or atomic uniqueness protection on source order identity.
- Test parallel and replayed events before applying cleanup to existing orders.

## Evidence basis

Codex chat “Fix duplicate SMUS order rows,” October 30, 2026. Log-derived findings are historical investigation evidence, not fresh live checks.
