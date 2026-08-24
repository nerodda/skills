---
name: youtube-thumbnail
description: "Drafts thumbnail concepts and text treatments for a video, generating several distinct visual directions to test — run alongside [[youtube-title]] since thumbnail and title are evaluated as a pair for click-through, not sequentially. Use once a final edit (or a locked outline) exists and it's time to package the video for the feed. Trigger on 'give me thumbnail ideas for this video,' 'what should the thumbnail say,' or 'draft thumbnail concepts.' Not for picking the title and not for writing the video's content."
---

# YouTube Thumbnail

Generates a set of distinct thumbnail concepts — visual direction plus exact on-image text — for a video, so a strong option can be picked or tested rather than defaulting to whatever frame is easiest to grab.

## When to use

Sibling skill to [[youtube-title]]: both run late in the pipeline, once the video (or at minimum a locked outline with a known payoff moment) exists. They're paired, not sequential — don't wait for a title to be chosen before drafting thumbnails, and don't let a thumbnail concept dictate the title. Both feed into [[youtube-publisher]] for final assembly. If the video's payoff or most visually interesting moment isn't known yet (edit still in progress), thumbnail concepts will be guesses — wait until it's locked, or ask.

## Inputs needed

- **The video's actual payoff** — the single most visually interesting, surprising, or emotionally charged moment or object in the video (not "what it's about" in the abstract — a specific frame or thing)
- **Brand visual kit** — colors, fonts, logo placement rules, whether a face-on-camera is standard for this channel
- **Competitive context** — what adjacent/competing thumbnails in this niche look like, so a concept doesn't blend in
- **Text treatment constraints** — max words allowed on-image (channel convention, usually 3–5), house font if one exists

## Concept framework

Generate concepts across distinct visual strategies — never submit multiple variants of the same strategy as if they were different concepts:

1. **Face + emotion** — a reaction shot (shock, excitement, skepticism) as the focal point
2. **Object / hero shot** — the product or result, isolated and large
3. **Before/after split** — a visual contrast, left/right or top/bottom
4. **Bold text or number** — a stat, count, or claim as the dominant visual element, minimal imagery
5. **Curiosity gap** — an obscured, partial, or pointed-at element that withholds the payoff

Rules for every concept:
- **On-image text capped at 4–5 words.** If it needs more, the idea belongs in the title, not the thumbnail.
- **One focal point only** — a thumbnail with two competing subjects loses both.
- **High contrast against YouTube's UI** — avoid critical detail in the bottom-right corner (duration badge) or far edges (mobile crop).
- **Legible at 120×90px** — if a concept only reads at full size, it fails; describe it in terms of what survives shrinking.

## Output format

3–5 concepts, each with:
1. **Strategy** — which of the five it uses
2. **Visual description** — composition, subject, framing, in enough detail to brief a designer
3. **Text treatment** — the exact on-image words, if any
4. **Rationale** — one line on why this stops a scroll for this specific audience

Flag which concept pairs best with which [[youtube-title]] variant, if titles are already available — a curiosity-gap thumbnail paired with a curiosity-gap title over-promises twice and reads as bait.
