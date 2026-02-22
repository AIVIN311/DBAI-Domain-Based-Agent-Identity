# DBAI Versioning Policy

DBAI follows a **Core-stable, Edge-evolving** model.

## Core
Includes:
- Manifest minimum fields
- Resolver verification requirements
- Anchor binding semantics

Core changes are rare and may trigger major version increments.

## Edge
Includes:
- Extensions
- Operational guidance
- Index and ecosystem considerations

Edge changes are non-breaking and may evolve across minor versions.

## Version Semantics
- `v0.x`: Experimental phase; core may change with community feedback
- `v1.0`: Core identity discovery semantics considered stable
- Minor versions (`v1.x`): Backward-compatible improvements
- Major versions (`v2.x`): Core semantic changes (expected to be rare)