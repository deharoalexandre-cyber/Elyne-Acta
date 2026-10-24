# Architecture — Elyne Acta

[Français](architecture.md) · [Overview](../README.en.md)

## Simplified flow

Request → EIE and Acta orchestration → tool proposal → application check → scoped execution → Acta memory and ledger.

## Components and boundaries

- Acta uses a local application, EIE inference engine, SQLite WAL state, and FTS5 retrieval combined with multilingual embeddings.
- Its cognitive ledger is Acta-specific: SHA-256 chaining, HMAC authentication, and an anchor in the described profile. It does not replace EAS Defense's ledger or decisions.
- The code workspace and network tools are distinct from conversation. Confinement and permissions must be verified for the deployed service and version, not inferred from their description.

This textual flow describes the product architecture. It does not replace verification on a specific build, hardware profile, and configuration. The [evidence summary](evidence.en.md) states what is actually documented.
