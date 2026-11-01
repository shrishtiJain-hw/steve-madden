# Maintaining the portfolio

Add a case when it documents a meaningful requirement, implementation, recovery, or technical investigation. Use requirements/<country>/<brand>/ for requested capabilities and issues/<country>/<brand>/ for incidents. USA supports SM, DV, BJ, ATM; Canada and Mexico support SM, DV, KG. Use a country-level shared/ folder for cases covering multiple brands or awaiting brand confirmation, and issues/shared/ for explicitly cross-country cases. Record the scope of each case; do not infer applicability from the country matrix.

Describe personal contribution separately from team findings. Keep requirement received, validation shared, accepted, deployed, recovered, and permanently resolved as distinct states. A resend may restore one order while recurring RCA remains open.

Summarize business behavior in your own words. Keep raw mail, customer/order identifiers, contact information, access details, internal URLs, and proprietary payloads outside Git. Do not attach mailbox exports or screenshots containing production details.

Add the case to README.md and catalog.json. Put the evidence basis in the case without exposing private message links. Record proposed checks as proposals, and claim successful execution only when a result exists.

Routine employee setup, account provisioning, reminders, and unresolved requests without substantive analysis do not belong in the issue portfolio. Requirements may be included before implementation when their status is explicit.
