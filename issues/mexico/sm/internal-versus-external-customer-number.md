# POS customer number used an internal facility ID

**Country:** Mexico\
**Brands:** SM\
**Status:** Code path identified; permanent fix proposed\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

The warehouse brokered feed emitted an internal selling-store identifier where the downstream contract expected its external customer code.

## Expected behavior and requirement

Resolve the selling facility’s external ID for CustomerNo and distinguish selling location from fulfillment location.

## RCA and evidence

The Codex code trace showed POS CustomerNo sourced directly from orderFacilityId. The import lookup used externalId without excluding closed facilities, and two facility records shared that external value. Which duplicate/cache path selected the old record at runtime remained unconfirmed.

## Documented actions

1. I investigated why a facility-replacement workaround still produced the old customer number.
2. The analysis compared the saved ship-group facility with import and export mapping code.
3. The proposed correction resolves the selling facility’s external ID and makes import lookup unambiguous. No code or UAT data change was executed in that chat.

## Outcome and remaining work

The wrong field source was identified. Feed mapping changes, duplicate-master cleanup, and existing-order correction remained proposed.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Test internal and external facility IDs that differ.
- Reject ambiguous external-ID matches rather than silently choosing one.
- Validate an existing affected order separately from a fresh import.

## Evidence basis

Codex chat “Fix brokered feed customer number,” October 31, 2026.
