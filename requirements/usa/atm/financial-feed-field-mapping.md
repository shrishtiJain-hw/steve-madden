# ATM warehouse and shipping-item feed mapping

**Country:** Usa\
**Brands:** ATM\
**Status:** Samples delivered; field semantics clarified\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

ATM feed changes used labels such as WH, Location, Facility, and Picked Up Store inconsistently across feed families.

## Expected behavior and requirement

Define each column separately for Store Fulfilled Item, Warehouse Brokered, and Appeasement feeds.

## RCA and evidence

The ambiguity was in the integration contract: some requested columns did not exist in the supplied feed family, so applying a requested value by column name alone could change the wrong field.

## Documented actions

1. I listed the available fields and requested clarification before changing the mapping.
2. I shared sample Store Fulfilled Item, Appeasement, and Warehouse Brokered feeds.
3. The stakeholder clarified that the shipping-item WH should use the current Picked Up Store value, that Picked Up Store should be blank, and that the appeasement facility should be RM.

## Outcome and remaining work

Concrete mapping guidance was obtained. Full production deployment and downstream acceptance for every feed are not documented in this thread.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Version the mapping by feed family rather than reusing ambiguous display labels.
- Validate shipping items and appeasement items separately.

## Evidence basis

My October 6 and October 8 messages and the stakeholder response in “ATM Mapping from hotwax.”
