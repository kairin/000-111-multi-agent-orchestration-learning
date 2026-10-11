# 2. Separate evidence from authority

## Learning outcome

Use an existing system as evidence without inheriting its goals, commands, or
permission boundaries.

## Historical case

**Observed:** the repository was separated from the upstream Git fork network,
but source files retained upstream package names, links, commands, community
documents, and a plugin download path. Git separation changed where a push
would go; it did not make every embedded instruction safe or current.

**Lesson:** provenance, technical coupling, and authority are separate
questions. Copying a source gives evidence. It does not authorize operating,
publishing, or changing the source system.

## Exercise

**Input:** [the historical original README](../archive/documents/README-upstream-original.md)
and this repository's [current README](../README.md). Read prose only.

Create a boundary map:

| Item | Evidence available | Authority granted | Allowed learning use |
|---|---|---|---|
| Product commands | Historical documentation | None | Identify side effects and dependencies |
| Source code | Versioned implementation | Read-only for this exercise | Verify a cited fact |
| Research notes | Prior analysis | Evidence, not owner decisions | Find gaps and contradictions |
| Curriculum | Current learning contract | Complete paper exercises | Produce reviewable artifacts |

Add one example where evidence exists but authority does not.

**Artifact:** the `evidence boundary` section of `integration-record.md`.

**Acceptance check:** each source has a provenance, allowed use, and prohibited
inference. The map does not direct a clone, install, build, release, or change
outside this repository.

**Stop:** if authority is missing, record the boundary. Do not turn it into an
implementation task.
