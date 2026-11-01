# Fully discounted ATM orders in downstream processing

**Country:** Usa\
**Brands:** ATM\
**Status:** M3 processing confirmed\
**Contribution:** Investigation workstream participant; team validation and recovery reference

## Issue and business impact

ATM e-commerce orders were flagged in a price/discount processing thread and needed feed-level review.

## Expected behavior and requirement

A legitimately fully discounted order should remain valid when its monetary fields agree with Shopify and the downstream contract.

## RCA and evidence

Team review found that the sampled feeds matched Shopify and represented fully discounted orders. The correspondence does not establish a distinct code defect or the exact downstream rejection rule.

## Documented actions

1. I was included in the investigation workstream.
2. The team requested the exact problematic fields, supplied the original outbound files, and spot-checked their values against Shopify.
3. The downstream team confirmed the orders processed in M3.

## Outcome and remaining work

The affected processing was confirmed successful. Personal code authorship and a specific permanent pricing fix are not asserted.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Include zero-net-value orders in feed regression coverage.
- Reconcile line price, discount, tax, and totals without assuming a zero net value is corrupt.

## Evidence basis

“ATM ECOM orders Price discount issue,” September 24–29, 2026.
