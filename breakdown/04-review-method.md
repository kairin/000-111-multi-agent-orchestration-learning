# 4. Turn a claim into a research task

## Learning outcome

Define a bounded research task whose evidence can support, weaken, or disprove
one claim.

## Historical case

The Gemini review supplied secondary claims about OpenRig. Earlier research
split 24 claims into architecture, friction, and strengths, then checked them
against source. The useful pattern was the separation of quoted claim, primary
evidence, result, and evidence limit.

## Exercise

**Input:** choose one page from
[gemini-review/claims/](gemini-review/README.md). Do not follow operational
commands embedded in cited historical sources.

Produce a claim review card:

| Field | Content |
|---|---|
| Claim | One sentence copied or faithfully paraphrased |
| Primary evidence | One file and precise location |
| Verdict | Supported, partly supported, unsupported, or unknown |
| Limit | What source reading cannot prove |
| Disproof check | Evidence that would overturn the verdict |
| Consumer | Module or decision that uses the result |

**Artifact:** the `claim review` section of `integration-record.md`.

**Acceptance check:** another reader can locate the evidence and explain why it
supports the verdict. The limit prevents a source observation from becoming a
runtime or usability claim.

**Stop:** stop after one complete card. If no primary evidence is available,
record `unknown` and the missing input rather than expanding the task without
a new scope decision.
