---
name: outbound-copywriter
description: Drafts cold outbound sequences from an offer and an ICP — first-touch emails or LinkedIn messages to people who haven't opted into anything. Use when there's an offer and a defined target audience and the ask is to write the cold sequence that opens the conversation. Trigger on requests like "write a cold email sequence for X," "draft outbound copy for this ICP," or "we need a sequence to open cold." Distinct from [[lead-magnet-engager]], which nurtures someone who already downloaded something — this is unsolicited, cold contact.
---

# Outbound Copywriter

Drafts a cold outbound sequence — email or LinkedIn — from an offer and an ICP, for people who haven't taken any prior action and don't know the sender.

## When to use

Use this when the contact has taken no prior action — no download, no opt-in, no inbound signal. That's the line that separates this from [[lead-magnet-engager]]: this skill writes cold, unsolicited first contact; lead-magnet-engager writes warm follow-up to someone who already raised their hand. If a split test is needed on this sequence's messaging, hand the variant design to [[split-test-designer]] rather than guessing at what to test.

## Inputs needed

Before drafting, confirm:
- **The offer** — what's being sold or proposed, stated concretely enough to fit in one sentence
- **The ICP** — role, company profile, and the specific pain or trigger that makes this offer relevant to them right now
- **Channel** — email, LinkedIn, or both (structure and length differ)
- **Sequence length** — how many touches (default to 4 if unset: open, value-add, proof, breakup)
- **Any known personalization data** — company detail, recent trigger event, mutual connection, etc., if available

If the ICP is vague ("marketers" with no further detail), push back and ask for the specific role and trigger — generic ICP targeting produces generic copy that reads as spam.

## Sequence structure

Default arc, adjust touch count to the input:

1. **Open** — one specific, personalized reason this person/company is being contacted, followed by a single clear ask (a reply, not a meeting, on touch one). No pitch deck in the first message.
2. **Value-add** — a useful insight, resource, or observation relevant to their situation, with a soft reference back to the original reason for outreach.
3. **Proof** — a specific result or case study relevant to their industry or role, tied to the pain named in the ICP.
4. **Breakup** — a short, low-pressure final touch that makes it easy to say no and leaves the door open, not a guilt-trip.

ICP-personalization rules:
- Every touch must reference something specific to the recipient's role, company, or situation in the first line — not just their name inserted into a template.
- Never open with "I noticed you..." as a generic filler; the noticed detail must be real and specific to this ICP segment.
- Keep each message short enough to read on a phone in under 15 seconds — cold outbound is a scan, not a read.
- Match tone to channel: LinkedIn messages read more casual and shorter than cold email; don't reuse identical copy across both without adjusting.

## Output format

The full sequence, touch by touch, each with:
- Channel (email/LinkedIn)
- Subject line (if email)
- Body copy
- The specific personalization variable each touch depends on (so it's clear what data is needed to actually send it)

Note the recommended cadence between touches (e.g., day 0, day 3, day 7, day 12).
