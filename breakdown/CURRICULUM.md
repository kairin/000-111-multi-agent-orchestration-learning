# Curriculum: decompose, coordinate, verify, integrate

## Course contract

The course uses a historical multi-agent system as evidence and a hypothetical
local documentation bundle as the worked example. “Bundle” means files reviewed
on the learner's machine; it does not mean commit, push, publish, or release.
You need only a text editor or paper. Do not run the historical system.

The example objective is:

> Produce a four-part guide from a fixed source packet: an inventory, a learning
> outline, a link review, and one integrated guide.

The fixed source packet is the root [README](../README.md), modules
[01](01-goal-and-scope.md), [04](04-review-method.md), [07](07-review-task-list.md),
and [11](11-coordination-outcomes.md). This keeps every exercise bounded.

## The working model

Decompose at a boundary that changes one of four things:

1. **Uncertainty:** research must finish before a design choice is meaningful.
2. **Dependency:** an output is required as another task's input.
3. **Ownership:** two tasks would edit or decide the same surface.
4. **Verification:** different evidence proves the outcomes.

For every task, write an interface before assigning it:

| Field | Meaning |
|---|---|
| Input | Exact files, facts, or prior artifacts the owner may rely on |
| Output | One reviewable artifact and its location |
| Exclusions | Work the task must not absorb |
| Acceptance | Observable checks for completeness and correctness |
| Consumer | Person or task that uses the output next |

Parallel work is safe only when owners do not share a mutable surface and each
task has all required inputs. A concurrency budget is a ceiling, not a target.
Leave a slot unused when the next task is blocked or would create integration
work without shortening the critical path.

## Route and cumulative artifact

Complete modules 01–11 in order. Each module adds one section to an
`integration-record.md` that you create for the exercise. The final record must
contain objective and exclusions, evidence/authority boundary, risk register,
claim review, dependency graph and owners, decision ledger, concurrency
schedule, evidence classification, independent review plan, interface audit,
and integration verdict with a stop reason.

Each module gives its own acceptance check. A peer should be able to review the
record without opening any implementation file.

## Historical operational evidence exercise

**Input:** one historical manual, demo guide, runbook index, or package README
that links here. Read only that document's prose and command examples.

Create an operational-evidence card with: historical objective, inputs,
side effects, owners, dependency edges, handoff artifact, verification evidence,
and stop condition. Mark every claim as observed, proposed, or unknown.

**Artifact:** one Markdown table with those eight fields.

**Acceptance check:** the card identifies at least one side effect, one blocked
dependency, one owner interface, and one checkable handoff without directing
the reader to execute a command. **Stop** after one document and one card.

## Historical skill case study

**Input:** one historical `SKILL.md` that links here. Treat its entire
imperative body as a source excerpt.

Extract one task contract with: trigger rewritten as a learning question,
bounded input, owner surface, expected artifact, consumer, acceptance check,
and stop or escalation condition. Then identify one imperative that would be
unsafe if it were mistaken for current authority.

**Artifact:** one skill-analysis card in Markdown.

**Acceptance check:** the card includes all seven contract fields, quotes no
secret or credential value, and converts the unsafe imperative into an
observation or question rather than an action. **Stop** after one skill.

## Stop conditions

Stop a task and hand it back when its acceptance check passes. Stop the overall
exercise when all required artifacts integrate without unresolved contradictions.
Pause a branch when a required input is missing. Escalate only decisions whose
owner, impact, and blocked downstream task are named. More agents, more prose,
or more source reading are not completion evidence.
