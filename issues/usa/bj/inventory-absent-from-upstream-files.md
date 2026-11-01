# BJ inventory missing from the M3 source feed

**Country:** Usa\
**Brands:** BJ\
**Status:** Upstream absence verified; replenishment confirmation requested\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

A BJ style showed no inventory in OMS even though the business expected availability.

## Expected behavior and requirement

Source inventory must include the correct product identifier before OMS can import and publish it.

## RCA and evidence

I checked four M3 reset files across late August and early September and found the affected UPC absent from all four. That supports an upstream-data gap for the inspected files, not a confirmed OMS import failure.

## Documented actions

1. I traced the product identifier through the available reset files.
2. I reported the repeated absence and confirmed no inventory had been received for that identifier.
3. The team asked the source-system owners whether stock should have been supplied.

## Outcome and remaining work

The investigation located the missing data at the source-file boundary. Inventory restoration and upstream correction are not confirmed.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Check the next source file and import result for the same identifier.
- Distinguish a missing row from a valid row carrying zero stock.

## Evidence basis

My September 15 update in “BJ Inventory Issue.”
