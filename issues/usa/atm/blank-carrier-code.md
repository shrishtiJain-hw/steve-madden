# Warehouse feed rejected for a blank carrier code

**Country:** Usa\
**Brands:** ATM\
**Status:** Feed mapping updated; affected feeds regenerated\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

ATM warehouse orders did not reach WMI because their brokered feeds lacked a carrier code used to derive ShippingType.

## Expected behavior and requirement

Every supported shipping-method label must produce the carrier value expected by downstream processing.

## RCA and evidence

The feed recognized Overnight but did not yet recognize Next Day. The unsupported input left the carrier field blank. This is a documented RCA, rather than an inference from a generic upload error.

## Documented actions

1. I clarified that the feed contained the Shipping Type header with blank values.
2. I communicated the cause: the incoming service label had changed from Overnight to Next Day.
3. My RCA update confirmed the feed was updated to handle Next Day and the affected feeds were regenerated and resent.

## Outcome and remaining work

Recovery and mapping updates were reported. The thread requests downstream verification and does not include a separate WMI acceptance receipt for every replayed order.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Assert a nonblank carrier code before export.
- Test both shipping labels through OMS, Mule, M3, and WMI.
- Verify retries do not create duplicate warehouse orders.

## Evidence basis

My October 6 RCA in “ATM order not in WMI,” with the related upload-failure conversation.
