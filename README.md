![STEVE MADDEN engineering portfolio](assets/banner.svg)

# STEVE MADDEN

Commerce operations, integration requirements, incident recovery, and technical investigations across the Steve Madden workstream.

**Shrishti Jain** · Product Associate · Business analysis and commerce operations

**59 case studies** · 45 issues and investigations · 14 requirements and delivery records\
Last curated: November 2, 2026

## Coverage and navigation

| Country | Brands |
| --- | --- |
| USA | SM, DV, BJ, ATM |
| Canada | SM, DV, KG |
| Mexico | SM, DV, KG |

SM = Steve Madden; DV = Dolce Vita; BJ = Betsey Johnson; ATM = ATM Collection; KG = Kurt Geiger. Case-specific scope appears beside each record. Country membership does not imply that every issue affected every brand.

- [USA issues](issues/usa/README.md) · [Canada issues](issues/canada/README.md) · [Mexico issues](issues/mexico/README.md)
- [USA requirements](requirements/usa/README.md) · [Canada requirements](requirements/canada/README.md) · [Mexico requirements](requirements/mexico/README.md)
- [Investigation guide](playbooks/investigation-guide.md) · [Review scope](RESEARCH_SCOPE.md)


## Case study register

| Case | Country | Brand scope | Recorded status |
| --- | --- | --- | --- |
| [Restoring missing financial feed shipments](issues/canada/dv/financial-feed-missing-shipments.md) | Canada | DV | Resolved in team update; customer validation requested |
| [Financial feed retry needed outside the restricted window](issues/canada/dv/financial-feed-processing-window.md) | Canada | DV | Sales feed reprocessed; downstream confirmation requested |
| [DV store could not complete shipping from fulfillment](issues/canada/dv/fulfillment-session-recovery.md) | Canada | DV | Customer confirmed recovery after session refresh |
| [New DV location missing from brokering choices](issues/canada/dv/new-location-missing-from-brokering.md) | Canada | DV | Location added; customer confirmed availability |
| [Contact updates blocked during Shopify fulfillment](issues/canada/shared/contact-update-source-of-truth.md) | Canada | SM, DV | Source-system update guidance confirmed by customer |
| [Recovering Canada label and packing-slip exceptions](issues/canada/shared/label-and-packing-slip-recovery.md) | Canada | SM, DV | Affected examples completed; cancellations separated |
| [Sales Summary dates missing from reporting](issues/canada/shared/missing-sales-summary-dates.md) | Canada | SM, DV | Source data reviewed and replacement CSVs supplied |
| [Canada feeds delayed by network processing issues](issues/canada/shared/network-related-feed-delay.md) | Canada | Country-wide; brands not itemized | Feeds processed and sent in the incident update |
| [Available-stock orders returned to preorder hold](issues/canada/shared/orders-returning-to-preorder.md) | Canada | SM, DV | October incident recovered; later manual holds distinguished |
| [Past-due unfillable orders did not auto-cancel](issues/canada/shared/past-due-auto-cancellations.md) | Canada | SM, DV | Listed orders cancelled after background processing refresh |
| [Recovering missing reconciliation report emails](issues/canada/shared/reconciliation-report-recovery.md) | Canada | Scope described in case | Historical reports supplied; targeted follow-up completed |
| [Wrong product imagery from a shared parent handle](issues/canada/sm/cross-shop-image-association.md) | Canada | SM | Immediate correction confirmed; permanent code fix planned |
| [Express shipping label failed under an incompatible service](issues/canada/sm/express-service-selection.md) | Canada | SM | Label generated; operating guidance acknowledged |
| [Mexico cancellations without Shopify refunds](issues/mexico/sm/cancellation-refund-sync.md) | Mexico | SM | Team-reported fix |
| [Fulfilled order import resolved to a virtual location](issues/mexico/sm/fulfilled-historical-order-import.md) | Mexico | SM | Import blocker identified; recovery route proposed |
| [POS customer number used an internal facility ID](issues/mexico/sm/internal-versus-external-customer-number.md) | Mexico | SM | Code path identified; permanent fix proposed |
| [PredictSpring send-sale feed failed required-field checks](issues/mexico/sm/send-sale-required-fields.md) | Mexico | SM | Field-level findings shared; retests requested |
| [Recovering a failed warehouse order upload](issues/mexico/sm/warehouse-order-upload-recovery.md) | Mexico | SM | Immediate recovery completed; recurring RCA open |
| [Inconsistent product names across operational reports](issues/shared/report-style-name-consistency.md) | Shared | SM | Incorrect output established; production cause unresolved |
| [Tracking synchronization and return processing recovery](issues/shared/tracking-and-return-sync.md) | Shared | SM, DV, KG | Resolved in follow-up; customer confirmation received |
| [Warehouse feed rejected for a blank carrier code](issues/usa/atm/blank-carrier-code.md) | Usa | ATM | Feed mapping updated; affected feeds regenerated |
| [Fully discounted ATM orders in downstream processing](issues/usa/atm/fully-discounted-order-validation.md) | Usa | ATM | M3 processing confirmed |
| [Inventory availability reduced by an item threshold](issues/usa/atm/inventory-threshold-removal.md) | Usa | ATM | Threshold removed; customer confirmed both systems |
| [Next Day orders imported as Standard](issues/usa/atm/next-day-import-mapping.md) | Usa | ATM | Configuration live; staging import confirmed |
| [BJ backorder styles routed into Unfillable](issues/usa/bj/backorder-to-unfillable-routing.md) | Usa | BJ | New-order configuration fixed; backlog correction underway |
| [Brokered BJ orders missing from reporting data](issues/usa/bj/brokered-orders-missing-from-report-table.md) | Usa | BJ | Recovery extract supplied; RCA open |
| [BJ inventory missing from the M3 source feed](issues/usa/bj/inventory-absent-from-upstream-files.md) | Usa | BJ | Upstream absence verified; replenishment confirmation requested |
| [Accessories unavailable despite open purchase orders](issues/usa/bj/overdue-accessory-purchase-orders.md) | Usa | BJ | Supply dependency identified; receipt pending |
| [BJ releases absent from the preorder report](issues/usa/bj/released-preorders-missing-records.md) | Usa | BJ | Data location explained; business classification open |
| [Completed DV order still visible in a store queue](issues/usa/dv/completed-order-still-in-progress.md) | Usa | DV | Open; earlier closure statement corrected |
| [Dolce Vita orders delayed in OMS import](issues/usa/dv/delayed-order-import.md) | Usa | DV | Reported backlog imported; recurring cause open |
| [Return records missing item details downstream](issues/usa/dv/incomplete-return-item-feeds.md) | Usa | DV | Examples reprocessed; further failures reported |
| [Physical return value and customer refund diverge](issues/usa/dv/return-versus-appeasement-value.md) | Usa | DV | Accounting contract unresolved |
| [Unexpected Shopify inventory adjustments attributed to SyncJobs](issues/usa/dv/unexpected-shopify-inventory-adjustments.md) | Usa | DV | External adjustment path under investigation |
| [Inventory missed after Shopify variant reassociation](issues/usa/dv/variant-reassociation-delta-sync.md) | Usa | DV | Inventory flow restored; customer confirmed |
| [Weekly shipped-units report used the wrong dates](issues/usa/dv/weekly-report-date-boundary.md) | Usa | DV | Corrected report delivered |
| [Orders stalled in Created across US brands](issues/usa/shared/created-order-backlog.md) | Usa | SM, DV, BJ | Reported backlog resolved; technical RCA unavailable |
| [Preorder update skipped before Shopify mapping existed](issues/usa/shared/preorder-mapping-created-after-event.md) | Usa | Brand scope unconfirmed | Targeted push reported in Codex discussion |
| [Displayed stock discrepancy remained after QOH explanation](issues/usa/shared/qoh-discrepancy-not-fully-explained.md) | Usa | Brand scope unconfirmed | Open; physical-count discrepancy still disputed |
| [Cancelled items remained in fulfillment queues](issues/usa/sm/cancelled-items-still-in-queue.md) | Usa | SM | Affected examples cleared; store confirmation received |
| [Duplicate order headers during overlapping import](issues/usa/sm/concurrent-order-creation.md) | Usa | SM | Race condition supported; exact creator unresolved |
| [Physical stock excluded by the selected inventory channel](issues/usa/sm/inventory-channel-exclusion.md) | Usa | SM | Channel-selection diagnosis; no resync performed |
| [Large allocation response failed database indexing](issues/usa/sm/large-allocation-audit-response.md) | Usa | SM | Allocator-side deployment reported; order brokered |
| [Changed product UPC blocked Fenix brokering](issues/usa/sm/old-upc-blocks-brokering.md) | Usa | SM | Orders brokered through a temporary upstream workaround |
| [Correcting an imported product style association](issues/usa/sm/style-association-correction.md) | Usa | SM | Style corrected; image correction pending |
| [KGCA English and French packing-slip updates](requirements/canada/kg/bilingual-packing-slips.md) | Canada | KG | Samples improved; French decimal-comma formatting pending |
| [KGCA report scheduling and reporting handover](requirements/canada/kg/kgca-report-scheduling.md) | Canada | KG | Delivered with an invoicing exception |
| [Exclude recalled facility supply from online preorders](requirements/canada/shared/exclude-recalled-preorder-supply.md) | Canada | SM, DV | DV change reported live; SM rollout still pending |
| [KGMX commerce setup](requirements/mexico/kg/kgmx-setup.md) | Mexico | KG | Completed — owner reported |
| [Mexico order-type change to stop automatic invoicing](requirements/mexico/shared/order-type-auto-invoicing.md) | Mexico | SM, DV | Production configuration and business confirmation recorded |
| [Mexico price and discount feed changes](requirements/mexico/sm/price-changes.md) | Mexico | SM, DV | Staging samples shared; final VAT treatment unresolved |
| [Preserve separate PO lines for different arrival dates](requirements/shared/split-purchase-order-lines.md) | Shared | Brand scope unconfirmed | Fresh-import UI validation recorded; rollout reported in call notes |
| [ATM warehouse and shipping-item feed mapping](requirements/usa/atm/financial-feed-field-mapping.md) | Usa | ATM | Samples delivered; field semantics clarified |
| [Stylux digital item feed integration](requirements/usa/dv/stylux-integration.md) | Usa | DV | Feed format accepted; downstream validation coordinated |
| [Order and return feed validation for GraphQL migration](requirements/usa/shared/graphql-feed-validation.md) | Usa | SM | Test scenarios and UAT data prepared; downstream review requested |
| [Narvar shipping protection feed handling](requirements/usa/shared/narvar-shipping-protection.md) | Usa | SM, DV, BJ | Samples shared; location semantics under review |
| [Send-sale shipping charges and tax in outbound feeds](requirements/usa/shared/send-sale-shipping-charge.md) | Usa | SM | Staging feeds reviewed; production move requested |
| [Brand and date aware shipped-units reporting](requirements/usa/shared/shipped-units-dashboard.md) | Usa | SM, DV, ATM | Reports delivered; dashboard permissions updated |
| [TikTok fulfillment and shipping-feed changes](requirements/usa/shared/tiktok-shipping.md) | Usa | DV | DVUS staging approach agreed; implementation unverified |

## Reading the record

Each new case separates the issue, expected behavior, RCA, documented actions, outcome, and recommended validation. Earlier cases retain their implementation narrative and explicit RCA/action additions. Proposed checks are not claimed as executed. An open RCA remains open even when a particular order or feed was recovered.

Personal contributions, customer confirmations, and team implementations retain their separate attribution. Cases with unknown brand scope are labelled accordingly. This is a curated record, not automatic mailbox monitoring.

Use the [case template](templates/case-study.md) and [contribution guide](CONTRIBUTING.md) for future additions. Routine employee creation and administrative provisioning are excluded.

This personal portfolio is independently prepared and unaffiliated with the brands. Raw mail, production payloads, credentials, and private customer/contact details are excluded.
