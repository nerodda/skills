---
name: x-trend-scan
description: Surfaces what is currently performing in-niche on X. Use before generating new content ideas, or when an idea backlog feels stale, to feed timing and topic signal upstream into idea-review and idea-tournament — the X analog of linkedin-trend-scan, tuned to X's faster cycle and different engagement signals. Not for drafting copy — trigger on "what's working on X right now" or "scan X for trends before we brainstorm."
---

# X Trend Scan

Scans the current X landscape in a given niche and returns what's actually performing right now, as research input — not copy.

## When to use

Use this at the research stage, upstream of [[idea-review]] and [[idea-tournament]], the same slot as [[linkedin-trend-scan]] but scoped to X. Its output is signal for what to pitch as an idea, not something to publish. Run it before a brainstorm, or periodically to keep the idea backlog current. Hand any promising signal to the idea pipeline first, then to [[x-copywriter]] once an idea is approved — this skill never drafts posts.

## Inputs needed

- **Niche or topic area** — or a specific list of peer/competitor accounts to benchmark against
- **Time window** — defaults to the last 3–7 days; X's cycle moves faster than LinkedIn's, so a 14-day window is usually too stale to be useful
- **Optional**: specific handles to prioritize or exclude

## What counts as a trend

X's engagement mechanics differ from LinkedIn's, so the bar is defined differently:

- A post from a comparably sized or larger in-niche account, published within the window, with quote-tweet and reply volume meaningfully above that account's own baseline (roughly 3x+ median) — weight quote-tweets and replies over raw likes/reposts, which are cheaper to accumulate and more exposed to bot amplification
- The same topic or angle appears independently across 3+ unrelated accounts within the window
- Genuine disagreement or debate in the replies is a stronger signal than uniform agreement — a post everyone quietly likes is weaker signal than one people are actively arguing about

Sanity-check virality before counting it: a spike driven by a small number of large accounts reposting, or a pattern consistent with bot amplification (near-identical low-effort replies, engagement with no account history), doesn't clear the bar even if the raw numbers look large.

Classify each signal as one of:
- **Format trend** — a structure being copied (e.g., a specific thread opener style, a screenshot-plus-take format)
- **Topic trend** — a subject getting sustained attention regardless of format
- **Moment trend** — tied to news or an event; shortest shelf life of the three on X, often hours to a couple of days rather than weeks

## Output format

A ranked list of 3–7 trend signals. For each:
1. What's trending and its classification (format / topic / moment)
2. 1–2 example posts or accounts as evidence
3. The specific signal that clears the bar
4. Shelf-life estimate — realistic for X's faster cycle, often measured in days or even hours for moment trends

This list is meant to be handed directly to [[idea-review]] or [[idea-tournament]] as input, not published as-is.
