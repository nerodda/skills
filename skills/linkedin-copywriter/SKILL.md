---
name: linkedin-copywriter
description: Drafts a LinkedIn post from a brief, in the account's voice. Use once a brief exists (from proposal-creator, repurpose, or researcher) and the idea has already cleared idea-review — not for generating the idea itself, and not for writing just the opening line. Trigger on requests like "write the LinkedIn post for this," "draft this brief as a LinkedIn post," or "turn this into a LinkedIn post."
---

# LinkedIn Copywriter

Turns a brief into a publish-ready LinkedIn post in the account's established voice — full structure, full body, ready to paste.

## When to use

Use this mid-pipeline: after a brief exists (from [[proposal-creator]], [[repurpose]], or [[researcher]]) and the idea has cleared [[idea-review]] or [[idea-tournament]], before [[taste-filter]] or [[ship-scan]]. If an opening line has already been chosen via [[linkedin-hook-writer]], use it as the post's first line rather than writing a new one. This is the LinkedIn-specific counterpart to [[x-copywriter]] — don't reuse LinkedIn output for X or vice versa; the platforms have different structural and tonal defaults.

## Inputs needed

- **The brief** — topic, angle, key points to hit, and any CTA
- **Voice/tone reference** — the account's past posts, or a voice doc, to match rhythm and vocabulary
- **Chosen hook** (optional) — if [[linkedin-hook-writer]] already produced one; otherwise write the opening line as part of the draft
- **Post type** — single narrative post vs. list/breakdown structure, if the brief doesn't make it obvious

If voice reference is thin or absent, say so before drafting — a post with no voice signal to match is a generic post, and that should be flagged, not silently produced.

## Voice and structure rules

- **Shape**: hook (1–2 lines) → line break → body in short paragraphs (1–3 sentences each, generous white space) → optional numbered/bulleted breakdown if the content is a list → closing line.
- **Register**: first person, opinionated, can be narrative or story-driven. Professional-adjacent, not corporate — LinkedIn tolerates a confident point of view that a press release wouldn't.
- **Length**: 150–300 words is the default range; up to ~600 words is fine for narrative or case-study posts. LinkedIn readers tolerate long-form in a way X readers don't — don't artificially compress a post that earns its length.
- **One idea per post.** If the brief contains two ideas, flag it and ask which one this post is actually about rather than cramming both in.
- **Closing line**: end on a question, a stated POV, or a soft CTA. Never a hard sell or an engagement-bait "thoughts?" tacked on with no connection to the body.
- **Hashtags**: 0–3 max, only if genuinely on-topic. Never stuff for reach.
- Match the voice reference's actual sentence rhythm and vocabulary — don't default to generic LinkedIn-guru cadence ("Here's the thing:" / "Let that sink in.") unless the account's own voice actually sounds like that.

## Output format

Return:
1. The full post text, ready to paste, with line breaks as they should appear
2. Word count and estimated character count
3. One line noting any assumptions made (which hook was used, how tone was calibrated, what was cut to keep it to one idea)
