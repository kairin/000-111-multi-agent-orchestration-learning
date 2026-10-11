# Contributing to the orchestration learning repository

This repository is a documentation-only learning resource. Contributions should
improve the curriculum, evidence labels, exercises, navigation, or historical
source mapping. They must not revive, install, build, or extend OpenRig.

## Propose a bounded change

Name the learning outcome, bounded evidence input, expected paper artifact,
completion check, exclusions, and stop point. Keep observed historical facts
separate from teaching examples. Cite public, redacted evidence.

## Verify documentation

Check changed links, headings, coverage accounting, and instruction boundaries.
Run the local documentation quality baseline and the portability report test.
Do not install dependencies or execute files under
`archive/openrig-0.5.16-source/`.

The active portability workflow uses `scripts/portability-report.mjs`. Historical
build and test commands in archived documents are evidence, not contribution
requirements.

## Preserve provenance

Do not edit immutable release notes, captured evidence, license texts, or
archived historical bytes to modernize their wording. Update
[the source map](../breakdown/HISTORICAL-SOURCE-MAP.md) if a historical file's
physical location changes.
