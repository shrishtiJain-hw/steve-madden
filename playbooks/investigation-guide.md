# Commerce incident investigation guide

These are proposed investigation methods drawn from the documented cases. They are not a record of production actions already executed.

| Symptom | First checks | Recovery acceptance |
| --- | --- | --- |
| Missing order | Source identity, import queue age, existing OMS order/history, approval state | One canonical order, correct state, no repeated inventory issuance |
| Inventory mismatch | Product mapping, source stock, channel eligibility, delta timestamp, outbound publisher | Expected OMS availability and matching downstream stock |
| Unbrokered order | Current and historical UPC, allocator response, eligible locations, audit persistence | Valid allocation with traceable request/response |
| Label failure | Order state, address/contact source, service mapping, existing label | One usable label and correct tracking |
| Financial-feed mismatch | Event type, cash refund, physical stock return, mapping version, processing window | Source and destination reconcile without duplicate cash or stock effects |
| Missing report | Eligible source rows, business date, job SQL, generated export, downstream ingestion, email delivery | Required period and records visible to the consumer |

## Closure record

Record the observed failure, confirmed cause or remaining hypotheses, action owner, actual recovery step, and independent acceptance evidence. Distinguish a customer-confirmed immediate fix from a planned permanent change. A successful resend does not establish the recurring root cause.
