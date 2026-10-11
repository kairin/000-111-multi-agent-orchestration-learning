# 5. Split work at meaningful boundaries

## Learning outcome

Build a task graph from uncertainty, dependencies, ownership, and distinct
acceptance evidence.

## Historical case

The earlier document mixed useful safety ideas with an active implementation
program: baseline tests, incremental code changes, configuration cleanup,
dependency maintenance, and a proposed Rust migration. Those activities have
different prerequisites and proofs. Treating them as one task would hide
blocked decisions and create overlapping ownership.

## Exercise

**Input:** the four local products in [CURRICULUM.md](CURRICULUM.md): inventory,
outline, link review, and integrated guide.

Draw this dependency graph, then complete the interface table:

```text
inventory ──> outline ──┐
                       ├──> integrated guide
inventory ──> link review ┘
```

| Task | Owner surface | Input | Output | Acceptance | Consumer |
|---|---|---|---|---|---|
| Inventory | Source list | Fixed source packet | Classified list | Every source appears once | Outline, link review |
| Outline | Learning structure | Accepted inventory | Section plan | Every objective has a section | Integration |
| Link review | Link table | Accepted inventory | Link findings | Each local target resolves | Integration |
| Integration | Final guide | Three accepted handoffs | Coherent guide | No contradiction or missing objective | Reviewer |

Add an exclusion to each row and mark the two tasks that may run in parallel.

**Artifact:** the `task graph and interfaces` section of
`integration-record.md`.

**Acceptance check:** parallel tasks have disjoint mutable surfaces, every edge
names an output consumed as input, and every task has a different check or a
clear reason to remain combined.

**Stop:** do not split further when a smaller task would have the same owner,
input, consumer, and acceptance check. Do not combine tasks across a blocking
edge.
