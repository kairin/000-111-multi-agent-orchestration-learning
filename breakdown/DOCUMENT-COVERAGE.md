# Documentation coverage ledger

## Baseline

At curriculum creation, the repository contained 518 tracked documentation and
instructional files: 401 Markdown, 110 YAML, 4 YML, and 3 HTML files. The groups
below are exhaustive for that baseline. New curriculum files are listed
separately and do not change the baseline counts.

| Baseline group | Count | Classification | Treatment and reason |
|---|---:|---|---|
| Root `*.md` | 4 | Entry point + immutable history/legal record | Rewrite `README.md` and `AGENTS.md`; preserve `CHANGELOG.md` and `COMMERCIAL.md` as records. |
| `breakdown/` | 54 | Curriculum candidates + research evidence | Rewrite the route and active planning narrative; preserve cited observations and label proposed or historical content. |
| `docs/` | 85 | Historical manuals and release evidence | Replace operational entrypoint authority with study routing; preserve versioned factual modules and release notes. |
| `skills/` | 46 | Historical executable agent instructions | Disable operational discovery/authority and route each skill family to an analysis exercise; preserve examples as primary sources. |
| `packages/` | 291 | Embedded specifications, fixture prose/YAML, and package manuals | Contextualize active README/manual entrypoints; preserve 100 YAML fixtures, 2 static HTML files, and leaf specifications as implementation evidence. |
| `docker/` | 11 | Historical runbooks and YAML fixtures | Convert runbook entrypoints to study cases; preserve fixture data. |
| `demo/` | 9 | Historical demo instructions and YAML topology examples | Replace run authority with an orchestration-analysis exercise; preserve seven YAML examples. |
| `.github/` | 9 | Historical community docs and workflows | Mark prose as archive context; preserve four workflow YML files as evidence. |
| `.evidence/` | 6 | Captured evidence | Preserve verbatim. These files support historical claims and are not exercises. |
| `archive/` | 1 | Original upstream README | Preserve verbatim as provenance evidence and route readers back to the curriculum. |
| `assets/` | 1 | Screenshot evidence index | Contextualize as historical capture metadata. |
| `spike/` | 1 | Historical prototype runbook | Convert its entrypoint into a paper analysis of experiment boundaries. |

| Group | Markdown | YAML | YML | HTML | Total |
|---|---:|---:|---:|---:|---:|
| Root | 4 | 0 | 0 | 0 | 4 |
| `breakdown/` | 53 | 0 | 0 | 1 | 54 |
| `docs/` | 84 | 1 | 0 | 0 | 85 |
| `skills/` | 46 | 0 | 0 | 0 | 46 |
| `packages/` | 189 | 100 | 0 | 2 | 291 |
| `docker/` | 9 | 2 | 0 | 0 | 11 |
| `demo/` | 2 | 7 | 0 | 0 | 9 |
| `.github/` | 5 | 0 | 4 | 0 | 9 |
| `.evidence/` | 6 | 0 | 0 | 0 | 6 |
| `archive/` | 1 | 0 | 0 | 0 | 1 |
| `assets/` | 1 | 0 | 0 | 0 | 1 |
| `spike/` | 1 | 0 | 0 | 0 | 1 |
| **Total** | **401** | **110** | **4** | **3** | **518** |

Changing a release note, fixture, captured result, or versioned as-built claim
would weaken provenance. The repository changes the authority of entrypoints
and automatically discovered instructions, then uses indexes and scoped agent
guidance to establish the boundary for leaf evidence. A leaf file is preserved
when it reports a historical observation or supplies fixture data and does not
act as a current navigation or execution surface.

The baseline contains 90 automatically discoverable `SKILL.md` files: 35 under
`skills/_canonical/` and 55 formerly embedded under `packages/`. The `skills/` group has
46 files because it also includes nine skill references/templates plus its
README and changelog. The `packages/` count includes the second skill copies as
well as specifications and fixtures. Every discovered skill needs historical
discovery metadata and an in-body study boundary; group-level indexing alone is
not sufficient for an automatically loaded instruction.

### Skill study routing

Use the file's path and subject to select a concrete card from the
[historical skill exercise](CURRICULUM.md#historical-skill-case-study):

| Skill family | Files | Required analysis focus |
|---|---:|---|
| Canonical/shared `core/` | 17 canonical + 17 shipped mirrors | Dependency edges, state ownership, recovery interface, and stop condition |
| Canonical/shared `pm/` | 7 + 7 | Decision owner, required input, review artifact, and acceptance evidence |
| Canonical/shared `pods/` | 4 + 4 | Non-overlapping ownership, handoff interface, safe concurrency, and integration verdict |
| Canonical/shared `process/` | 7 + 7 | Verification loop, counter-evidence, bounded rework, and completion check |
| Embedded plugin assets | 19 | Historical side effect, authority boundary, downstream consumer, and failure mode |
| Vault fixture | 1 | Credential boundary, allowed structural evidence, and stop/escalation rule |
| **Total** | **90** | One observable skill-analysis card per selected file |

The mirrored pairs remain separate files in the baseline because both were
discoverable. A learner analyzes one selected file, not all copies.

## Current physical boundary

The baseline tables preserve the paths and counts that existed when the
curriculum was created. The historical runtime and build material now lives
under `archive/openrig-0.5.16-source/`. The exact 2,820-file relocation ledger
is [HISTORICAL-SOURCE-MANIFEST.tsv](HISTORICAL-SOURCE-MANIFEST.tsv); its prose
guide is [HISTORICAL-SOURCE-MAP.md](HISTORICAL-SOURCE-MAP.md).

Current learning documents, fixtures, licenses, notices, captured evidence,
and release history remain outside that runtime boundary. The active
portability workflow retains `scripts/portability-report.mjs` and its test.
Original OpenRig issue and pull-request templates are archived byte-for-byte;
the active `.github` templates now request changes to this learning resource.

New curriculum files are `CURRICULUM.md`, `RESEARCH-EVIDENCE.md`, this ledger,
`HISTORICAL-SOURCE-MAP.md`, `HISTORICAL-SOURCE-MANIFEST.tsv`, and
`gemini-review/AGENTS.md`. Validation must confirm the baseline arithmetic, inspect every active
index, skill, and runbook for current operational authority, and check relative
links in changed Markdown files.
