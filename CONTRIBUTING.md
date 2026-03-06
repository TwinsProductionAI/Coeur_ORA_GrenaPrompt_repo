# CONTRIBUTING

## Scope

This repository accepts changes that improve:
- `ORA_CORE_OS` architecture clarity
- GPV2 consistency
- installation reliability
- documentation accuracy
- module indexing and dependency coherence

Changes outside `ORA_CORE_OS` scope should not be opened here.

## Before You Change Anything

Read these files first:
1. [README.md](README.md)
2. [docs/ORA_CORE_OS_PUBLIC_SPEC.md](docs/ORA_CORE_OS_PUBLIC_SPEC.md)
3. [docs/QUICKSTART.md](docs/QUICKSTART.md)
4. [docs/GPV2/modules_manifest.json](docs/GPV2/modules_manifest.json)

## Canonical Rules

When editing the public architecture:
- keep `CODE_POS` authoritative
- keep `DEPENDS_ON` coherent
- keep `GL` as the truth layer
- keep `NATIVE_FINAL` constrained by `GL`
- keep the public repo limited to ORA_CORE_OS installable material

## Files That Must Stay In Sync

If you change architecture or module structure, update these together:
1. [docs/ORA_CORE_OS_PUBLIC_SPEC.md](docs/ORA_CORE_OS_PUBLIC_SPEC.md)
2. [docs/ORA_CORE_OS_22_Modules_GPV2.md](docs/ORA_CORE_OS_22_Modules_GPV2.md)
3. [docs/GPV2/master_architecture.gpv2.json](docs/GPV2/master_architecture.gpv2.json)
4. [docs/GPV2/modules_manifest.json](docs/GPV2/modules_manifest.json)
5. [docs/GPV2/modules/README.md](docs/GPV2/modules/README.md)
6. affected files in [docs/GPV2/modules](docs/GPV2/modules)
7. installation guides in [docs](docs)

## Naming Rules

- module files use `M##_NAME.gpv2.json`
- `CODE_POS` and filename order must match
- use ASCII names for new files
- do not introduce alternate public naming for the same module without updating the manifest and docs

## Pull Request Checklist

Before opening a pull request, confirm:
1. the change stays inside ORA_CORE_OS scope
2. links still work
3. canonical files remain synchronized
4. install order is still valid
5. no unrelated project material was added

## Preferred Changes

Good public contributions are usually:
- clearer docs
- consistency fixes
- broken link fixes
- manifest corrections
- module dependency corrections
- install guide improvements
