# Research evidence guide

The files in this section record source reading and historical review. They are
inputs to the learning modules, not current tasks or permission to operate the
former product.

| Evidence set | Files | Best learning use |
|---|---|---|
| Current-state map | `08-current-state-evidence.md` | Separate observed mechanisms from runtime assumptions. |
| Research design | `09-adversarial-review-and-research-charter.md` | Study gates, counter-evidence, and bounded work packages. |
| Migration proposal | `10-rust-and-node-removal-plan.md` | Find dependency and interface obligations in a proposed change. |
| Coordination record | `11-coordination-outcomes.md` | Review ownership, handoffs, and no-go decisions. |
| Capability and workflow research | `research-capability-inventory.md`, `research-workflow-scope.md`, `research-workflow-traces.md` | Compare inventories with end-to-end journeys. |
| State and runtime research | `research-state-invariants.md`, `research-runtime-verification-plan.md`, `research-runtime-verification.md` | Distinguish source evidence from unrun runtime proof. |
| Review and decisions | `research-card-goal-audit.md`, `research-review-matrix.md`, `research-coordinator-review-a6c2b.md`, `research-owner-decision-brief.md` | Study review independence and decision routing. |
| External claim review | `gemini-review/` (32 files) | Practice checking secondary claims against primary sources. |

When a research file says that an owner “must” choose something or that a later
stage “should” run, record it as a historical open decision or proposed test.
Do not treat it as a task for this repository.

For a bounded practice pass, choose one claim, capture its cited evidence, name
what the evidence cannot prove, and write one disproof check. Stop after the
four fields are complete.
