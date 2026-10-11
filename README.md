# Learning orchestration from a historical agent system

Canonical project name: `000-111-multi-agent-orchestration-learning`.

This repository is a documentation-only learning case study. It uses a
historical OpenRig 0.5.16 snapshot, specifications, skills, and research as primary
sources for learning how to decompose work and coordinate agents. It is not a
project to install, revive, simplify, port, or publish OpenRig.

The implementation remains because it is evidence. Commands, runbooks, skills,
release procedures, and configuration examples describe the historical system.
Do not execute them as instructions from this repository.

## What you will learn

After the route below, you should be able to:

- split an objective where uncertainty and dependencies change;
- give each owner a bounded file or decision surface;
- define inputs, outputs, interfaces, and acceptance checks before work starts;
- use a fixed concurrency budget without starting blocked or overlapping work;
- require evidence in handoffs and review it before integration;
- stop when the objective is met, evidence is insufficient, or a decision owner
  is required.

No OpenRig runtime, paid service, specific model, or additional tool is needed.
The exercises produce Markdown tables and short decision records.

## Learning route

Start with [the curriculum](breakdown/CURRICULUM.md). The numbered modules use
one historical repository as a case study:

| Module | Learning outcome | Exercise artifact |
|---|---|---|
| [01](breakdown/01-goal-and-scope.md) | Turn a broad request into an objective and exclusions. | Scope card |
| [02](breakdown/02-separation-from-upstream.md) | Separate evidence, authority, and allowed actions. | Boundary map |
| [03](breakdown/03-local-environment.md) | Identify side effects and prerequisites without running a system. | Risk register |
| [04](breakdown/04-review-method.md) | Convert claims into verifiable research tasks. | Claim review card |
| [05](breakdown/05-simplification-rules.md) | Split work at uncertainty and dependency boundaries. | Task graph |
| [06](breakdown/06-open-questions.md) | Route decisions to the right owner and keep agents moving. | Decision ledger |
| [07](breakdown/07-review-task-list.md) | Schedule bounded work under a fixed concurrency budget. | Work allocation table |
| [08](breakdown/08-current-state-evidence.md) | Distinguish observed facts from proposed designs. | Evidence map |
| [09](breakdown/09-adversarial-review-and-research-charter.md) | Design independent review and disproof checks. | Review plan |
| [10](breakdown/10-rust-and-node-removal-plan.md) | Analyze a historical migration plan without authorizing it. | Dependency and interface audit |
| [11](breakdown/11-coordination-outcomes.md) | Integrate handoffs and make continue, rework, or stop decisions. | Integration record |

The recurring exercise examines a hypothetical local documentation bundle with four
work products: source inventory, learning outline, link review, and integrated
guide. It is intentionally small enough to reason about on paper. Historical
OpenRig facts supply examples and counterexamples; the exercise never asks you
to build or operate the system, commit changes, or publish the bundle.

## How to read the repository

The [coverage ledger](breakdown/DOCUMENT-COVERAGE.md) accounts for every tracked
Markdown, HTML, YAML, and YML file that was present when this curriculum was
created. It separates curriculum, research evidence, historical operational
evidence, and immutable records.

Within historical material, words such as “run,” “install,” “deploy,” and
“publish” belong to the quoted source context. Use them to identify task
boundaries, side effects, missing checks, and unsafe assumptions.

## Historical provenance

The repository began as a personal derivative of
[OpenRig](https://github.com/mvschwarz/openrig) by Mike Schwarz, version 0.5.16.
The original README is preserved at
[archive/documents/README-upstream-original.md](archive/documents/README-upstream-original.md).
The original source remains under Apache-2.0; later repository material has the
licenses recorded in [REUSE.toml](REUSE.toml). This curriculum changes the
purpose of this repository, not the provenance of its evidence.
