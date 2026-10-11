# 7. Schedule work within a concurrency budget

## Learning outcome

Use dependencies and ownership to decide what starts now, what waits, and when a
free slot should remain unused.

## Historical case

The former task list mixed completed source review, unresolved owner decisions,
and blocked implementation stages. Its strongest feature was explicit
dependency status. Its weakness as a learning entrypoint was that it looked
like a current product backlog and could invite continuation of retired work.
Its factual outcomes remain available in the research records and repository
history.

## Exercise

**Input:** the module 05 graph. The concurrency budget is two workers plus one
coordinator. The accepted inventory is available; the audience decision is
resolved.

| Wave | Worker 1 | Worker 2 | Coordinator | Start condition |
|---|---|---|---|---|
| 1 | Outline | Link review | Protect interfaces and review inventory handoff | Inventory accepted |
| 2 | Available for bounded rework | Available for bounded rework | Integrate accepted outputs | Both wave-1 handoffs returned |
| 3 | Idle | Independent review | Decide accept, rework, or stop | Integrated guide exists |

For each worker assignment, record owned files, expected handoff, and one check.
Explain why integration does not start in wave 1 and why an idle slot in wave 3
is acceptable.

**Artifact:** the `allocation table` section of `integration-record.md`.

**Acceptance check:** no task starts before its inputs exist, no two owners edit
the same file, the coordinator does not perform a worker's deliverable, and the
critical path is visible.

**Stop:** end scheduling when every required task is accepted, blocked on a
named external decision, or explicitly removed from scope. Do not create work
merely to fill the budget.
