# INSTALL MANUAL GPV2

## Purpose

This guide explains how to install `ORA_CORE_OS` manually using the `GPV2` documents in this repository.

This is a manual installation guide, not an automated installer.

## Installation Goal

The goal is to reproduce a working structured setup with:
- one coherent master configuration
- 22 internal modules
- a clear reading and execution order
- stable memory and quality gates
- a consistent output layer

## What You Need Before Installing

- a workspace where you can maintain source-of-truth files
- a place to store your master prompt or master profile
- a project structure where modules can be referenced individually
- a way to separate public outputs from internal architecture

Recommended setup:
1. one master project for `ORA_CORE_OS`
2. one folder for `GPV2` documents
3. one file or prompt for the master architecture
4. one file per module
5. one manifest file for module order and dependencies

## Source Files To Use

Read and install from these files:
1. [ORA_CORE_OS_22_Modules_GPV2.md](ORA_CORE_OS_22_Modules_GPV2.md)
2. [GPV2/README.md](GPV2/README.md)
3. [GPV2/modules_manifest.json](GPV2/modules_manifest.json)
4. [GPV2/modules/README.md](GPV2/modules/README.md)
5. [GPV2/usage_map.gpv2.json](GPV2/usage_map.gpv2.json)

## Installation Model

The recommended manual installation model is:
1. install the master architecture
2. install the 4 section groups
3. install the 22 modules in code order
4. wire module dependencies
5. validate usage blocks
6. test end-to-end outputs

## Step 1 - Install the Master Architecture

Use the `MASTER` block as the top-level source of truth.

You should preserve:
- architecture purpose
- section order
- public profile
- usage blocks

Minimum required fields:
- `META.ID`
- `META.VERSION`
- `SECTIONS`
- `USAGE_BLOCKS`

## Step 2 - Create the 4 Section Groups

Create these four groups exactly:
1. `S1 - ORCHESTRATION_GOUVERNANCE`
2. `S2 - POSITIONNEMENT_SIGNALISATION`
3. `S3 - MEMOIRE_APPRENTISSAGE`
4. `S4 - PIPELINE_PRODUCTION`

Do not flatten the system too early. The section grouping is what keeps the system readable.

## Step 3 - Install the 22 Modules In Order

Install in this order:
1. `M01 VOCAL_SI`
2. `M02 LOCK`
3. `M03 PRIMORDIA`
4. `M04 RESPIRA`
5. `M05 AURA_MXB`
6. `M06 RIME`
7. `M07 MR_NET`
8. `M08 MR_PROPRE`
9. `M09 AUDIT`
10. `M10 ARCH_PLUS`
11. `M11 PRIORITY_MATRIX`
12. `M12 REM`
13. `M13 REM_PLUS`
14. `M14 ECHOTWIN`
15. `M15 NEUTRINO`
16. `M16 ORA_N6`
17. `M17 JSON`
18. `M18 EN`
19. `M19 FR`
20. `M20 GL`
21. `M21 GL_G`
22. `M22 NATIVE_FINAL`

## Step 4 - Respect Dependency Wiring

Each module file declares:
- `DEPENDS_ON`
- `USED_IN`
- `INPUTS`
- `OUTPUTS`

Manual installation rule:
- do not activate a module if its required upstream dependencies are missing
- do not expose a public workflow until `CONTROL` and `MEMORY` paths are defined

Critical dependency paths:
1. `VOCAL_SI -> RESPIRA -> JSON -> EN/FR/GL -> GL_G -> NATIVE_FINAL`
2. `LOCK -> PRIMORDIA -> RIME -> MR_NET/MR_PROPRE -> AUDIT`
3. `ARCH_PLUS -> PRIORITY_MATRIX -> FR`
4. `REM -> REM_PLUS -> ECHOTWIN -> NEUTRINO -> ORA_N6`

## Step 5 - Configure the 4 Usage Blocks

Expose the system externally through these blocks:

`SETUP`
- modules: `M10 M11 M13 M16`
- output: profile sheet, priority map, memory base, canon index

`EXECUTION`
- modules: `M01 M04 M17 M18 M19 M20 M21 M22`
- output: summaries, drafts, structured outputs, checklists

`CONTROL`
- modules: `M02 M03 M05 M06 M07 M08 M09`
- output: control, truth check, risk cleanup, audit trace

`MEMORY`
- modules: `M12 M13 M14 M15 M16`
- output: memory state, patterns, signals, canon updates

## Step 6 - Keep The Public Surface Simpler Than The Internal System

Recommended rule:
- internal complexity stays in GPV2
- public behavior stays simple

The public surface should present:
- one system
- one memory layer
- one quality layer
- one consistent output layer

## Step 7 - Validate The Installation

Validation checklist:
1. `SETUP` can produce a profile sheet
2. `EXECUTION` can produce a clean structured output
3. `CONTROL` can flag uncertainty and risky claims
4. `MEMORY` can preserve useful information between runs
5. `NATIVE_FINAL` does not invent facts outside `GL`

## Step 8 - Recommended Manual Tests

Run these tests after installation:
1. feed a vague project brief and confirm `VOCAL_SI` routes it correctly
2. feed risky or uncertain claims and confirm `PRIMORDIA` or `GL` tags them correctly
3. generate one structured output and confirm `FR` respects `ARCH_PLUS` and `PRIORITY_MATRIX`
4. store one persistent project fact and confirm `REM_PLUS` and `ORA_N6` can recover it
5. generate one final output and confirm `NATIVE_FINAL` adds no unsupported facts

## Minimum Viable Manual Installation

If you want the fastest usable version, install these first:
1. `M01 VOCAL_SI`
2. `M03 PRIMORDIA`
3. `M06 RIME`
4. `M10 ARCH_PLUS`
5. `M11 PRIORITY_MATRIX`
6. `M13 REM_PLUS`
7. `M17 JSON`
8. `M19 FR`
9. `M20 GL`
10. `M22 NATIVE_FINAL`

This is the smallest coherent ORA_CORE_OS base.

## Files To Maintain As Source Of Truth

Keep these synchronized:
1. master architecture file
2. usage map file
3. modules manifest
4. one file per module
5. installation guides

If these drift apart, the installation becomes interpretive instead of reliable.
