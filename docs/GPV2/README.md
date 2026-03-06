# GPV2 Index

This folder contains the modular GPV2 release for `ORA_CORE_OS`.

If you are new to the repository, start with [../QUICKSTART.md](../QUICKSTART.md).

## Files

- [master_architecture.gpv2.json](master_architecture.gpv2.json)
Top-level architecture, section grouping, and usage blocks.

- [usage_map.gpv2.json](usage_map.gpv2.json)
Neutral runtime block mapping for setup, execution, control, and memory.

- [modules_manifest.json](modules_manifest.json)
Machine-readable index of all 22 modules.

- [modules/README.md](modules/README.md)
One GPV2 file per module.

## Installation Order

Follow this order:
1. `master_architecture.gpv2.json`
2. `modules_manifest.json`
3. `modules/M01_...` through `modules/M22_...`
4. `usage_map.gpv2.json`
5. [../INSTALL_MANUAL_GPV2.md](../INSTALL_MANUAL_GPV2.md)
6. [../INSTALL_CUSTOM_GPT.md](../INSTALL_CUSTOM_GPT.md)

## Sections

- `S1` orchestration and governance
- `S2` positioning and signal shaping
- `S3` memory and learning
- `S4` production pipeline

## Notes

- `CODE_POS` is the canonical install order.
- `CLIENT_VISIBLE` marks which modules can be surfaced externally.
- `DEPENDS_ON` should be respected during manual installation.
- keep `master_architecture`, `usage_map`, and the module files synchronized.
