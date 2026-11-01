# Wrong product imagery from a shared parent handle

**Country:** Canada\
**Brands:** SM\
**Status:** Immediate correction confirmed; permanent code fix planned\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

A Canada product displayed imagery associated with a different shop’s product.

## Expected behavior and requirement

Product associations and imagery must resolve within the correct shop context.

## RCA and evidence

The team reported that both shops shared the same parent handle. The immediate correction restored the correct images, while a permanent code fix was planned separately.

## Documented actions

1. I coordinated the image-discrepancy investigation and communicated its progress.
2. A teammate reported the shared-parent-handle cause and immediate recovery.
3. The customer checked OMS and confirmed the correct images.

## Outcome and remaining work

The immediate correction was accepted. The planned permanent code deployment was not independently confirmed in this thread.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Scope parent-product lookups by shop as well as handle.
- Test identical handles across two shops.
- Verify both existing images and a subsequent product refresh.

## Evidence basis

“SMCA - GRAZIE style - Photos Discrepancy,” October 19, 2026.
