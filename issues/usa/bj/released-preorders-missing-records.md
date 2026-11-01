# BJ releases absent from the preorder report

**Country:** Usa\
**Brands:** BJ\
**Status:** Data location explained; business classification open\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Released orders were missing from the expected Released Preorders report.

## Expected behavior and requirement

Report coverage should match the actual source parking queue, and queue assignment should agree with the business workflow.

## RCA and evidence

Facility-change history showed the lines were released from BACKORDER_PARKING. The Released Preorders query selects PRE_ORDER_PARKING releases. I verified matching records and quantities in the released-backorders source. The business then clarified that BJ expects preorder-only handling.

## Documented actions

1. I reviewed the facility-change history for the supplied examples.
2. I compared the query eligibility rule with the source queue.
3. I verified the records in released-backorders data and requested generated-report confirmation.

## Outcome and remaining work

The apparent missing-data symptom was explained. Why the lines entered the backorder bucket, and the desired business treatment, remained under review.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Reconcile release events across both queue types before claiming data loss.
- Agree on BJ queue semantics with the business and align report naming.

## Evidence basis

My October 1 findings and the subsequent business reply in “BJ Released Preorders… please advise.”
