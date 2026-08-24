---
name: linkedin-trend-scan
description: Surfaces what is currently performing in-niche on LinkedIn. Use before generating new content ideas, or when an idea backlog feels stale, to feed real timing and topic signal upstream into idea-review and idea-tournament. Not for drafting copy — trigger on requests like "what's working on LinkedIn right now for this niche" or "scan for LinkedIn trends before we brainstorm."
---

# LinkedIn Trend Scan

Scans the current LinkedIn landscape in a given niche and returns what's actually performing right now, as research input — not copy.

## When to use

Use this at the research stage, upstream of [[idea-review]] and [[idea-tournament]] — its output is signal for deciding what to pitch as an idea, not a post to publish. Run it before a brainstorm, or periodically to keep an idea backlog current. It does not draft posts; hand anything promising to the idea pipeline first, then [[linkedin-copywriter]] once an idea is approved.

## Inputs needed

- **Niche or topic area** — or a specific list of peer/competitor accounts to benchmark against
- **Time window** — defaults to the last 7–14 days if not specified; narrow it for fast-moving topics
- **Optional**: specific handles to prioritize, or handles to exclude (e.g., accounts too large to be a realistic comparison)

## What counts as a trend

A signal only clears the bar if one of these is true:

- A post from a comparably sized or larger in-niche account, published within the window, with engagement meaningfully above that account's own baseline (roughly 3x+ their typical median) — not just high engagement in absolute terms
- The same topic or angle appears independently across 3+ unrelated accounts within the window (independent convergence is a stronger signal than one viral post)

Weight comment quality over like count — likes are cheap and easily inflated by algorithmic reach; genuine debate or disagreement in the comments is a stronger trend signal than uniform agreement. Exclude pure engagement-bait formats with no topical content ("Agree?" / "Repost if you..."), and exclude anything whose reach is plausibly explained by follower count alone rather than the content itself.

Classify each signal as one of:
- **Format trend** — a structure being copied across accounts (e.g., a specific carousel style, a "story then lesson" arc)
- **Topic trend** — a subject getting sustained attention regardless of format
- **Moment trend** — tied to news or an event; short shelf life, note the expiry

## Output format

A ranked list of 3–7 trend signals. For each:
1. What's trending and its classification (format / topic / moment)
2. 1–2 example posts or accounts as evidence
3. The specific signal that clears the bar (which threshold above it met)
4. Shelf-life estimate — roughly how many days this stays relevant

This list is meant to be handed directly to [[idea-review]] or [[idea-tournament]] as input, not published as-is.
