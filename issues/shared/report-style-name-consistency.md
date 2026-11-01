# Inconsistent product names across operational reports

**Country:** Shared\
**Brands:** SM\
**Status:** Incorrect output established; production cause unresolved\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Unreconciled, Released, and Combined preorder/backorder reports showed inconsistent product/style text for the same variant.

## Expected behavior and requirement

Use the business-approved recognizable product name consistently, with color and size kept distinct and no repeated size suffix.

## RCA and evidence

Codex review traced an earlier item-description source and later parent-product-name changes. Combined and Released outputs still differed. The user clarified that a recognizable product name, rather than a literal Shopify variant option string, was the desired business value. Possible execution-path, stale-data, and source-parent issues remained unproven.

## Documented actions

1. I compared the report examples and clarified the expected business text.
2. The review traced source fields and previous parent-name query changes.
3. The recommendation retained the parent-name direction and proposed tracing actual SQL, source parent data, generated data, and the final attachment.

## Outcome and remaining work

The naming inconsistency is supported. The chat explicitly did not perform further production checks or deploy a fix. Shared brand indexing describes the US reporting workstream; the inspected attachments were SMUS examples.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Trace the same variant through every affected report.
- Check parent-join cardinality so units and demand do not multiply.
- Verify actual job SQL and downstream refresh before declaring deployment success.

## Evidence basis

Codex chat “Fix report STYLE values,” October 31, 2026.
