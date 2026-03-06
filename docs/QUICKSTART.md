# QUICKSTART

## Purpose

This guide is the fastest way to understand and evaluate `ORA_CORE_OS`.

Use it if you want to:
- understand the architecture quickly
- inspect the core files in the right order
- test a minimal install path before reading everything

## Fastest Reading Order

Read these files in order:
1. [ORA_CORE_OS_PUBLIC_SPEC.md](ORA_CORE_OS_PUBLIC_SPEC.md)
2. [GPV2/master_architecture.gpv2.json](GPV2/master_architecture.gpv2.json)
3. [GPV2/modules_manifest.json](GPV2/modules_manifest.json)
4. [GPV2/modules/README.md](GPV2/modules/README.md)
5. [INSTALL_MANUAL_GPV2.md](INSTALL_MANUAL_GPV2.md) or [INSTALL_CUSTOM_GPT.md](INSTALL_CUSTOM_GPT.md)

## Minimal Evaluation Set

If you do not want to read the full 22-module release first, inspect this smaller set:
1. [GPV2/master_architecture.gpv2.json](GPV2/master_architecture.gpv2.json)
2. [GPV2/modules_manifest.json](GPV2/modules_manifest.json)
3. [GPV2/modules/M01_VOCAL_SI.gpv2.json](GPV2/modules/M01_VOCAL_SI.gpv2.json)
4. [GPV2/modules/M03_PRIMORDIA.gpv2.json](GPV2/modules/M03_PRIMORDIA.gpv2.json)
5. [GPV2/modules/M10_ARCH_PLUS.gpv2.json](GPV2/modules/M10_ARCH_PLUS.gpv2.json)
6. [GPV2/modules/M11_PRIORITY_MATRIX.gpv2.json](GPV2/modules/M11_PRIORITY_MATRIX.gpv2.json)
7. [GPV2/modules/M13_REM_PLUS.gpv2.json](GPV2/modules/M13_REM_PLUS.gpv2.json)
8. [GPV2/modules/M17_JSON.gpv2.json](GPV2/modules/M17_JSON.gpv2.json)
9. [GPV2/modules/M19_FR.gpv2.json](GPV2/modules/M19_FR.gpv2.json)
10. [GPV2/modules/M20_GL.gpv2.json](GPV2/modules/M20_GL.gpv2.json)
11. [GPV2/modules/M22_NATIVE_FINAL.gpv2.json](GPV2/modules/M22_NATIVE_FINAL.gpv2.json)
12. [GPV2/usage_map.gpv2.json](GPV2/usage_map.gpv2.json)

## What To Check First

When reading the files above, verify these points:
1. `CODE_POS` is consistent from `M01` to `M22`
2. `DEPENDS_ON` makes sense for upstream wiring
3. `GL` remains the truth layer
4. `NATIVE_FINAL` depends on the output and truth layers
5. `usage_map` matches the public install paths

## Fastest Manual Test

To evaluate the architecture manually:
1. load `master_architecture.gpv2.json`
2. load `modules_manifest.json`
3. load the minimal evaluation set above
4. trace one request through `SETUP`, `EXECUTION`, `CONTROL`, and `MEMORY`
5. confirm the final output does not exceed what `GL` can support

## Pick The Next Guide

Choose one next step:
- [INSTALL_MANUAL_GPV2.md](INSTALL_MANUAL_GPV2.md) for a file-driven install
- [INSTALL_CUSTOM_GPT.md](INSTALL_CUSTOM_GPT.md) for a ChatGPT-based install
- [GPV2/modules/README.md](GPV2/modules/README.md) for module-by-module inspection
