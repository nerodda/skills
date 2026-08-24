---
name: lead-magnet-engager
description: Drafts the nurture email sequence that follows a lead magnet download — warm, opt-in-based outreach to someone who already raised their hand. Use once a lead magnet asset exists and it's time to write what happens after someone downloads it. Trigger on requests like "write the nurture sequence for this lead magnet" or "what should we email people after they download this." Not for building the asset itself — that's [[lead-magnet-creator]] — and not for cold outbound, which is [[outbound-copywriter]].
---

# Lead Magnet Engager

Drafts the nurture email sequence that runs after someone downloads a lead magnet — warm follow-up to a person who already opted in, not the asset itself and not cold outreach.

## When to use

Use this downstream of [[lead-magnet-creator]], once the asset exists and is live behind an opt-in. This skill never touches the asset — it only writes what happens in the inbox afterward. It's distinct from [[outbound-copywriter]] on temperature: this sequence goes to someone who already raised their hand by downloading something, so it opens warm and delivers value before it ever asks for anything. Outbound sequences open cold, to someone who has taken no action yet.

## Inputs needed

Before drafting, confirm:
- **The lead magnet itself** — what it is and what outcome it promised, so the sequence delivers on that promise rather than drifting to a different pitch
- **The next desired action** — what happens after the sequence: a sales call, a trial signup, a second content offer, etc.
- **Sequence length** — how many emails (if unset, default to 4–5: deliver, deepen, prove, offer, close)
- **Sender voice/persona** — who the emails are from, so tone matches how that person actually writes

If the next desired action is missing, ask — a nurture sequence with no destination just decays into content with no purpose.

## Sequence structure

Default to this arc unless the inputs call for something shorter:

1. **Delivery** — hands over the asset (or confirms it's already delivered) and sets one expectation for what's coming next in the sequence.
2. **Deepen** — expands on one specific piece of the asset with added value, not a rehash of what they already have.
3. **Proof** — a case study, result, or credibility point relevant to the problem the lead magnet addressed.
4. **Offer** — introduces the next step (the paid product, the call, the trial) tied directly back to the outcome the lead magnet promised.
5. **Close** — a direct, low-friction ask with a clear deadline or reason to act now, plus a graceful out for those not ready.

Rules:
- Every email must reference the specific lead magnet by name or topic in the first two lines — a generic nurture sequence that could follow any download isn't doing its job.
- Never ask for anything in email 1. The first touch is pure delivery and trust-building.
- Escalate the ask gradually — each email can be slightly more direct than the last, but the jump from email to email should never feel like a hard pivot.
- If the sequence runs past 5 emails, each additional email needs its own distinct value angle — don't pad with repetition of the offer.

## Output format

The full sequence, email by email, each with:
- Subject line
- Body copy
- One-line note on the specific action or reference that ties it back to the lead magnet

Number the emails in send order and note the recommended send cadence (e.g., day 0, day 2, day 5) between them.
