# Physical stock excluded by the selected inventory channel

**Country:** Usa\
**Brands:** SM\
**Status:** Channel-selection diagnosis; no resync performed\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

The user requested an inventory resync because Online ATP appeared zero for variants with physical stock.

## Expected behavior and requirement

Online ATP must be inspected under the channel that actually owns the eligible facilities.

## RCA and evidence

Screenshots reviewed in Codex showed all physical ATP excluded under the selected ATM channel. The contributing facilities belonged to the SM Shopify facility group. Zero availability in the ATM view therefore did not prove that SM inventory sync had failed.

## Documented actions

1. I compared physical ATP, excluded ATP, and Online ATP.
2. I checked facility-group membership and identified the mismatched selected channel.
3. The recommended next step was to inspect the existing SM channel and confirm the actual Shopify publishing channel. No facilities were added to ATM and no resync was performed.

## Outcome and remaining work

The investigation explains the zero in the selected view. Final Shopify quantities were not verified live.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Check channel ownership before recalculation or resync.
- Avoid broad facility-membership changes as a workaround for a display-selection issue.

## Evidence basis

Codex chat “Resync JKOODLES BLUSH inventory,” October 26, 2026.
