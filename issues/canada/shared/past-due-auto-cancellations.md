# Past-due unfillable orders did not auto-cancel

**Country:** Canada\
**Brands:** SM, DV\
**Status:** Listed orders cancelled after background processing refresh\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Past-due orders remained open beyond their expected cancellation timing.

## Expected behavior and requirement

Orders that meet the configured cancellation criteria should be processed by the scheduled background workflow.

## RCA and evidence

The reply documents delayed background processing and its refresh. It does not identify a specific service exception, scheduling defect, or database cause.

## Documented actions

1. I investigated the delayed cancellations.
2. My update states that background processing was refreshed for the past-due orders.
3. I confirmed the listed orders cancelled as expected and asked the business to flag recurrence.

## Outcome and remaining work

The affected examples were cancelled. A deeper recurring RCA is not claimed.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Monitor due-versus-processed cancellation counts.
- Verify policy eligibility before retrying background work.
- Check a later scheduled run independently.

## Evidence basis

My September 5 response in “Unfillable Report - Auto Cancel?” Brand coverage follows the Canada report workstream; individual examples are not republished.
