# 1. Define the objective and scope

## Learning outcome

Turn a broad request into one outcome, explicit exclusions, and observable
completion conditions. Scope is the first interface: downstream owners should
not need to guess what the request author meant.

## Historical case

**Observed:** this repository began with OpenRig 0.5.16 source and a goal to
make a smaller personal tool. The research later added a proposed full Rust and
Node-removal destination. Those statements generated a large implementation
backlog before the owner had resolved which workflows must remain.

**Lesson:** a technology destination is not a complete objective. It does not
identify the user outcome, retained behavior, or evidence that proves success.

## Exercise

**Input:** the example objective in [CURRICULUM.md](CURRICULUM.md) and the root
[README](../README.md).

Write a scope card with:

| Field | Required content |
|---|---|
| Outcome | One result a reviewer can observe |
| Required products | Inventory, outline, link review, integrated guide |
| Exclusions | Runtime execution, implementation edits, commit, or publication |
| Evidence | The checks that prove each product exists and agrees |
| Stop point | The condition that ends the exercise |

**Artifact:** the `scope` section of `integration-record.md`.

**Acceptance check:** every required product maps to one check, every exclusion
rules out an identifiable action, and no technology choice substitutes for the
outcome.

**Stop:** do not decompose work until the card passes the check. Return an
unresolved change in audience or required products to the objective owner.
