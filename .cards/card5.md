**Goal:** Decide and confirm what's needed to send the 6 drafted outreach emails (Mountain Burrito, Ono Poke Bowl, McCabe's Tire, Morganton Hemp, Alexander Brooke Boutique, Glambeauty) — this is a decision + a couple clicks, not a build.

**Time:** 15 minutes

**Reward:** Gold star + unblocks 6 more prospects with zero extra writing (emails are already drafted).

## Background

The email templates are already written. A previous send batch (24 emails, 2026-07-17) already proved the Gmail credentials work. This card is just about confirming and sending these 6 specific ones.

## Steps

1. Open `OmniTender/docs/operations/outreach-tracker.md` and `OmniTender/docs/operations/revenue-sprint-checklist.md` to see the current state.
2. Confirm the Gmail credential (`GMAIL_USER`/`GMAIL_APP_PASSWORD`) is still valid — ask whoever set it up if unsure, or just try a dry run (see below).
3. On your machine: `cd` into OmniVerse, run `DRY_RUN=1 node scripts/send-campaign.js` to preview subject lines — confirm it doesn't error.
4. If the dry run looks right, decide: fold these 6 into a bulk send, or send by hand (they have vertical-specific angles that don't match the generic template — sending by hand may work better).
5. Once you decide to send for real: `$env:LIMIT='6'; node scripts/send-campaign.js` (PowerShell).
6. Update `outreach-tracker.md`: mark these 6 as "Contacted", today's date, channel "Email".

## When You're Done

Comment "Done ✅" — note whether you sent via the bulk script or by hand. Close this card.

**Note:** This is Daniel's decision + action (needs email access) — assign to Daniel or whoever has the Gmail credential.
