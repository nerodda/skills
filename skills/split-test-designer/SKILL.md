---
name: split-test-designer
description: Designs a split test — hypothesis, control, variant, success metric, and sample/duration requirements — without writing the variant copy itself. Use when someone wants to test a change and needs the experiment structured properly before anything gets written or built. Trigger on requests like "design a split test for X," "how should we A/B test this," or "set up an experiment for this." Not for writing the actual variant copy — hand that to the relevant copywriter skill once the test is designed.
---

# Split Test Designer

Designs the structure of a split test — hypothesis, control, variant, success metric, and sample/duration requirements — so a valid experiment can run. It does not write the variant copy itself.

## When to use

Use this whenever a test needs to be designed before it's built: a subject line test, a CTA test, an outbound opener test, a landing page headline test, etc. This skill stops at the design — once the test is designed, hand the actual variant-copy drafting to whichever copywriter skill fits the asset (e.g., [[outbound-copywriter]] for a cold sequence variant, [[linkedin-hook-writer]] for a hook variant). Mixing the two jobs produces a test where the variant was picked before the hypothesis was, which defeats the point of testing.

## Inputs needed

Before designing, confirm:
- **What's being tested** — the specific asset or touchpoint (subject line, CTA, hook, landing page section, etc.)
- **Current baseline** — what's running now, if anything, to serve as control
- **The metric already tracked** — what data is actually available to measure against (open rate, reply rate, conversion rate, etc.) — don't design a test around a metric nobody can pull
- **Available volume** — rough traffic/send volume per period, needed to sanity-check whether a valid sample is reachable in a reasonable window

If available volume is unknown, ask — a test designed for a sample size the traffic can't reach in a reasonable timeframe isn't a usable design.

## Experiment-design checklist

Every test design must include all of the following, in this order:

1. **Hypothesis** — a single sentence in the form "If we change [X], then [metric] will [improve/change] because [reason]." Not "let's see what happens" — a real, falsifiable prediction.
2. **Single variable** — name the one element being changed. If the request bundles multiple changes (new headline + new CTA + new image), split it into separate tests or explicitly flag that a multi-variable test won't isolate which change caused the result.
3. **Control** — what stays unchanged, stated explicitly, not just implied by "everything else."
4. **Variant** — described at the level of "what's different," not the actual copy (that's downstream work).
5. **Success metric** — the one primary metric that decides the winner, plus any guardrail metric that shouldn't get worse even if the primary metric improves.
6. **Minimum sample size / duration** — a concrete number or time window before results can be trusted, sized to the available volume from the inputs. If volume is too low to reach a meaningful sample in a reasonable window, say so and recommend a longer window or a bigger swing (bigger expected effect) instead of a subtle one.
7. **Decision rule** — what result ends the test and what happens next (ship the winner, extend the test, or call it inconclusive).

## Output format

The completed checklist above, one labeled section per item, ending with a one-line summary of what happens next: who builds the variant copy and which skill that falls to.
