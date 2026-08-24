---
name: youtube-title
description: "Generates and ranks a set of title variants for a video against a click-through framework — run alongside [[youtube-thumbnail]] since the two are tested as a pair, not written sequentially. Use once a final edit (or a locked outline) exists and it's time to package the video. Trigger on 'give me title options for this video,' 'rank these YouTube titles,' or 'what should we call this video.' Not for drafting thumbnail concepts and not for the SEO description."
---

# YouTube Title

Generates a spread of title variants across distinct angles, scores each against a fixed click-through framework, and returns a ranked shortlist — instead of one title picked by gut feel.

## When to use

Sibling skill to [[youtube-thumbnail]]: both run late in the pipeline, once the video (or a locked outline with a known payoff) exists, and both feed [[youtube-publisher]]. They're paired, not sequential — title variants shouldn't be written to match a thumbnail already locked in, and vice versa; generate both independently, then check the winning combination for consistency at assembly. Not the place to write SEO copy for the description — that's [[youtube-description]], which has looser length constraints and different goals (search matching, not click-through).

## Inputs needed

- **The video's actual content/payoff** — what happens in it, stated plainly, so titles can be checked against reality
- **Target keyword(s)** — if this video is meant to rank in search or suggested video, not every video needs this
- **Channel's existing title conventions** — house voice, whether numbers/brackets/emoji are used, past titles that performed well
- **Length constraint** — YouTube truncates around 60 characters on desktop search/suggested, less on mobile

## Titling framework

Generate 8 variants spread across these angles — don't cluster all 8 around one angle:

1. **Curiosity gap** — opens a loop without lying about the payoff
2. **Number / list** — a count framing ("3 ways," "the one thing")
3. **How-to / direct benefit** — states the outcome plainly
4. **Contrarian / bold claim** — challenges a common assumption
5. **Question** — poses the question the video answers
6. **Result-first** — leads with a specific, real metric or outcome

(Angles 1–6 map to 8 variants because some angles are worth two takes; don't force exactly one variant per angle if one angle clearly fits the video better.)

Score each variant 1–5 on four criteria:

- **Clarity** — can a stranger tell what this video is about from the title alone?
- **Curiosity gap** — does it open a loop, without being false to the content? (A maxed-out curiosity score paired with a low promise-payoff match is a red flag, not a win.)
- **Keyword presence** — does it contain the target keyword(s) naturally, if any are set?
- **Length fit** — does it read fully before truncation (~60 characters, with the first ~40 the most important for mobile)?

Additionally, flag (pass/fail, not scored) **promise-payoff match**: does the title claim something the video actually delivers? A variant that fails this is disqualified regardless of score — it's not a ranking problem, it's a bait problem.

## Output format

1. **Table** of all 8 variants with per-criterion scores and a total
2. **Top 3** recommended for testing, each with one line on why it ranked where it did
3. **Disqualified variants**, if any, with the promise-payoff issue named explicitly
