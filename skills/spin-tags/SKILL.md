---
name: spin-tags
description: Generates spintax variants of an existing piece of copy using {option1|option2|option3} bracket syntax for programmatic ad or outbound variation. Use when copy already exists and needs mechanical variation at the word/phrase level for tools that consume spintax — not a rewrite of the piece, a narrow syntax transformation. Trigger on requests like "spin this copy," "add spintax to this," or "give me variants for this ad in spintax format."
---

# Spin Tags

Takes existing copy and inserts spintax — the `{option1|option2|option3}` bracket syntax — at the word and phrase level, so downstream tools can generate randomized variants for ad or outbound platforms.

## When to use

Use this only when copy already exists and the ask is specifically for spintax-formatted variation, not a rewrite. This is a narrow, mechanical transformation: swap in alternate words and phrases at chosen points in the existing copy, preserving its structure and meaning. It is not [[philipp-rewrite]] — that skill rewrites a piece's voice and structure wholesale; this skill touches only the specific spots marked for variation and leaves everything else untouched.

## Inputs needed

Before spinning, confirm:
- **The source copy** — the exact text to spin
- **Variation points** — which words/phrases should vary, if the requester has specific ones in mind (if not, choose points yourself per the rules below)
- **Variant count target** — how many options per spin point (default 3 if unset)
- **Platform constraint**, if any — some ad platforms have character limits per rendered variant; note if the longest possible combination needs to fit a limit

If no specific variation points are given, select them yourself using the rules below rather than asking — this is a mechanical task and over-asking defeats the point.

## Spintax syntax rules

- Format: `{option1|option2|option3}` — pipe-separated alternatives inside curly braces, no spaces around the pipes unless the option itself needs a leading/trailing space.
- Spin at the word or short-phrase level only — a single word, or a phrase of 2–4 words that reads naturally in every combination. Never spin a whole sentence as one option unless the sentence-level meaning genuinely doesn't change between variants.
- Every option inside one set of braces must be grammatically interchangeable — same part of speech, same tense, fits the same sentence slot. A spin set that breaks grammar in some combinations is a bug, not a variant.
- Default to 3 options per spin point (2 minimum, 5 maximum) — fewer than 2 isn't a variant, and more than 5 usually means the option list needs curating, not padding.
- Prioritize spin points that most affect how the copy reads or performs: the hook/opening word, the CTA verb, urgency language, and the key benefit noun. Don't spin filler words (articles, conjunctions) — that inflates the combination count without adding meaningful variation.
- Nested spintax (a spin set inside another spin set's option) is allowed only if the platform consuming it supports nesting; default to flat, non-nested spin sets unless told otherwise.

## Output format

The source copy with spintax inserted inline, plus:
- A count of total spin points used
- The total number of possible unique combinations (product of each spin set's option count)
- A flag if that combination count exceeds any stated platform limit
