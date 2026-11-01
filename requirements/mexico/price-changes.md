# Mexico price and discount feed changes

**Status:** Requirements clarified; staging validation shared  
**Contribution:** Requirement analysis, mapping clarification, and QA coordination

## Business context

Mexico feeds needed revised pricing semantics while retaining existing column headers across warehouse, store, and return workflows.

## Approach and contribution

I translated stakeholder requests into a concrete mapping and shared staging output for validation:

| Column | Required business meaning |
| --- | --- |
| L | Coupon or discount amount |
| T | Compare-at price, falling back to the previous unit price when unavailable |
| AU | Discounted unit price before coupons |

I highlighted that unchanged headers could conceal a changed meaning, clarified that column T must not be blank, and followed up on VAT treatment across the OMS, Mule, and M3 boundaries.

## Outcome and remaining work

Mapping clarification and sample validation are documented. The thread contains conflicting VAT expectations and a later request for final confirmation; this case does not claim final VAT sign-off or completed deployment for every feed.

## Validation and next checks

Proposed QA matrix: compare-at present/absent, coupon present/absent, multi-line orders, returns, rounding, and VAT at each interface. Use synthetic values and reconcile line totals before approval.

## Evidence basis

“Mexico Price Changes,” including my September 22, September 29–30, October 6, and later VAT clarification messages.
