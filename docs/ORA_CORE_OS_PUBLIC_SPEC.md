# ORA_CORE_OS Public Spec

## Status

This document is the public reference specification for `ORA_CORE_OS` as published in this repository.

Scope of this document:
- define what ORA_CORE_OS is
- define what is canonical
- define what is installable
- define what stays in scope publicly

## Scope

`ORA_CORE_OS` is published here as:
- a modular architecture
- a GPV2 specification
- a manual installation system
- a Custom GPT installation source

It is not published here as:
- a visual asset repository
- a general ORA archive
- a mixed-content brand repository
- an executable runtime package

## Canonical Public Files

The canonical public files are:
1. [ORA_CORE_OS_22_Modules_GPV2.md](ORA_CORE_OS_22_Modules_GPV2.md)
2. [GPV2/master_architecture.gpv2.json](GPV2/master_architecture.gpv2.json)
3. [GPV2/business_usage.gpv2.json](GPV2/business_usage.gpv2.json)
4. [GPV2/modules_manifest.json](GPV2/modules_manifest.json)
5. [GPV2/modules/README.md](GPV2/modules/README.md)
6. [INSTALL_MANUAL_GPV2.md](INSTALL_MANUAL_GPV2.md)
7. [INSTALL_CUSTOM_GPT.md](INSTALL_CUSTOM_GPT.md)

If these files drift apart, the repository becomes less reliable as a spec.

## Public Architecture Model

ORA_CORE_OS is organized in 4 section groups.

`S1 - ORCHESTRATION_GOUVERNANCE`
- routing
- constraints
- truth gates
- quality and audit controls

`S2 - POSITIONNEMENT_PERSUASION`
- persona shaping
- persuasion weighting

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

## Canonical Public Invariants

These rules define the public behavior of ORA_CORE_OS in this repository:

1. `CODE_POS` is the authoritative module position.
2. `DEPENDS_ON` is authoritative for dependency wiring.
3. `CLIENT_VISIBLE` controls what may be surfaced externally.
4. `NATIVE_FINAL` must not add facts unsupported by `GL`.
5. `GL` is the truth and uncertainty layer.
6. `GPV2` files are the installable source of truth.
7. The public repo must stay limited to ORA_CORE_OS.

## Install Surfaces

This repository supports three public install surfaces:

`Manual GPV2`
- install the master architecture
- install the 22 modules in `CODE_POS` order
- wire dependencies
- validate business blocks

`Custom GPT`
- upload the ORA_CORE_OS GPV2 knowledge files
- use a strict ORA_CORE_OS instruction layer
- preserve the same module and truth rules

`Modular Project`
- keep one file per module
- use the manifest as routing and install reference
- preserve section grouping and business mapping

## Business Interpretation

The 22-module architecture should not be sold publicly as 22 separate offers.

Public reading:
- one system
- one installation path
- one client-facing output layer

Internal reading:
- 22 modules
- 4 section groups
- explicit dependencies
- explicit truth and memory controls

## Public Exclusions

The public repository must exclude:
- unrelated image libraries
- character galleries
- UI exploration dumps
- side documentation outside ORA_CORE_OS
- mixed-scope project material

## Recommended Verification

A public ORA_CORE_OS install is considered coherent if:
1. the master architecture loads cleanly
2. the 22 modules are present
3. the manifest points to every module file
4. `CODE_POS` order is stable
5. `NATIVE_FINAL` obeys `GL`
6. business blocks map cleanly to the module graph

## Versioning Rule

When ORA_CORE_OS changes publicly, update in sync:
- the public spec
- the single-file GPV2 reference
- the manifest
- the split module files
- the install guides
