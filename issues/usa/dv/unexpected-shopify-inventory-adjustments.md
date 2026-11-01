# Unexpected Shopify inventory adjustments attributed to SyncJobs

**Country:** Usa\
**Brands:** DV\
**Status:** External adjustment path under investigation\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Shopify displayed incorrect inventory after adjustments attributed to a sync application.

## Expected behavior and requirement

Inventory changes should be traceable to the source publisher, affected locations, and intended full or delta update.

## RCA and evidence

My mail distinguished the observed manual adjustments under SyncJobs from HotWax actions. Later Codex call notes record a disputed full-sync-file attribution. Neither source establishes who produced the file or a final root cause.

## Documented actions

1. I examined the adjustment history and asked the team to investigate the source of the SyncJobs changes.
2. I escalated to the relevant integration owners.
3. The follow-up discussion identified the need to verify the reported full file before deciding on a hard sync.

## Outcome and remaining work

The issue remained open in the latest reviewed messages. A hard sync was discussed as conditional recovery, not documented as performed.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Correlate Shopify adjustment timestamps with outbound file and job history.
- Identify the publishing application before reapplying stock.
- Validate a small affected sample before any broad recovery.

## Evidence basis

“INVENTORY DISCREPENCIES Hotwax + Shopify,” October 28–29, plus October 29 call notes in Codex chat “Update job schedule times.”
