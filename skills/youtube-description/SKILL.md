---
name: youtube-description
description: "Writes a video's description block — the SEO description, timestamped chapters, and links block — once a final edit exists and timestamps are locked. Use after editing is finished and before final packaging. Trigger on 'write the description for this video,' 'give me chapters for this,' or 'draft the links block.' Not for the video's title or thumbnail (parallel skills) and not for final upload assembly."
---

# YouTube Description

Writes the full description block for a video: the search-facing opening lines, timestamped chapters, and the links block, in one paste-ready piece of copy.

## When to use

Use only after the final edit exists and its timestamps are locked — chapters need real, unshifting timecodes, so writing this before editing is finished means redoing it. This runs after [[youtube-title]] and [[youtube-thumbnail]] (or in parallel, once the edit is locked, since it doesn't depend on which title/thumbnail wins) and feeds directly into [[youtube-publisher]] for final assembly. It's metadata content in its own right — not visual packaging like title/thumbnail, and not the assembly check itself.

## Inputs needed

- **Final edited video** — locked runtime and timestamps; chapters written against an edit that might still change are wasted work
- **Target keywords** — for search and "suggested video" matching; the first 1–2 sentences carry the most SEO weight
- **Links to include** — website, related videos/playlists, socials, lead magnet or offer, with priority order
- **Required disclosures** — sponsor, affiliate, or legal language that must appear, and where it's required to appear

## Structure and rules

**Opening (first 1–2 sentences):**
- Must work standalone — this is what shows before the "...more" cutoff and what search/suggested-video surfaces pull from
- Keyword-rich but written as a sentence, not a keyword list
- Should function like a hook: state what the viewer gets, not a vague summary

**Chapters:**
- Must start at `0:00` — YouTube requires this to register chapters at all
- Minimum 3 chapters, each spanning at least 10 seconds
- Label by content, not by structure — "Why this breaks at scale" beats "Part 2," and "Intro" is never an acceptable label
- Chapters must match the final edit's actual timestamps exactly — don't estimate

**Links block:**
- Ordered by priority — the primary CTA (whatever [[youtube-publisher]] will treat as the main ask) goes first, not buried under socials
- Every link labeled with what it is, not a bare URL

**Hashtags:**
- Maximum 3 — YouTube shows the first 3 above the title, more than 3 adds clutter with no added benefit

## Output format

Return the full description as one paste-ready block, in this order:
1. Opening hook lines (1–2 sentences)
2. Full body copy, if the format calls for more than the opening
3. Chapters list with timestamps
4. Links block, priority-ordered
5. Hashtags (up to 3)
6. Any required disclosure text, placed where required
