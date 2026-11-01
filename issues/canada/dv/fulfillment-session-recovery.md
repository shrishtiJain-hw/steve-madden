# DV store could not complete shipping from fulfillment

**Country:** Canada\
**Brands:** DV\
**Status:** Customer confirmed recovery after session refresh\
**Contribution:** Investigation, validation, and stakeholder coordination

## Issue and business impact

Store fulfillment users could not ship packed orders through their current application session.

## Expected behavior and requirement

A valid fulfillment session should expose the current permissions and allow eligible packed orders to ship.

## RCA and evidence

The team reported the issue fixed and the final successful recovery used a complete logout followed by Launchpad sign-in. The thread does not establish whether stale authentication, cached permissions, or another session problem was the underlying defect.

## Documented actions

1. I reported the issue resolved and documented that most of the affected packed orders had been processed.
2. I asked the store to log out of all HotWax apps, sign in through Launchpad, and reopen Fulfillment.
3. The store confirmed that the workflow worked after those steps.

## Outcome and remaining work

The user workflow was restored. The initial message still distinguished processed orders from remaining examples; it did not establish a new root cause for every order.

## Recommended validation and prevention

The following checks are proposed follow-up guidance unless explicitly confirmed above.

- Retest the remaining packed orders after session refresh.
- Verify current role and store association without sharing credentials.
- Record whether a fresh session resolves recurrence.

## Evidence basis

My October 11–12 messages and the store confirmation in “DV73 - E-COMM INCONVENIENCE.”
