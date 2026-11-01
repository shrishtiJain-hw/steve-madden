# Dolce Vita orders delayed in OMS import

**Country:** Usa\
**Brands:** DV\
**Status:** Reported backlog imported; recurring cause open\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Customer-service teams could not locate recent Shopify orders in HotWax.

## Expected behavior and requirement

Eligible orders should import once, become visible to operations, and progress to the appropriate processing state.

## RCA and evidence

The thread describes a sync delay and successful recovery imports. It does not identify the failing job, queue, or permanent technical cause.

## Documented actions

1. I reported the requested orders imported and acknowledged the sync delay.
2. The team imported the remaining stuck examples and continued the root-cause investigation.
3. Customer service acknowledged the recovery and agreed to flag additional missing examples.

## Outcome and remaining work

The supplied backlog was recovered. The root cause and durable prevention remained open.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Compare source order creation with OMS import timestamps.
- Check queue age, retries, and duplicate identification before replay.

## Evidence basis

“Dolce Vita Orders not importing in Hotwax,” October 13–15, 2026.
