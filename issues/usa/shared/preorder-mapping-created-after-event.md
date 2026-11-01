# Preorder update skipped before Shopify mapping existed

**Country:** Usa\
**Brands:** Brand scope unconfirmed\
**Status:** Targeted push reported in Codex discussion\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Some sizes showed preorder supply in OMS and M3 but did not expose the expected preorder behavior in Shopify.

## Expected behavior and requirement

A product linked to Shopify after its original preorder event should receive the outstanding preorder configuration.

## RCA and evidence

The Codex investigation recorded September preorder events followed by October Shopify mappings. The initial updates could not resolve a Shopify variant. Delta processing did not revisit the old events after mapping creation. The source conversation distinguishes mapping creation time from Shopify product creation time.

## Documented actions

1. I investigated the mapping timeline and old preorder-event dates.
2. The discussion identified why recent-change filtering missed those records after linking.
3. A targeted push and enabled continue-selling setting were reported in the discussion, with verification cautions retained.

## Outcome and remaining work

A recovery was reported in the chat. A fresh production verification and exact brand assignment are not inferred from the product name alone.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Replay pending preorder state when a previously missing mapping becomes available.
- Verify both preorder tags and continue-selling settings after recovery.

## Evidence basis

Codex chat “Investigate CALICO-SEQ BLUSH sizes,” October 27, 2026.
