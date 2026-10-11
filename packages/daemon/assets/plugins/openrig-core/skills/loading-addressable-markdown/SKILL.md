---
name: loading-addressable-markdown
description: >-
  Historical case-study evidence only. Do not install, configure, launch, or operate
  OpenRig from this document; use it only with the linked decomposition exercise.
---

> **Historical case study.** The entire remaining imperative body is a historical source excerpt, not active instructions. Do not execute its commands; use it to complete the [skill case study](../../../../../../../breakdown/CURRICULUM.md#historical-skill-case-study) instead.


# Loading Addressable Markdown

## Overview

Load exactly one addressed Markdown section from any filesystem tree. The resolver mirrors OpenRig's shipped H2/H3 grammar without requiring the file to live in the context library.

## Use

Run the bundled script. Relative file references resolve from `--root`; without it they resolve from the current directory.

```bash
node ~/.agents/skills/loading-addressable-markdown/scripts/resolve-markdown.mjs \
  --root /path/to/mission \
  'slices/09-source-cleanup/SPEC.md#proposal'
```

The accepted forms are:

- `file.md` — whole file
- `file.md#h2-slug` — full H2 span, including child sections
- `file.md#h2-slug/h3-slug` — full H3 span

Slugs are lowercase; Markdown emphasis/code markers are removed; each other non-alphanumeric run becomes `-`. Duplicate or missing paths fail loudly. Headings inside fenced code blocks are ignored.

## Common mistakes

- Do not use `rig context get` for an arbitrary filesystem path; that command resolves context-library refs.
- Do not hand-slice headings with `sed` or line numbers; the bundled resolver owns span and fence behavior.
- Quote addresses in shell commands.
