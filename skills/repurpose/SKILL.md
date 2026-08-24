---
name: repurpose
description: Breaks one finished long-form piece into channel-specific derivatives — extracted angles, hooks, and excerpts ready to hand to each channel's drafting skill. Use once a long-form piece or case study is finished and needs to seed content for LinkedIn, X, YouTube, or other channels. Trigger on requests like "repurpose this piece," "what can we get out of this article," or "turn this into a content batch." Not a final-draft skill for any single channel — it selects and extracts, the channel skills do the platform-native writing.
---

# Repurpose

Takes one finished long-form piece and derives a set of channel-specific angles, excerpts, and briefs — the raw material each channel's own drafting skill turns into a final, platform-native post.

## When to use

Use this once a piece from [[long-form]] (or any other finished long-form asset — a case study, a transcript) is published or ready to publish, and it's time to extract what can be built from it for other channels. This is the extraction/angle-selection step, not the final draft — its output feeds into [[linkedin-copywriter]], [[x-copywriter]], [[youtube-script]], and similar channel skills as their brief or source material. Don't use this to write the LinkedIn post or the tweet directly; if the source piece doesn't exist yet, run [[long-form]] first.

## Inputs needed

Before deriving, confirm:
- **The source piece** — the finished long-form article or asset, in full
- **Target channels** — which channels to derive for (LinkedIn, X, YouTube, etc.); don't derive for every possible channel by default if only some are wanted
- **Quota per channel**, if there's a house convention (e.g., "3 LinkedIn angles, 5 tweetable lines") — otherwise derive as many strong candidates as the source supports, not a padded fixed number

## Derivation method, per channel

For each target channel, extract rather than compress — find what's already sharp in the source instead of summarizing the whole piece down to fit.

- **LinkedIn** — pull 2–4 standalone angles: a strong claim, a contrarian take, a concrete result, or a lesson learned, each specific enough to open a post on its own. Include the supporting detail/quote from the source that backs it. Hand off to [[linkedin-copywriter]] (and [[linkedin-hook-writer]] if hooks need separate treatment).
- **X** — pull the most quotable, self-contained lines or stats — sentences that already read as a tweet without editing, or numbers striking enough to stand alone. Hand off to [[x-copywriter]].
- **YouTube** — identify whether the piece supports a full script treatment (a narrative or teachable arc) or just a topic/outline seed; extract the core narrative beats or teaching points in order. Hand off to [[youtube-script]].
- **Newsletter** — if a newsletter recap is wanted, extract the 3–5 most newsletter-relevant points, not the full argument; hand off to [[newsletter-writer]] rather than drafting the issue here.

For every channel, note which specific passage or data point in the source each derivative comes from — a channel skill working from a vague paraphrase drifts from the source; one working from a cited excerpt won't.

## Output format

Per requested channel: a labeled list of derived angles/excerpts, each with the source passage it's drawn from and a one-line note on why it works for that channel. This is a handoff document for the channel skills, not a finished post in any format.
