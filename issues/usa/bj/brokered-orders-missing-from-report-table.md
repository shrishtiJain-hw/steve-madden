# Brokered BJ orders missing from reporting data

**Country:** Usa\
**Brands:** BJ\
**Status:** Recovery extract supplied; RCA open\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

The reporting team could not find a day’s brokered BJ orders in its expected table.

## Expected behavior and requirement

Operational brokering events should be available to the downstream reporting dataset for the same business date.

## RCA and evidence

The mails establish missing reporting records and the availability of a replacement extract, but do not establish whether export, table ingestion, date filtering, or a later transformation caused the gap.

## Documented actions

1. I acknowledged the missing brokered-items records and investigated the affected date.
2. I supplied a file containing the BJ orders brokered that day.
3. I explicitly kept the RCA open in my delivery update.

## Outcome and remaining work

A recovery dataset was delivered. Delivery of that file is not proof that the recurring table-population path was repaired.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Reconcile OMS broker events, exported records, and destination table counts.
- Check business-date and timezone filters before regenerating data.
- Validate a subsequent scheduled run.

## Evidence basis

My September 29 and October 1 messages in “BJ Brokered orders from 09/17 not in Hotwax Table.”
