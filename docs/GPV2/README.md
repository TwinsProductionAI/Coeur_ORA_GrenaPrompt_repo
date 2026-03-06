# GPV2 Index

This folder contains the modular GPV2 release for `ORA CORE OS`.

## Files

- [master_architecture.gpv2.json](master_architecture.gpv2.json)
Top-level architecture, section grouping, and business blocks.

- [business_usage.gpv2.json](business_usage.gpv2.json)
Business-facing block mapping for onboarding, production, quality, and retention.

- [modules_manifest.json](modules_manifest.json)
Machine-readable index of all 22 modules.

- [modules/README.md](modules/README.md)
One GPV2 file per module.

## Installation Order

Follow this order:
1. `master_architecture.gpv2.json`
2. `modules_manifest.json`
3. `modules/M01_...` through `modules/M22_...`
4. `business_usage.gpv2.json`
5. [../INSTALL_MANUAL_GPV2.md](../INSTALL_MANUAL_GPV2.md)

## Sections

- `S1` orchestration and governance
- `S2` positioning and persuasion
- `S3` memory and learning
- `S4` production pipeline

## Notes

- `CODE_POS` is the canonical install order.
- `CLIENT_VISIBLE` marks which modules can be surfaced externally.
- `DEPENDS_ON` should be respected during manual installation.

