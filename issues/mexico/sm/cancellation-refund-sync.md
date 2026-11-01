# Mexico cancellations without Shopify refunds

**Status:** Team-reported fix  
**Contribution:** Team resolution reference; individual implementation not asserted

**Country:** Mexico  
**Brand scope:** SM

## Business context

Orders could appear cancelled in Shopify while the corresponding refund still required manual processing.

## Approach and contribution

The team distinguished cancellation state from refund completion. Follow-up correspondence identified Shopify refund processing on cancellation as disabled.

## Outcome and remaining work

A team update reported the issue fixed. This case records the shared finding and the operational distinction; it does not attribute the implementation to me.

## Validation and next checks

Recommended checks: verify cancellation and refund independently, inspect payment transaction outcomes, test partial cancellation, and confirm no duplicate refund on retry.

## Evidence basis

“Mexico cancellation not flowing to Shopify,” including the October follow-up reporting the disabled refund-processing setting.
