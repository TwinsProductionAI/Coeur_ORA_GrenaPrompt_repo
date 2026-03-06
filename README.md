# ORA_CORE_OS

Public repository focused only on `ORA_CORE_OS` and its `GPV2` architecture.

This repository now keeps a strict scope:
- ORA_CORE_OS architecture
- GPV2 modular documentation
- manual installation documentation
- business-facing ORA_CORE_OS offer mapping

Everything outside this scope is intentionally excluded from the public repository.

## Core Files

- [docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md](docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md)
Business-facing reading of the 22-module architecture.

- [docs/ORA_CORE_OS_22_Modules_GPV2.md](docs/ORA_CORE_OS_22_Modules_GPV2.md)
Single-file GPV2 reference for the full ORA_CORE_OS architecture.

- [docs/INSTALL_MANUAL_GPV2.md](docs/INSTALL_MANUAL_GPV2.md)
Manual installation guide.

- [docs/GPV2/README.md](docs/GPV2/README.md)
Entry point for the modular GPV2 layout.

- [docs/GPV2/modules_manifest.json](docs/GPV2/modules_manifest.json)
Machine-readable index of the 22 modules.

- [docs/GPV2/modules/README.md](docs/GPV2/modules/README.md)
Human-readable index of the split GPV2 modules.

## Recommended Reading Order

1. [README.md](README.md)
2. [docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md](docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md)
3. [docs/INSTALL_MANUAL_GPV2.md](docs/INSTALL_MANUAL_GPV2.md)
4. [docs/GPV2/README.md](docs/GPV2/README.md)
5. [docs/GPV2/modules_manifest.json](docs/GPV2/modules_manifest.json)
6. [docs/GPV2/modules/README.md](docs/GPV2/modules/README.md)

## Scope

This public repo is intentionally limited to `ORA_CORE_OS`.

Excluded from publication:
- visual asset dumps
- background image folders
- character image folders
- UI exploration assets
- unrelated historical or auxiliary docs

## Installation Model

The public installation path is:
1. read the master GPV2 architecture
2. read the install guide
3. use the modules manifest
4. install the 22 modules in `CODE_POS` order

## License

See [LICENSE](LICENSE).
