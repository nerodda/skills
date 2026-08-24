---
name: youtube-publisher
description: "Assembles a finished video with its title, thumbnail, description, and publish metadata into a single upload-ready package, checking completeness and consistency across all of it. Use once [[youtube-title]], [[youtube-thumbnail]], and [[youtube-description]] have all produced their outputs and it's time to check everything before upload. Trigger on 'package this video for upload,' 'is this ready to publish,' or 'assemble the final upload package.' Does not draft, write, or design any content itself — only assembles and checks what the other skills already produced."
---

# YouTube Publisher

Assembles a finished video, its chosen title, its chosen thumbnail, and its description into one upload-ready package, and runs a checklist to catch anything missing or inconsistent before it goes live.

## When to use

Use last, once every upstream piece exists: the final edited video (from [[youtube-script]]'s filmed/edited output), a chosen title (from [[youtube-title]]), a chosen thumbnail (from [[youtube-thumbnail]]), and a description with chapters (from [[youtube-description]]). This is closest in spirit to [[ship-scan]] — a final check-and-assemble gate — but scoped to a single video asset rather than a whole piece of content. It never originates content: if something's missing, the fix is running the relevant upstream skill, not filling the gap here.

## Inputs needed

- **Final video file or link**, with confirmed runtime
- **Chosen title** — which [[youtube-title]] variant won, and why (for the record, not re-litigated here)
- **Chosen thumbnail** — image file or final concept from [[youtube-thumbnail]]
- **Description block** — full text from [[youtube-description]], chapters included
- **Publish metadata** — category, visibility (public/unlisted/scheduled), scheduled publish time if any, playlist assignment, end screen/cards configuration, captions file

## Assembly checklist

Run every item; this is a checklist, not a creative judgment call:

- [ ] Title matches the chosen [[youtube-title]] variant exactly — no last-minute edits introduced at upload
- [ ] Title displays fully without truncation at target length
- [ ] Thumbnail file is correct resolution/format (1280×720, under 2MB) and matches the chosen [[youtube-thumbnail]] concept
- [ ] Description is present in full, chapters start at `0:00`, and timestamps match the actual final edit
- [ ] All links in the description block are live and correctly targeted
- [ ] Captions/SRT file attached, or auto-captioning explicitly accepted as sufficient
- [ ] Category and tags set
- [ ] Playlist assignment made, if this video belongs to one
- [ ] End screen elements point to the correct next video/subscribe prompt
- [ ] Visibility and scheduled publish time set correctly
- [ ] Required sponsor/affiliate/legal disclosures present, both in description and on-screen if required
- [ ] **Title/thumbnail consistency check** — the two don't contradict or double-bait (e.g., both promising a different specific reveal)

Any failed item gets routed back to the skill that owns it — never patched here. This skill assembles and verifies; it doesn't rewrite a weak title or redesign a thumbnail.

## Output format

1. **Checklist** — every item above, marked pass/fail
2. **Blocking issues** — failed items, each naming which upstream skill owns the fix
3. **Verdict** — Ready to publish: yes / no, stated plainly
