# 6. Route questions to evidence or a decision owner

## Learning outcome

Distinguish research questions from policy choices and keep independent work
moving while a decision is unresolved.

## Historical case

The prior research accumulated questions about retained interfaces, state
migration, operating systems, terminal providers, external tools, packaging,
and a proposed Rust/Node boundary. Source inspection could reveal current
mechanisms and dependencies, but it could not choose the owner's desired
product. Repeatedly asking agents to research a preference would not resolve it.

## Exercise

**Input:** the task graph from module 05 and these three questions:

1. Which local links are broken?
2. Should the guide target a new learner or an experienced coordinator?
3. Does the inventory include every file in the fixed packet?

Create a decision ledger:

| Question | Type | Resolver | Blocks | Work that may continue | Escalation evidence |
|---|---|---|---|---|---|
| Broken links | Research | Link-review owner | Integration | Outline | Findings table |
| Audience | Owner decision | Objective owner | Outline tone, integration | Inventory, link review | Two concrete options and impact |
| Inventory complete | Verification | Inventory reviewer | Both parallel consumers | None that consumes inventory | Reconciliation count |

**Artifact:** the `decision ledger` section of `integration-record.md`.

**Acceptance check:** each question has one resolver, named downstream impact,
and evidence appropriate to its type. No preference is assigned to a research
agent and no factual check is escalated to the owner.

**Stop:** escalate only the audience decision, with options and affected work.
Resume its blocked branches after the answer; do not restart independent work.
