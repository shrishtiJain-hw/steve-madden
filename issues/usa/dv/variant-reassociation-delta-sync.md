# Inventory missed after Shopify variant reassociation

**Country:** Usa\
**Brands:** DV\
**Status:** Inventory flow restored; customer confirmed\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

New sizes under a reorganized Shopify product did not all receive available OMS inventory.

## Expected behavior and requirement

After variant or inventory-item associations change, an affected variant should be eligible for an inventory refresh even if stock quantity did not change.

## RCA and evidence

Moving variants to the main Shopify product changed their variant and inventory associations. Delta sync selected inventory records updated since its previous run. Several sizes later received stock updates and synced, while one unchanged size retained an old timestamp and was skipped under the new association.

## Documented actions

1. I traced the association change and compared the affected inventory-update histories.
2. I explained why the sizes that received subsequent changes recovered automatically.
3. My update documented refreshing the unchanged size’s record so the scheduled job selected it.
4. I confirmed inventory was flowing for all affected sizes and received customer confirmation.

## Outcome and remaining work

The reported sizes synced successfully. This recovery points to a mapping-change refresh requirement in addition to quantity-change selection.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Refresh eligibility after mapping changes, not only stock changes.
- Test a reassociated variant whose quantity remains unchanged.
- Verify Shopify inventory-item mapping and final availability.

## Evidence basis

My September 11 RCA and the customer confirmation in “DV ROXLA… New Sizes Needing Inventory to Flow from Hotwax.”
