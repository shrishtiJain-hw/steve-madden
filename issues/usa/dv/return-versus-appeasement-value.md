# Physical return value and customer refund diverge

**Country:** Usa\
**Brands:** DV\
**Status:** Accounting contract unresolved\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

M3 appeared to record both appeasement and return values for a case involving a TikTok refund and a separate Narvar physical return.

## Expected behavior and requirement

Cash refund and inventory-return valuation must retain their distinct meanings while producing the business-approved M3 records.

## RCA and evidence

Team review identified two source records: a TikTok customer refund and a Narvar item return without an attached payment refund. A zero refund on the physical return did not make its sales-value export zero. The business disputed the resulting M3 behavior, so the explanation is not final acceptance.

## Documented actions

1. I coordinated review of the return, appeasement records, and financial exports.
2. The team documented how the separate source events became different feed records.
3. Stakeholders requested additional investigation into zero-value handling in M3.

## Outcome and remaining work

The transformation behavior was explained, but the required accounting treatment and correction remained open.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Use an event-level reconciliation showing cash movement separately from stock movement.
- Agree on expected zero-refund physical-return records before changing the feed.
- Test duplicate and out-of-order refund/return events.

## Evidence basis

“Return/Appeasement,” October 16–29, and related October 29 Codex call notes.
