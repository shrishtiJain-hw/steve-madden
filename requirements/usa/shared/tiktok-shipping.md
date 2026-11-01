# TikTok fulfillment and shipping-feed changes

**Country:** Usa\
**Brands:** DV\
**Status:** DVUS staging approach agreed; implementation unverified\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

TikTok-managed fulfillment and labels change the customer-address information available to Shopify and downstream systems.

## Expected behavior and requirement

Agree on how WMI receives a TikTok order when the actual delivery address is withheld, and retain the intended TikTok shipping identifier.

## RCA and evidence

October 30 call notes state that TikTok would fulfill and generate labels. The discussion considered Shopify Flow enrichment versus a HotWax feed change. These are business meeting notes, not an independently verified TikTok platform specification.

## Documented actions

1. I documented the fulfillment/address requirement and downstream WMI dependency.
2. The call compared source enrichment with hardcoding a reference address in the HotWax feed.
3. The recorded DVUS staging action was to use a reference address and Ship Via TIKT for TikTok orders through Mule and M3.

## Outcome and remaining work

The staging approach is more specific than the initial meeting invitations. No completed staging test, production rollout, or measured outcome is present in the reviewed record.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Validate label ownership and routing end to end with the receiving warehouse.
- Confirm agreed address handling without republishing any customer addresses.
- Test cancellation and tracking behavior before production release.

## Evidence basis

October 30 call notes in Codex chat “Update job schedule times,” with “TikTok Shipping” invitations as earlier workstream evidence.
