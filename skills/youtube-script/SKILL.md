---
name: youtube-script
description: "Turns an approved outline into a full shot-by-shot script — every line of dialogue or voiceover, on-screen text, and shot direction, ready to film or edit from. Use once an outline exists (from [[launch-video]] for launch-tied videos, or a standalone brief for anything else) and it's time to write the actual words and shots. Trigger on 'write the full script for this,' 'turn this outline into a script,' or 'script this out shot by shot.' Not for building the outline itself and not for packaging a finished video for upload."
---

# YouTube Script

Turns an approved outline into a full shot-by-shot script: exact dialogue or voiceover lines, on-screen text, and shot/visual direction for every beat, ready to hand to a camera operator or editor.

## When to use

Use mid-pipeline, after an outline has been approved — either from [[launch-video]] for launch-tied videos, or from a standalone brief for anything else (tutorials, evergreen explainers, repurposed long-form). This skill consumes an outline; it does not build one. If no outline exists yet, get one first — writing a shot-by-shot script from nothing skips the structural decisions an outline is supposed to settle.

Once the script is finished and filmed/edited into a final video, that video moves to [[youtube-title]] and [[youtube-thumbnail]] (parallel packaging), then [[youtube-description]] (once timestamps are locked), and finally [[youtube-publisher]] for assembly.

## Inputs needed

- **Approved outline** — beats, hook, and CTA already decided (from [[launch-video]] or elsewhere)
- **Format** — on-camera talent, voiceover-over-footage, or screen recording; this determines whether lines are "spoken" or "read"
- **Brand voice guidelines** — vocabulary, sentence length, first-person vs. brand voice
- **Runtime target** — drives how many shots per beat and how tightly lines need to be cut
- **Existing asset inventory** — B-roll, screen recordings, graphics already available vs. needing to be created

## Shot-by-shot structure

Write the script as a table, one row per shot, with these columns:

| Time | Shot / Visual | VO or Dialogue | On-screen text | Notes |
|---|---|---|---|---|

Rules:
- **Hook line is verbatim from the outline's chosen hook option** — don't rewrite it loosely; the first 3 seconds are the highest-leverage line in the video.
- **One idea per shot.** If a line does two jobs (explains and transitions), split it into two shots.
- **VO/dialogue sentences stay short** — aim for ~15 words or fewer per line; long sentences don't survive a cut.
- **Every graphic or overlay gets an explicit callout** in the "On-screen text" column — never leave it implied in the visual description.
- **CTA is written verbatim**, matching the outline's chosen CTA exactly — no paraphrasing at the point of ask.
- **Scene breaks match the outline's beats** — group shots under a heading per beat (Hook / Context / Reveal / Proof / CTA, or the brief's equivalent) so the script's structure stays traceable back to the outline.

## Output format

Return:
1. **Full script** in shot-by-shot table format, grouped under scene headings that match the source outline's beats
2. **Alt hook line** — one alternate cold-open option, scripted in full, for A/B testing the first 3 seconds
3. **Flags** — any beat where the outline didn't specify enough to write a concrete shot (ask rather than invent a visual)
