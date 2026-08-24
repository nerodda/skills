---
name: x-copywriter
description: Drafts a post or thread for X from a brief, in the account's voice. Use once a brief exists and the idea has already cleared idea-review — the X/Twitter analog of linkedin-copywriter, but not a straight port of it, since X has different length constraints, thread mechanics, and register. Trigger on requests like "write the X post for this," "turn this into a thread," or "draft this brief for X."
---

# X Copywriter

Turns a brief into a publish-ready X post or thread — respecting X's character limits, thread mechanics, and terser register, rather than treating X as a shorter version of LinkedIn.

## When to use

Use this mid-pipeline, in the same slot as [[linkedin-copywriter]]: after a brief exists (from [[proposal-creator]], [[repurpose]], or [[researcher]]) and the idea has cleared [[idea-review]] or [[idea-tournament]], before [[taste-filter]] or [[ship-scan]]. There is no separate hook-writer skill for X — unlike LinkedIn, this skill owns the opening line itself, because on X the first line isn't a fold-teaser, it effectively *is* the post. Don't reuse a LinkedIn draft here; rewrite from the brief with X's constraints in mind.

## Inputs needed

- **The brief** — topic, angle, key points, and any CTA
- **Voice/tone reference for X specifically** — many accounts run blunter, more casual, or more opinionated on X than on LinkedIn; don't assume the LinkedIn voice doc transfers
- **Format constraint** — single post vs. thread, or let the brief's density decide (see rule below)
- **Character limit** — default 280/post unless the account has extended posting enabled; confirm rather than assume

## X-specific rules

- **Register**: terser, more declarative, more comfortable being blunt or informal than LinkedIn. Skip narrative scaffolding — get to the point in the first clause.
- **Single post**: the opening line carries the entire value of the post — there's no fold to rely on. Aim to fit the complete thought within 280 characters; cut ruthlessly rather than trailing off.
- **Thread trigger**: use a thread only when the brief has 3+ distinct points or sequential steps that genuinely need separate beats — not to pad a single-post idea into more surface area.
- **Thread mechanics**: tweet 1 must stand alone as a hook and open a loop (state what's coming, don't just announce a topic); each following tweet carries exactly one idea; the loop opened in tweet 1 must be closed by the final tweet — no threads that trail off without paying off the opening promise; close with a recap or CTA tweet, not a hard stop mid-thought.
- **No hashtags** — a dead convention on X, unlike LinkedIn's occasional 1–3.
- **White space**: used sparingly compared to LinkedIn's paragraph-per-line style — X readers scroll faster and tolerate denser blocks.
- Avoid LinkedIn-native phrasing ported straight over ("I'm thrilled to announce...", "Let that sink in.") — it reads as off-platform on X.

## Output format

For a single post: the post text plus character count, flagged if over the limit.

For a thread: a numbered list, one entry per tweet, each with its own character count, flagged individually if any tweet exceeds the limit. Close with one line confirming the loop opened in tweet 1 is paid off by the final tweet.
