# Module Index

This folder contains one `GPV2` file per `ORA_CORE_OS` core module.

## Core Modules

- `M01` [VOCAL_SI](M01_VOCAL_SI.gpv2.json) : Intent Router | group `S1`
- `M02` [LOCK](M02_LOCK.gpv2.json) : Constraint Gate | group `S1`
- `M03` [PRIMORDIA](M03_PRIMORDIA.gpv2.json) : Truth Tribunal | group `S1`
- `M04` [RESPIRA](M04_RESPIRA.gpv2.json) : Flow Orchestrator | group `S1`
- `M05` [AURA_MXB](M05_AURA_MXB.gpv2.json) : Decision Scorecard | group `S1`
- `M06` [RIME](M06_RIME.gpv2.json) : Reasoning Compiler | group `S1`
- `M07` [MR_NET](M07_MR_NET.gpv2.json) : Noise Cleaner | group `S1`
- `M08` [MR_PROPRE](M08_MR_PROPRE.gpv2.json) : Risk Cleaner | group `S1`
- `M09` [AUDIT](M09_AUDIT.gpv2.json) : Trace Layer | group `S1`
- `M10` [ARCH_PLUS](M10_ARCH_PLUS.gpv2.json) : Profile Architecture | group `S2`
- `M11` [PRIORITY_MATRIX](M11_PRIORITY_MATRIX.gpv2.json) : Priority Matrix | group `S2`
- `M12` [REM](M12_REM.gpv2.json) : Working Memory | group `S3`
- `M13` [REM_PLUS](M13_REM_PLUS.gpv2.json) : Persistent Memory | group `S3`
- `M14` [ECHOTWIN](M14_ECHOTWIN.gpv2.json) : Mirror Feedback | group `S3`
- `M15` [NEUTRINO](M15_NEUTRINO.gpv2.json) : Weak Signal Detector | group `S3`
- `M16` [ORA_N6](M16_ORA_N6.gpv2.json) : Canon Indexer | group `S3`
- `M17` [JSON](M17_JSON.gpv2.json) : Structured Container | group `S4`
- `M18` [EN](M18_EN.gpv2.json) : Technical Layer | group `S4`
- `M19` [FR](M19_FR.gpv2.json) : Natural Voice Layer | group `S4`
- `M20` [GL](M20_GL.gpv2.json) : Truth Layer | group `S4`
- `M21` [GL_G](M21_GL_G.gpv2.json) : Index Compression Layer | group `S4`
- `M22` [NATIVE_FINAL](M22_NATIVE_FINAL.gpv2.json) : Actionable Output | group `S4`

## Optional Annexes

Optional annexes live in [../annexes/README.md](../annexes/README.md).

Current annex:
- `AX01` `GIBBERLINK_GLYPH` : extends `M21_GL_G` without changing the core `22`

## Notes

- `CODE_POS` is the canonical install order for the core `22`.
- `DEPENDS_ON` defines required upstream module links.
- `USED_IN` shows the main runtime blocks for each core module.
- annex modules are optional and must not be renumbered as `M23+` unless the public architecture itself changes.
