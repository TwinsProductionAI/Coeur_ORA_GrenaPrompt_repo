# INSTALL CUSTOM GPT

## Purpose

This guide explains how to install `ORA_CORE_OS` inside a Custom GPT while staying strictly inside the public ORA_CORE_OS scope.

This guide uses only the ORA_CORE_OS documents published in this repository.

## Goal

The goal is to build a Custom GPT that:
- uses ORA_CORE_OS as its architecture base
- respects the 22-module GPV2 structure
- keeps the same truth, dependency, and output rules
- does not pull in unrelated ORA materials

## Files To Use

Use only these knowledge files:
1. [GPV2/master_architecture.gpv2.json](GPV2/master_architecture.gpv2.json)
2. [GPV2/business_usage.gpv2.json](GPV2/business_usage.gpv2.json)
3. [GPV2/modules_manifest.json](GPV2/modules_manifest.json)
4. [GPV2/modules/M01_VOCAL_SI.gpv2.json](GPV2/modules/M01_VOCAL_SI.gpv2.json)
5. [GPV2/modules/M02_LOCK.gpv2.json](GPV2/modules/M02_LOCK.gpv2.json)
6. [GPV2/modules/M03_PRIMORDIA.gpv2.json](GPV2/modules/M03_PRIMORDIA.gpv2.json)
7. [GPV2/modules/M04_RESPIRA.gpv2.json](GPV2/modules/M04_RESPIRA.gpv2.json)
8. [GPV2/modules/M05_AURA_MXB.gpv2.json](GPV2/modules/M05_AURA_MXB.gpv2.json)
9. [GPV2/modules/M06_RIME.gpv2.json](GPV2/modules/M06_RIME.gpv2.json)
10. [GPV2/modules/M07_MR_NET.gpv2.json](GPV2/modules/M07_MR_NET.gpv2.json)
11. [GPV2/modules/M08_MR_PROPRE.gpv2.json](GPV2/modules/M08_MR_PROPRE.gpv2.json)
12. [GPV2/modules/M09_AUDIT.gpv2.json](GPV2/modules/M09_AUDIT.gpv2.json)
13. [GPV2/modules/M10_ARCH_PLUS.gpv2.json](GPV2/modules/M10_ARCH_PLUS.gpv2.json)
14. [GPV2/modules/M11_SONCAS.gpv2.json](GPV2/modules/M11_SONCAS.gpv2.json)
15. [GPV2/modules/M12_REM.gpv2.json](GPV2/modules/M12_REM.gpv2.json)
16. [GPV2/modules/M13_REM_PLUS.gpv2.json](GPV2/modules/M13_REM_PLUS.gpv2.json)
17. [GPV2/modules/M14_ECHOTWIN.gpv2.json](GPV2/modules/M14_ECHOTWIN.gpv2.json)
18. [GPV2/modules/M15_NEUTRINO.gpv2.json](GPV2/modules/M15_NEUTRINO.gpv2.json)
19. [GPV2/modules/M16_ORA_N6.gpv2.json](GPV2/modules/M16_ORA_N6.gpv2.json)
20. [GPV2/modules/M17_JSON.gpv2.json](GPV2/modules/M17_JSON.gpv2.json)
21. [GPV2/modules/M18_EN.gpv2.json](GPV2/modules/M18_EN.gpv2.json)
22. [GPV2/modules/M19_FR.gpv2.json](GPV2/modules/M19_FR.gpv2.json)
23. [GPV2/modules/M20_GL.gpv2.json](GPV2/modules/M20_GL.gpv2.json)
24. [GPV2/modules/M21_GL_G.gpv2.json](GPV2/modules/M21_GL_G.gpv2.json)
25. [GPV2/modules/M22_NATIVE_FINAL.gpv2.json](GPV2/modules/M22_NATIVE_FINAL.gpv2.json)

Do not upload unrelated docs, images, or non-ORA_CORE_OS assets.

## Recommended Custom GPT Setup

Use this layout:
1. `Instructions`
2. `Knowledge`
3. `Optional actions only if strictly needed`

For a first installation, you do not need custom actions.

## Knowledge Upload Order

Upload in this order:
1. `master_architecture.gpv2.json`
2. `modules_manifest.json`
3. all 22 module files in `CODE_POS` order
4. `business_usage.gpv2.json`

This order reduces ambiguity and helps keep the master architecture above module-level detail.

## Suggested Instruction Layer

Use a system instruction similar to this:

```text
You operate strictly from ORA_CORE_OS.
Use only the ORA_CORE_OS GPV2 knowledge uploaded to this GPT.
Treat GPV2 as the structural source of truth.
Respect the 22 modules and their CODE_POS ordering from M01 to M22.
Respect DEPENDS_ON when composing behavior.
Use CLIENT_BLOCKS and USED_IN to map requests to the right functional path.
Do not invent extra modules, extra architecture, or external lore.
Keep outputs consistent with the truth constraints of GL.
NATIVE_FINAL must not introduce facts unsupported by GL.
If required information is missing, state uncertainty clearly instead of inventing certainty.
Keep the external behavior simpler than the internal architecture.
```

## Recommended Behavior Policy

The Custom GPT should behave like this:
- use ORA_CORE_OS only
- route through the published module graph
- keep public language clear and usable
- expose simple outputs, not raw architectural complexity
- preserve uncertainty tags when facts are missing

## Recommended Install Logic

Map incoming requests using these public blocks:

`ONBOARDING`
- `M10 M11 M13 M16`

`PRODUCTION`
- `M01 M04 M17 M18 M19 M20 M21 M22`

`QUALITY`
- `M02 M03 M05 M06 M07 M08 M09`

`RETENTION`
- `M12 M13 M14 M15 M16`

## What Not To Do In Custom GPT

Do not:
- add unrelated ORA assets
- merge in non-ORA_CORE_OS documents
- bypass `GL` when producing final outputs
- skip `CODE_POS` and dependency logic completely
- expose the full internal complexity unless explicitly needed

## Validation Tests

After building the Custom GPT, test it with these prompts:

1. `Create a clean onboarding summary for a new client brand.`
Expected result:
- persona and persuasion logic appear
- no unsupported factual claims

2. `Write a sales email from a vague brief.`
Expected result:
- route through production behavior
- output is actionable and coherent

3. `What should you do if a claim is uncertain?`
Expected result:
- explicit uncertainty handling
- no fake certainty

4. `Summarize your architecture briefly.`
Expected result:
- simple public explanation
- not a lore dump

## Minimum Viable Custom GPT Install

If file count is a problem, minimum recommended upload set:
1. `master_architecture.gpv2.json`
2. `modules_manifest.json`
3. `M01_VOCAL_SI.gpv2.json`
4. `M03_PRIMORDIA.gpv2.json`
5. `M10_ARCH_PLUS.gpv2.json`
6. `M11_SONCAS.gpv2.json`
7. `M13_REM_PLUS.gpv2.json`
8. `M17_JSON.gpv2.json`
9. `M19_FR.gpv2.json`
10. `M20_GL.gpv2.json`
11. `M22_NATIVE_FINAL.gpv2.json`

This is not the full architecture, but it is the smallest coherent ORA_CORE_OS Custom GPT base.

## Best Practice

Keep the Custom GPT aligned with these files whenever the repo changes:
- `ORA_CORE_OS_PUBLIC_SPEC.md`
- `master_architecture.gpv2.json`
- `modules_manifest.json`
- split module files

If those drift apart, the GPT install will become interpretive instead of controlled.
