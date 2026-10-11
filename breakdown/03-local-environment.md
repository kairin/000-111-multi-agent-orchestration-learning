# 3. Map side effects before execution

## Learning outcome

Identify state, side effects, and collision risks from documentation without
running the system or inspecting live credentials.

## Historical case

**Observed at the research baseline:** the copied implementation used command
names and a state directory also used by an installed OpenRig version. The
historical daemon could write agent and terminal configuration, manage hooks,
and download a plugin. The old document responded with operational advice such
as choosing an installation, changing paths, and backing up live state.

**Current boundary:** those directions are historical evidence. This learning
repository does not authorize checking, removing, backing up, or changing any
installation, home-directory configuration, provider, or credential.

## Exercise

**Input:** the two paragraphs above and the source summary in
[08-current-state-evidence.md](08-current-state-evidence.md#85-five-concrete-runtime-flows-and-the-contracts-they-carry).
Do not inspect the live machine.

Create a risk register:

| Surface | Historical side effect | Failure if shared | Evidence needed before a real run | Owner |
|---|---|---|---|---|
| Command name | Selects an executable | Wrong program starts | Resolved executable identity | Operator |
| State directory | Reads and writes durable state | Versions corrupt shared data | Isolated path and recovery proof | Runtime owner |
| Agent configuration | Adds or removes managed blocks | User settings change | Ownership markers and rollback test | Adapter owner |
| Download path | Retrieves external content | Unreviewed code enters the system | Pinned source and offline policy | Security owner |

Add one risk from the source summary. For that row, name the downstream task
that cannot start until evidence exists.

**Artifact:** the `risk register` section of `integration-record.md`.

**Acceptance check:** every row names a state surface, a concrete failure, a
specific evidence requirement, and one owner. No row asks the learner to touch
the live surface.

**Stop:** finish when the five rows pass the check. In real work, a task with a
missing isolation or recovery requirement stays blocked; it does not consume a
concurrency slot.
