# Preserve separate PO lines for different arrival dates

**Country:** Shared\
**Brands:** Brand scope unconfirmed\
**Status:** Fresh-import UI validation recorded; rollout reported in call notes\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Repeated product identifiers on different PO lines needed to retain their quantities and arrival dates rather than collapse into one line.

## Expected behavior and requirement

Carry the PO line identifier in the feed and preserve each split line in the newly imported PO.

## RCA and evidence

The requirement concerns line identity: product ID alone is insufficient when the same product arrives in separate dated quantities. No retroactive update of existing POs was promised.

## Documented actions

1. I reviewed fresh-import screenshots against the supplied feed with Codex.
2. The recorded comparison matched split quantities and dates and reconciled the complete imported total.
3. A subsequent reply draft documented new-PO-only behavior; call notes separately reported the HotWax-side rollout while downstream changes remained dependent on Mule.

## Outcome and remaining work

The chat supports initial import/UI validation. Draft text is not treated as a sent deployment confirmation. Repeat-import idempotency and selective line-update tests remained recommended.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Re-import the same file and verify unchanged row count and total.
- Change one split line and confirm only that line updates.
- Confirm downstream deployment and business acceptance independently.

## Evidence basis

Codex chats “Summarize Hotwax split PO thread” and “Update job schedule times,” October 27–30.
