---
name: results-scan
description: Pulls performance data on published content back into the pipeline. Use periodically — weekly, or after a launch push — once content has been live long enough to have real numbers, to score what worked and feed decisions back into idea-review, idea-tournament, or split-test-designer. Trigger on requests like "how did last week's posts do," "pull results from the launch," or "what should we do more of." Not the pre-publish check on a single piece — that's ship-scan.
---

# Results Scan

Pulls performance data on already-published content and turns it into concrete pipeline decisions — what to repeat, what to stop, what's worth testing — closing the loop back to idea scoring.

## When to use

This is the loop-back step, run periodically (weekly, monthly, or after a launch push) rather than per-piece. Comes after publish and has nothing to do with pre-publish gates like [[taste-filter]] or [[ship-scan]]. Feeds its findings into [[idea-review]] and [[idea-tournament]] to inform how future ideas get scored, and into [[split-test-designer]] when a finding is worth structuring into a deliberate test rather than just a hunch.

## Inputs needed

- **Published pieces in scope** — URLs/IDs and publish dates
- **Platform analytics pull** — views, engagement rate, CTR, replies/comments, saves/shares, conversions, whichever apply to the channel
- **Comparison baseline** — account average, prior period, or a specific benchmark to measure against
- **The original angle/hook/idea behind each piece** — needed to reconnect a result back to the pipeline decision that produced it

## Process

- Normalize metrics per channel before comparing — a "good" LinkedIn post and a "good" newsletter aren't the same numbers.
- Compare each piece against its own channel's baseline, never across channels.
- Separate reach, engagement, and conversion metrics — a piece can win on one and lose on another; don't collapse them into one score.
- Look for the pattern behind winners and losers — angle, hook, format, timing, length — not just "this one did well."
- Flag statistically thin data (low sample size, short time live) instead of drawing a conclusion from noise.
- Tie every finding to a decision: what should repeat, what should stop, what's worth a deliberate split test.

## Output format

1. **Table** — piece / channel / key metric(s) / vs. baseline (+/-%)
2. **Top and bottom performers**, each with the likely reason why (angle, hook, format, timing)
3. **Patterns worth repeating** — flagged for idea-review to weight in future scoring
4. **Patterns worth testing** — flagged for split-test-designer
5. **Inconclusive results**, named as such rather than forced into a story
