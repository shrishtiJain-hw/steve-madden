# Orders stalled in Created across US brands

**Country:** Usa\
**Brands:** SM, DV, BJ\
**Status:** Reported backlog resolved; technical RCA unavailable\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Customer service reported a large backlog of Created orders spanning SM, DV, and BJ.

## Expected behavior and requirement

Imported orders should progress according to eligibility rules rather than remain indefinitely at creation.

## RCA and evidence

The source lists affected examples across all three brands and confirms recovery. It does not identify whether tags, approval evaluation, job execution, or another service caused the backlog.

## Documented actions

1. I acknowledged the shared Created-state backlog and coordinated investigation.
2. I reported that affected orders were now progressing beyond Created.
3. Customer service acknowledged the recovery.

## Outcome and remaining work

The stated recovery is supported. A permanent technical RCA or exact implementation is not available and is not fabricated.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Monitor Created-state age by brand and approval reason.
- Compare old backlog and fresh orders after recovery.
- Preserve eligibility checks when replaying stuck messages.

## Evidence basis

“Orders Stuck in Created Status,” September 17–18, 2026.
