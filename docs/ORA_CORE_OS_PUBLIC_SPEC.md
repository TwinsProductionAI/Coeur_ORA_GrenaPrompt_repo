# ORA_CORE_OS Public Spec

## Status

This document is the public reference specification for `ORA_CORE_OS` as published in this repository.

Scope of this document:
- define what ORA_CORE_OS is
- define what is canonical
- define what is installable
- define what stays in scope publicly
- define how optional annexes extend the public core without changing it

## Scope

`ORA_CORE_OS` is published here as:
- a modular architecture
- a GPV2 specification
- a manual installation system
- a Custom GPT installation source
- an optional annex extension surface

It is not published here as:
- a visual asset repository
- a general ORA archive
- an executable runtime package
- a multi-project bundle

## Canonical Public Files

The canonical public files are:
1. [ORA_CORE_OS_22_Modules_GPV2.md](ORA_CORE_OS_22_Modules_GPV2.md)
2. [GPV2/master_architecture.gpv2.json](GPV2/master_architecture.gpv2.json)
3. [GPV2/usage_map.gpv2.json](GPV2/usage_map.gpv2.json)
4. [GPV2/modules_manifest.json](GPV2/modules_manifest.json)
5. [GPV2/modules/README.md](GPV2/modules/README.md)
6. [GPV2/annexes_manifest.json](GPV2/annexes_manifest.json)
7. [GPV2/annexes/README.md](GPV2/annexes/README.md)
8. [INSTALL_MANUAL_GPV2.md](INSTALL_MANUAL_GPV2.md)
9. [INSTALL_CUSTOM_GPT.md](INSTALL_CUSTOM_GPT.md)

If these files drift apart, the repository becomes less reliable as a spec.

## Public Architecture Model

ORA_CORE_OS is organized in 4 section groups.

`S1 - ORCHESTRATION_GOUVERNANCE`
- routing
- constraints
- truth gates
- quality and audit controls

`S2 - POSITIONNEMENT_SIGNALISATION`
- profile shaping
- priority shaping

`S3 - MEMOIRE_APPRENTISSAGE`
- working memory
- persistent memory
- feedback loops
- weak signal detection
- canon indexing

`S4 - PIPELINE_PRODUCTION`
- structure
- technical layer
- natural language layer
- truth layer
- indexing layer
- final actionable output

## Canonical Module Order

The canonical install order is the `CODE_POS` order:
- `M01` through `M22`

This order is authoritative for:
- manual installation
- Custom GPT assembly
- modular project setup
- documentation cross-reference

## Optional Public Annexes

Optional annexes are allowed publicly only if they respect all of these rules:
1. they do not change the `22` core module count
2. they do not renumber themselves as `M23+`
3. they declare which core module they extend
4. they remain installable only after the core system is coherent
5. they do not silently replace a canonical core module

Current public annex:
- `AX01 GIBBERLINK_GLYPH`
  - extends `M21_GL_G`
  - adds an optional glyph and phonetic bridge layer
  - does not modify the canonical `M01 -> M22` order

## Canonical Public Invariants

These rules define the public behavior of ORA_CORE_OS in this repository:

1. `CODE_POS` is the authoritative module position for the core `22`.
2. `DEPENDS_ON` is authoritative for dependency wiring.
3. `CLIENT_VISIBLE` controls what may be surfaced externally.
4. `NATIVE_FINAL` must not add facts unsupported by `GL`.
5. `GL` is the truth and uncertainty layer.
6. `GPV2` files are the installable source of truth.
7. The public repo must stay limited to ORA_CORE_OS.
8. Public docs must remain synchronized with the canonical files.
9. Annexes may extend but must not silently mutate the core graph.

## Install Surfaces

This repository supports three public install surfaces:

`Manual GPV2`
- install the master architecture
- install the 22 core modules in `CODE_POS` order
- wire dependencies
- validate usage blocks
- optionally add annexes after the core install is stable

`Custom GPT`
- upload the ORA_CORE_OS GPV2 knowledge files
- use a strict ORA_CORE_OS instruction layer
- preserve the same module and truth rules
- optionally upload annexes as explicit add-ons only

`Modular Project`
- keep one file per core module
- use the manifest as routing and install reference
- preserve section grouping and usage mapping
- keep annexes separate from the core module set

## Public Exclusions

The public repository must exclude:
- unrelated image libraries
- side documentation outside ORA_CORE_OS
- non-core project bundles
- materials that are not required to install or study ORA_CORE_OS

## Recommended Verification

A public ORA_CORE_OS install is considered coherent if:
1. the master architecture loads cleanly
2. the 22 core modules are present
3. the manifest points to every core module file
4. `CODE_POS` order is stable
5. `NATIVE_FINAL` obeys `GL`
6. usage blocks map cleanly to the core module graph
7. any optional annex declares its extension target explicitly

## Versioning Rule

When ORA_CORE_OS changes publicly, update in sync:
- the public spec
- the single-file GPV2 reference
- the core manifest
- the annex manifest if annexes changed
- the split core module files
- the annex files if annexes changed
- the install guides
