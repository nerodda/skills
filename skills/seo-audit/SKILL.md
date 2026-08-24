---
name: seo-audit
description: Checks a draft or live page against on-page SEO fundamentals — title tag, meta description, heading structure, internal links, alt text, and keyword placement. Use before publishing a piece, or periodically against a live URL, to catch on-page issues before they cost search visibility. Trigger on requests like "SEO check this draft," "audit this page," or "is this ready to publish." A checking skill, not a drafting one — it doesn't rewrite the piece, it reports what's wrong.
---

# SEO Audit

Checks a draft or a live page against a concrete on-page SEO checklist and reports what passes, what fails, and what to fix — a gate before publish, not a rewrite.

## When to use

Use this before a piece goes live (on a draft from [[long-form]] or elsewhere) or periodically against an already-published URL to catch drift. This is a checking skill, in the same shape as [[ship-scan]] or [[taste-filter]] — it audits and reports, it does not rewrite the piece itself. If issues are found, they go back to whoever owns the draft to fix, not fixed silently inside this skill.

## Inputs needed

- **The content** — either a draft (with its intended title tag/meta description if not obvious from the text) or a live URL to fetch and inspect
- **Target keyword(s)** — the primary keyword/phrase this page is meant to rank for, plus any secondary terms
- **Site context**, if auditing a live URL — existing internal linking conventions, so missing internal links can be flagged against what's actually available to link to

If no target keyword is given, ask for one — keyword placement checks are meaningless without knowing what the page is trying to rank for.

## On-page checklist

Check each item and mark pass / fail / warning with the specific fix.

- **Title tag** — present, under ~60 characters, contains the primary keyword (ideally near the front), unique from other pages on the site, and reads as a real title rather than keyword-stuffed.
- **Meta description** — present, under ~155–160 characters, contains the primary keyword, and reads as a compelling reason to click rather than a keyword list.
- **URL slug**, if applicable — short, contains the primary keyword, no unnecessary stop words or query cruft.
- **Heading structure** — exactly one H1 matching the page's actual topic, logical H2/H3 nesting (no skipped levels), and headings that describe the section rather than being generic.
- **Keyword placement** — primary keyword appears in the H1, in the first ~100 words of body copy, and at least once more in a subheading or body naturally (not forced or stuffed).
- **Internal links** — a reasonable number of contextual links to other relevant pages on the site, with descriptive anchor text (not "click here"); flag orphaned pages with no inbound internal links pointing to them if that context is available.
- **External links**, if present — link to credible sources, open in a sensible target, and don't undermine the page's own authority on the topic.
- **Image alt text** — every meaningful image has descriptive alt text; decorative images either have empty alt or are excluded appropriately. Flag any alt text that's just keyword-stuffed rather than descriptive.
- **Content length/depth vs. intent** — rough gut check that the page's depth matches what the target keyword's search intent requires (a comparison keyword needs more than a one-paragraph answer).
- **Duplicate/thin content** — flag if the page substantially overlaps with another existing page's title/keyword target, which splits rather than builds authority.

## Output format

A checklist report, one line per item: pass / fail / warning, plus the specific fix for anything short of pass. End with an overall verdict — **ready to publish** or **needs fixes** — and, if needs fixes, the two or three highest-priority items to address first.
