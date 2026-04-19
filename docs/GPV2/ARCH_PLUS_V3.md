# ARCH+ v3 - Persona Genesis Engine

ARCH+ v3 is the advanced M10 variant for identity architecture inside ORA_CORE_OS.
It keeps the canonical `M10` position and extends the existing `ARCH_PLUS` module
instead of creating a new numbered core module.

## Purpose

ARCH+ v3 turns a human, team or company context into an ArchiPersona profile:

- identity and cognitive posture
- mission and reason to exist
- tone and emotional calibration
- risk, audacity and reflective depth
- up to four active Personae
- up to four ARC++ domains or specializations

The module does not invent missing user data. Unknown values stay `INCERTAIN`;
safe defaults are marked `SUGGESTION` until validated by the user.

## Activation Flow

```text
RUN:ARCH_PLUS
  -> scan known context
  -> prefill all six foundation groups
  -> mark fields as USER_PROVIDED, CANON, SUGGESTION or INCERTAIN
  -> run coherence tests
  -> pass through Primordia
  -> produce archipersona_profile + persona_state + arc_plus_plus_map
```

## Modes

`FAST_PREFILL` fills every field from known context and safe suggestions.
It asks only if a blocking field remains missing.

`DEEP_CALIBRATION` runs the full six-question ArchiPersona ritual.

## Six Foundation Groups

1. `context_identity`: role, identity, cognitive posture.
2. `goal_why`: objective, mission, reason to exist.
3. `tone_emo`: tone, emotion profile, intensity.
4. `limits_risk`: risk, audacity, reflective depth.
5. `personae_start`: maximum four active Personae.
6. `arc_plus_plus`: maximum four ARC++ domains.

## ORA_CORE_RAG Boundary

ORA_CORE_RAG may index the public ARCH+ v3 spec, schemas and tests.
It must not write private client profile payloads into the ORA core index.
Client activations require a valid GLK route manifest and tenant-scoped storage.

## Canon Files

- `modules/M10_ARCH_PLUS.gpv2.json`: current minimal M10 baseline.
- `modules/M10_ARCH_PLUS_V3.gpv2.json`: advanced M10 ARCH+ v3 module.
- `tests/M10_ARCH_PLUS_V3.tests.gpv2.json`: declarative validation tests.

## Migration Rule

M10 v1.1.0 remains valid as the compact baseline.
M10 ARCH+ v3 is the preferred profile activation spec when a surcouche needs
structured identity, Personae, ARC++ and RAG-safe activation.