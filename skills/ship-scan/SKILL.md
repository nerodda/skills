---
name: ship-scan
description: Final pre-publish check for gaps, broken links, and missing assets. Use immediately before anything goes live, after taste-filter has already passed the draft on voice and quality — this is the last mechanical gate, not a content judgment call. Trigger on requests like "is this ready to publish," "final check before it goes out," or "ship-check this post." Catches broken links, missing images or alt text, bad metadata, and leftover placeholder text — not tone or genericness, that's taste-filter's job.
---

# Ship Scan

Runs a mechanical checklist over a finished piece right before it goes live — links, assets, metadata, formatting, placeholder text — and returns a clear ready/not-ready verdict.

## When to use

Run this last, after [[taste-filter]] has cleared the draft for voice and quality, and immediately before scheduling or hitting publish. This is a mechanical gate, not a quality judgment — if a voice or tone issue turns up here, send the piece back to taste-filter rather than fixing it in place.

## Inputs needed

- **Final draft/asset**, in its actual ready-to-publish form — not a working doc
- **Target platform** — blog, LinkedIn, X, YouTube, newsletter, etc.
- **Full list of links** used in the piece
- **Required assets** — images, thumbnail, video file, downloadable or lead-magnet attachment
- **Platform metadata requirements** — title tag, meta description, OG image, tags/categories, alt text conventions

## Checklist

- [ ] Every link resolves — no 404s, no typos in URLs
- [ ] Every external link that should carry tracking has correct UTM parameters
- [ ] All images/assets referenced in the draft actually exist and are attached
- [ ] Every image has alt text
- [ ] No placeholder text remains — `[TK]`, `[INSERT STAT]`, `[LINK HERE]`, lorem ipsum, bracketed notes-to-self
- [ ] Metadata is complete: title tag, meta description, OG image/preview card render correctly
- [ ] Formatting renders correctly on the target platform — check the actual platform preview, not just the source doc
- [ ] CTA is present and links to the correct destination
- [ ] Citations/attribution from [[researcher]] survived editing intact and correctly formatted
- [ ] Publish settings are correct: scheduled time, correct account/channel, correct visibility

## Output format

1. Fails only — list each checklist item that didn't pass, skip restating every pass
2. **Blocking issues** (must fix before publish) vs. **warnings** (should fix, won't break anything)
3. Final verdict: **Ready to publish** / **Not ready** — fix items above
