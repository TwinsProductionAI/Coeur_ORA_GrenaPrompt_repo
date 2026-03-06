# ORA_CORE_OS

`ORA_CORE_OS` is a modular architecture specification for building a structured AI copilot from `GPV2` components.

This public repository is intentionally scoped to one thing only:
- the `ORA_CORE_OS` architecture

It does not aim to publish unrelated visual assets, side experiments, or broader project history.

## What ORA_CORE_OS Is

`ORA_CORE_OS` defines a 22-module operating architecture organized into 4 section groups:
- orchestration and governance
- positioning and persuasion
- memory and learning
- production pipeline

The public interpretation of that architecture is simple:
- one modular system
- one install path
- one client-facing output layer

## Public Positioning

The strongest public reading of this repository is:
- a specification
- a manual installation pack
- a modular GPV2 reference

The internal complexity stays in GPV2.
The public surface stays readable.

## Core Reading Order

1. [docs/ORA_CORE_OS_PUBLIC_SPEC.md](docs/ORA_CORE_OS_PUBLIC_SPEC.md)
2. [docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md](docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md)
3. [docs/INSTALL_MANUAL_GPV2.md](docs/INSTALL_MANUAL_GPV2.md)
4. [docs/INSTALL_CUSTOM_GPT.md](docs/INSTALL_CUSTOM_GPT.md)
5. [docs/GPV2/README.md](docs/GPV2/README.md)
6. [docs/GPV2/modules_manifest.json](docs/GPV2/modules_manifest.json)
7. [docs/GPV2/modules/README.md](docs/GPV2/modules/README.md)

## Repository Contents

- [docs/ORA_CORE_OS_PUBLIC_SPEC.md](docs/ORA_CORE_OS_PUBLIC_SPEC.md)
Public reference spec for scope, invariants, structure, and install rules.

- [docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md](docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md)
Business-facing reading of the 22-module architecture.

- [docs/ORA_CORE_OS_22_Modules_GPV2.md](docs/ORA_CORE_OS_22_Modules_GPV2.md)
Single-file GPV2 reference for the full architecture.

- [docs/INSTALL_MANUAL_GPV2.md](docs/INSTALL_MANUAL_GPV2.md)
Manual installation guide.

- [docs/INSTALL_CUSTOM_GPT.md](docs/INSTALL_CUSTOM_GPT.md)
Custom GPT installation guide using the same ORA_CORE_OS source of truth.

- [docs/GPV2/README.md](docs/GPV2/README.md)
Entry point for the modular GPV2 layout.

- [docs/GPV2/modules_manifest.json](docs/GPV2/modules_manifest.json)
Machine-readable module index and install order.

- [docs/GPV2/modules/README.md](docs/GPV2/modules/README.md)
Human-readable module index.

## Architecture At A Glance

Section groups:
- `S1` orchestration and governance
- `S2` positioning and persuasion
- `S3` memory and learning
- `S4` production pipeline

Canonical install order:
- `M01` through `M22`
- `CODE_POS` is authoritative

Core public install surfaces:
- manual GPV2 installation
- Custom GPT installation
- modular project installation from one file per module

## Public Rules

- `ORA_CORE_OS` only
- `GPV2` is the structural source of truth
- `CODE_POS` defines install order
- `DEPENDS_ON` must be respected
- `NATIVE_FINAL` must not add facts unsupported by `GL`
- anything outside ORA_CORE_OS scope stays out of the public repo

## Best Use Of This Repository

Use this repository if you want to:
- study the ORA_CORE_OS architecture
- install it manually
- port it into a Custom GPT or structured AI workspace
- keep the system modular instead of monolithic

## License

See [LICENSE](LICENSE).
