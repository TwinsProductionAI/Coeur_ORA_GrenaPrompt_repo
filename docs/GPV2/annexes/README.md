# Annex Index

This folder contains optional public annex modules for `ORA_CORE_OS`.

Core rule:
- annexes do not change the canonical `22` core modules
- annexes do not change the `M01 -> M22` install order
- annexes must declare which core module they extend

## Annexes

- `AX01` [GIBBERLINK_GLYPH](AX01_GIBBERLINK_GLYPH.gpv2.json)
  - type: `ANNEX_MODULE`
  - extends: `M21_GL_G`
  - role: optional glyph and phonetic bridge above the core compression layer

## Usage Rule

Install annexes only after the 22 core modules are already coherent.

For `AX01`:
- keep `M21_GL_G` authoritative for indexing and compression
- use `AX01` only if you want an extra Gibberlink glyph/phonetic layer
- do not renumber it as `M23`
