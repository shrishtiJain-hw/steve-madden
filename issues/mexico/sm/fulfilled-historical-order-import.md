# Fulfilled order import resolved to a virtual location

**Country:** Mexico\
**Brands:** SM\
**Status:** Import blocker identified; recovery route proposed\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

An already-fulfilled Shopify order failed OMS import while archived-order behavior was being investigated.

## Expected behavior and requirement

Historical import should record the completed shipment with correct location context and avoid issuing inventory again.

## RCA and evidence

The Codex review found the Shopify fulfillment location mapped to a virtual brokering facility. That explained the fulfillment-processing blocker. Merely unarchiving the order would not repair the location resolution.

## Documented actions

1. I investigated archived-order import behavior and the fulfillment-location mapping.
2. The code review identified a historical-order route that records history without a second inventory issuance.
3. The proposed recovery required checking for existing order/history records and confirming the deployed service before a targeted import. No live import was performed.

## Outcome and remaining work

A targeted recovery design was established. Neither a production mapping change nor successful historical import is claimed.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Check existing source identity and history before retrying.
- Confirm a physical fulfillment location or explicitly supported historical behavior.
- Verify completed state and avoid duplicate inventory issuance.

## Evidence basis

Codex chat “Check Shopify archived order imports,” October 28, 2026.
