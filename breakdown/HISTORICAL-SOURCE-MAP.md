# Historical source map

## Boundary

The historical OpenRig runtime and build tree is stored under
`archive/openrig-0.5.16-source/`. This is a physical evidence boundary: files
inside it are retained for source analysis and are not a current project,
dependency set, installation target, or executable exercise.

The snapshot is the repository state used by this curriculum. It includes
historical upstream source, later derivative work, and teaching annotations
that were already present when the tree moved. It is not described as a
pristine upstream checkout. The upstream attribution, licenses, notice, release
history, and original README remain at the repository root or their documented
provenance paths.

## Mapping rule

Each archived file keeps its old path below the boundary:

```text
old: packages/daemon/src/index.ts
new: archive/openrig-0.5.16-source/packages/daemon/src/index.ts
```

The same prefix rule applies to the archived `packages/`, `config/`, and
`spike/` trees; historical build manifests; historical executable files from
`demo/`, `docker/`, `skills/`, and `scripts/`; and the original GitHub issue and
pull-request templates. Contextualized learning documents and fixtures remain
at their active paths.

The machine-readable
[HISTORICAL-SOURCE-MANIFEST.tsv](HISTORICAL-SOURCE-MANIFEST.tsv) records the
pre-move Git blob SHA-1, old path, and new path for all 2,820 moved files. A
validator can hash each destination as a Git blob and compare it with the first
column without executing the historical source.

## Active repository code

The portability report remains active repository governance:

- `.github/workflows/portability-report.yml`
- `scripts/portability-report.mjs`
- `scripts/portability-report.test.mjs`

It examines proposed documentation changes and has no OpenRig runtime or package
dependency. The workflow, its script, `.git`, licenses, notices, curriculum,
and current learning contribution templates are outside the historical runtime
boundary.

## Reading legacy references

Current curriculum and reference documents cite the archived destination paths.
Immutable changelog, captured evidence, and original-source documents preserve
their historical path spelling. Resolve one of those legacy paths by looking it
up in the TSV ledger or by prefixing
`archive/openrig-0.5.16-source/` when the entry appears in the ledger.
