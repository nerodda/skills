---
name: process-flowchart
description: Turns a described process into a visual flowchart rendered as Mermaid diagram syntax. Use when a process, workflow, or decision sequence has been described in prose or bullet form and needs to become a diagram someone can actually follow at a glance. Trigger on requests like "turn this into a flowchart," "diagram this process," or "map out the steps visually." A diagramming skill, not a copywriting one — it doesn't rewrite or improve the process, only visualizes it.
---

# Process Flowchart

Converts a process described in prose, bullets, or a rough sequence of steps into a visual flowchart, output as Mermaid diagram syntax so it renders directly wherever Mermaid is supported.

## When to use

Use this whenever a process needs to be seen, not just read — onboarding flows, decision trees, approval chains, content pipelines, or any sequence with branches or handoffs that prose makes hard to follow. This is a visualization skill: it does not edit, improve, or restructure the underlying process — if the process itself is unclear or has gaps, flag that, but don't silently invent steps to make the diagram look complete.

## Inputs needed

Before diagramming, confirm:
- **The process description** — the steps, in whatever form they exist (prose, bullets, a messy brain dump is fine)
- **Start and end points** — where the process begins and where it terminates (or terminates in more than one place, e.g., approved vs. rejected)
- **Decision points** — any step where the path branches based on a condition, and what the conditions are
- **Actors/swimlanes** — if different people or systems own different steps, note who owns what (optional, only if it changes the diagram)

If steps are missing or the branch logic is ambiguous (e.g., "then it gets reviewed" with no stated outcome), ask what happens on each branch rather than assuming a single path.

## Notation

Output as Mermaid flowchart syntax (`flowchart TD` for top-down, or `flowchart LR` for left-right if the process is naturally sequential/short). Node and edge conventions:

- **Process step** — rectangle: `A[Do the thing]`
- **Decision point** — diamond: `B{Condition?}`, with labeled edges for each branch: `B -->|Yes| C` / `B -->|No| D`
- **Start/end** — rounded/stadium shape: `S([Start])` / `E([End])`
- **External handoff** (to another person/system/tool) — subroutine shape: `H[[Hand off to X]]`
- Every node gets a short verb-led label (e.g., "Submit request," not "Request submission stage") — labels should read as actions, not stage names.
- Every decision node must have every branch labeled and every branch must terminate somewhere (either back into the flow, at an end node, or explicitly marked as a loop back to an earlier step).
- Use subgraphs (`subgraph Name ... end`) to group steps by actor/owner when swimlanes are relevant; skip subgraphs entirely when there's a single owner throughout.

## Output format

A single fenced Mermaid code block, valid and renderable as-is, preceded by one line naming the process being diagrammed. If any step in the source description was ambiguous and required a judgment call to diagram, note that call in one line beneath the diagram rather than silently resolving it.
