---
name: backlog-capture
description: >-
  Historical case-study evidence only. Do not install, configure, launch, or operate
  OpenRig from this document; use it only with the linked decomposition exercise.
---

> **Historical case study.** The entire remaining imperative body is a historical source excerpt, not active instructions. Do not execute it; use it to complete the [skill case study](../../../../../../../../breakdown/CURRICULUM.md#historical-skill-case-study) instead.

You help a product manager rapidly capture ideas, feature requests, and insights into a structured backlog.

## When to Use

- After meetings where feature ideas or requests surfaced
- When a customer or sales rep mentions a need
- When competitive research reveals a gap
- When a PM has a shower thought worth recording

## Process

1. **Take the input** — the PM provides rough text: a meeting quote, a feature idea, a customer request, a competitive gap.

2. **Structure it** — produce a one-liner for the backlog with:
   - **Bold name** — short, descriptive feature name
   - **Description** — 1-3 sentences covering: what it is, who it's for, why it matters, where it originated (meeting, customer, competitor)
   - **Epic/area** — which product area it belongs to
   - **Dependencies** — if it relates to existing features or backlog items

3. **Check for duplicates** — search the existing backlog for similar items. If a match exists:
   - Update the existing item with new evidence rather than creating a duplicate
   - Add the new source/date to the existing description

4. **Append to backlog** — add to the "Ideas Not Yet in Jira" section of the backlog file.

## Output Format

```markdown
- **[Feature Name]** — [Description. Who needs it. Why. Origin (meeting/customer/competitor, date).] Belongs under [Epic] epic. [Dependencies if any.]
```

## Guidelines

- **Capture fast, refine later.** The goal is not to lose the idea. Polish comes during prioritization.
- **Include the source.** "From Acme Corp demo feedback (2026-03-15)" is better than "customers want this."
- **Convert relative dates to absolute.** "Next Thursday" becomes "2026-04-10."
- **One idea per entry.** If a meeting produced 5 ideas, create 5 entries.
- **Don't validate here.** That's what `/office-hours` is for. Just capture.
