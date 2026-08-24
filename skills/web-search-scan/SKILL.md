---
name: web-search-scan
description: Runs a structured web search on a given question or topic and returns sourced findings with citations. Use for general-purpose, open-web research — fact-checking a claim, gathering background on a topic, or answering "what does the internet say about X" — when the need isn't specific to sourcing material for a draft or scanning platform performance/trends. Trigger on requests like "search the web for X," "find out what's out there on X," or "look this up and give me sources."
---

# Web Search Scan

Runs a structured web search against a question or topic and returns findings with sources attached — a general-purpose research utility, not tied to any particular downstream deliverable.

## When to use

Use this for open-ended, general web research where the goal is simply "find out what's true or being said about X, with sources." It's distinct from [[researcher]], which sources material specifically to feed a draft already in motion, and from [[linkedin-trend-scan]] / [[x-trend-scan]], which scan platform-specific performance and trend data rather than the open web. If the question is "what's trending on LinkedIn right now," use the platform scan; if it's "what does the web say about this topic," use this.

## Inputs needed

Before searching, confirm:
- **The question or topic** — stated as specifically as possible; a vague topic produces a vague scan
- **Scope constraints**, if any — date range (e.g., "last 6 months only"), source type preference (e.g., news vs. primary sources vs. forums), or geography
- **What the findings are for**, if known — helps calibrate depth, but this skill will still run a general scan without it

If the question is too broad to search meaningfully ("tell me about marketing"), narrow it before running the search rather than returning a shallow scan of a huge topic.

## Search-and-source method

1. Run multiple search queries covering different angles of the question — don't rely on a single query and treat its top results as the full answer.
2. Prioritize primary sources (original reporting, official data, the entity's own statements) over secondary summaries or aggregator content when both are available.
3. Note source recency for anything time-sensitive — a claim sourced from a 3-year-old article on a fast-moving topic should be flagged as potentially stale, not presented as current.
4. Cross-check any load-bearing claim (a stat, a quote, a specific number) against at least two independent sources where possible; if only one source exists, say so rather than implying it's confirmed.
5. Discard sources that can't be attributed to an identifiable origin (no author, no organization, no verifiable publication) unless nothing better exists — and flag it as low-confidence if used.

**Sourcing/citation rule:** every finding in the output must carry an inline citation (source name + link) immediately next to the claim it supports. No unattributed claims — if a claim can't be sourced, either drop it or explicitly label it as inference rather than finding.

## Output format

1. **Summary** — 2–4 sentences answering the question directly, up front
2. **Findings** — a bulleted list, each bullet one finding with its source cited inline
3. **Confidence notes** — anything stale, single-sourced, or low-confidence, flagged explicitly
4. **Gaps** — anything the search couldn't answer, stated plainly rather than papered over
