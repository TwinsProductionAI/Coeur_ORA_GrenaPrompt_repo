# Coeur ORA and GrenaPrompt

Public documentation repository for `Coeur ORA`, `ORA CORE OS`, and the `GrenaPrompt` / `GPV2` architecture.

This repository documents a modular AI operating architecture designed to support one clear client-facing offer:
- `ORA Brand and Sales Copilot`

The goal is not to publish raw complexity. The goal is to make the system:
- understandable
- installable
- auditable
- modular

## What This Repository Contains

`Coeur ORA` is documented here as a layered architecture:
- orchestration and governance
- positioning and persuasion
- memory and learning
- production pipeline

`GrenaPrompt` and `GPV2` are used as structural formats to make the system:
- readable by humans
- stable across iterations
- easier to diff, maintain, and install manually

## Recommended Reading Path

If you want the public overview, read in this order:
1. [README.md](README.md)
2. [docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md](docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md)
3. [docs/INSTALL_MANUAL_GPV2.md](docs/INSTALL_MANUAL_GPV2.md)
4. [docs/GPV2/README.md](docs/GPV2/README.md)
5. [docs/GPV2/modules_manifest.json](docs/GPV2/modules_manifest.json)

If you want the raw 22-module architecture:
1. [docs/ORA_CORE_OS_22_Modules_GPV2.md](docs/ORA_CORE_OS_22_Modules_GPV2.md)
2. [docs/GPV2/modules/README.md](docs/GPV2/modules/README.md)

## Repository Structure

- [docs/Architecture_et_Commandes.md](docs/Architecture_et_Commandes.md)
Classic architecture and commands overview.

- [docs/Chronologie_ORA.md](docs/Chronologie_ORA.md)
Project timeline and milestones.

- [docs/FGP_GrenaPrompt.md](docs/FGP_GrenaPrompt.md)
Framework-level principles and specifications.

- [docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md](docs/ORA_CORE_OS_Architecture_22_Modules_Offre_Client.md)
Business-facing interpretation of the 22-module architecture.

- [docs/ORA_CORE_OS_22_Modules_GPV2.md](docs/ORA_CORE_OS_22_Modules_GPV2.md)
Single-file GPV2 reference for the full architecture.

- [docs/INSTALL_MANUAL_GPV2.md](docs/INSTALL_MANUAL_GPV2.md)
Manual installation guide for setting up the system.

- [docs/GPV2/README.md](docs/GPV2/README.md)
Entry point for the modular GPV2 layout.

- [docs/GPV2/modules_manifest.json](docs/GPV2/modules_manifest.json)
Machine-readable index of the 22 modules.

- [docs/GPV2/modules/README.md](docs/GPV2/modules/README.md)
One file per GPV2 module.

## What GPV2 Is Used For Here

In this repository, `GPV2` is used as a packaging format for:
- master architecture
- module metadata
- installation order
- business mapping
- inputs, outputs, and dependencies

That makes the project easier to:
- publish
- install manually
- clone into a Custom GPT or structured project workflow
- maintain over time

## Current Status

This repository is currently strongest as:
- a documentation release
- a modular architecture reference
- a manual installation base

It is not yet presented here as a packaged runtime or SaaS product.

## Publishing Position

The strongest public position for this project is:
- document the architecture clearly
- show how it can be installed manually
- expose the modular system cleanly
- keep the client-facing offer simpler than the internal complexity

## License

See [LICENSE](LICENSE).

