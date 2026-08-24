---
name: taste-filter
description: Screens a draft against a house style bar and rejects the generic ones. Use once a draft exists — from long-form, newsletter-writer, linkedin-copywriter, x-copywriter, or similar — and before it goes to ship-scan, to check voice, specificity, and whether the piece sounds like anyone could have written it. Trigger on requests like "does this sound like us," "taste-check this draft," or "is this too generic." Not a mechanical check — for broken links, missing assets, and metadata, use ship-scan instead.
---

# Taste Filter

Screens a finished draft against a house voice-and-specificity bar and returns a verdict, so generic-sounding content gets caught before it reaches the mechanical pre-publish gate.

## When to use

Sits between a finished draft — from [[long-form]], [[newsletter-writer]], [[linkedin-copywriter]], [[x-copywriter]], or any other drafting skill — and [[ship-scan]]. Run it once the piece is written but before the final mechanical check: a piece can pass every ship-scan item and still be generic, and that's exactly what this catches. Don't use it for links, formatting, or metadata — that's ship-scan's job.

## Inputs needed

- **The draft**, in full
- **House style reference** — examples of past pieces that landed, or a written style guide if one exists
- **Channel/format** — the voice bar differs by channel; a LinkedIn post and a newsletter aren't held to the same line-level standard

## Rubric

Score on two independent axes, 1–5 each.

### Voice fit (1–5)
Does this sound like this specific person or brand, or could it have come from any account in the niche?
- **5** — Distinct voice throughout; specific phrasing choices that are recognizably "ours."
- **3** — Readable and on-topic, but voice fades in and out.
- **1** — Could be swapped into a competitor's feed with a find-and-replace on the name.

### Specificity (1–5)
Does it say something concrete, or does it float at the level of generic advice?
- **5** — Concrete examples, numbers, named tools/people/situations.
- **3** — Mostly concrete with a few generic filler lines.
- **1** — Reads like it was assembled from platitudes — no real specifics anywhere.

### Banned patterns (hard fail regardless of score)
Flag and reject on sight:
- Hollow openers — "In today's fast-paced world...", "Let's dive in..."
- The "it's not just X, it's Y" crutch used more than once
- Empty superlatives — "game-changer," "unlock," "revolutionize" — without a concrete claim backing them
- Rhetorical-question hooks with no real answer coming ("Ever wonder why...?")
- Any AI-listicle tell: uniform three-part parallel structure with no variation in rhythm

## Verdict bar

Combined score = Voice fit + Specificity (max 10).

- **8–10 → Pass.** Send to ship-scan. Note the combined score in one line.
- **5–7 → Rework.** Name the weaker axis and what to cut or sharpen — quote the generic lines directly.
- **2–4 → Reject.** Send back to the drafting skill; this needs a different approach, not a line edit.

A banned pattern in the opening line is an automatic fail on Voice fit regardless of the rest of the score — fix the hook before anything else.

## Output format

1. Voice fit score + one-line reasoning with a quoted example
2. Specificity score + one-line reasoning with a quoted example
3. Combined score
4. Banned patterns caught, quoted directly
5. Verdict (Pass / Rework / Reject) with the one biggest thing to fix
