---
name: linkedin-hook-writer
description: Generates opening-line variants built to stop the scroll on LinkedIn. Use once a post's angle is set but the first line needs options — this feeds into linkedin-copywriter, it does not draft the rest of the post. Trigger on requests like "give me some hooks for this," "I need a stronger opening line," or "write hook options for this LinkedIn post."
---

# LinkedIn Hook Writer

Generates a set of opening-line variants for a single LinkedIn post — the 1–3 lines shown before the "see more" fold — so the post starts with the strongest possible option instead of whatever came out first.

## When to use

Use this narrowly: only the opening line(s), never the body. It sits between an idea/angle being set and [[linkedin-copywriter]] drafting the full post — feed the chosen hook into that skill rather than writing the post here. Can also run standalone against an existing draft when only the opener needs replacing. Not for X — hooks there are governed by [[x-copywriter]] directly, since X posts don't have a fold to write toward.

## Inputs needed

- **The post's core idea or angle** — or the full draft, if swapping in a better opener on existing copy
- **Audience/ICP** — who this needs to stop mid-scroll
- **Hooks to avoid** — archetypes or exact lines used recently, so variants don't repeat a format the audience has already seen from this account

## Hook taxonomy

Pull from at least three of these archetypes per batch — don't generate eight variations on one archetype:

- **Contrarian claim** — states the opposite of common advice. ("Everyone tells you to post daily. That's why most accounts plateau.")
- **Confession / vulnerability** — admits a mistake or blind spot plainly. ("I got this wrong for three years.")
- **Specific number or result** — a concrete, unhedged figure. ("We went from 12 to 4,000 in 90 days.")
- **Direct question** — asks something the reader has actually wondered, not a rhetorical filler question.
- **Pattern interrupt** — an unexpected or out-of-register first line that breaks the scroll rhythm.
- **Story cold-open** — drops into a scene mid-action, no throat-clearing setup.
- **List tease** — promises a specific count of things. ("3 things nobody tells you about onboarding.")

## Rules

- Generate 5–8 variants per request, spanning at least 3 different archetypes.
- Each variant must stand alone — no "and then..." lines that depend on the next sentence to make sense.
- Keep each hook within what LinkedIn actually shows before the fold: roughly 3 lines / ~210 characters. A hook that gets truncated mid-thought fails regardless of how strong the line is.
- No question-only hooks that could apply to any post in the niche ("Ever wonder why X matters?") — specificity is the bar, not just interrogative phrasing.
- Don't pad the count with near-duplicates of the same line reworded — each variant should force a genuinely different read of the post.

## Output format

A numbered list of hook variants, each labeled with its archetype. Close with one line naming the strongest variant and the specific reason it's strongest (not just "this one feels punchier").
