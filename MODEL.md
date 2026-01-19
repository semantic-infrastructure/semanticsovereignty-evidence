# Reference Model — Semantic Sovereignty

**Model name:** Canonical Meaning Control (CMC)  
**Domain:** semanticsovereignty.com  
**Repository:** semanticsovereignty-evidence  
**Version:** v1.0  
**Last updated:** 2026-01-19

---

## Model intent

The CMC model defines a **structural framework** for governing meaning in machine-consumable systems.
It specifies how terms are canonically defined, bounded, versioned, and changed over time.

The model is designed for:
- semantic governance and drift prevention,
- interoperability across systems and datasets,
- audit and lifecycle transparency.

It does **not** evaluate correctness or interpret meaning in context.

---

## Model structure

### Layer 1 — Term Authority

The **term authority** identifies the entity responsible for publishing and maintaining
the canonical definition of a term.

Responsibilities:
- Publish the canonical record
- Maintain version history
- Document deprecations and replacements

Constraints:
- Authority defines reference status, not correctness.
- Authority does not enforce usage.

---

### Layer 2 — Definition Boundary

The **definition boundary** specifies the semantic perimeter of a term.

Components:
- Formal definition
- Included meaning
- Explicit exclusions
- Disambiguation notes

Constraints:
- One concept per canonical identifier
- Boundaries must be explicit and reviewable
- Synonyms map *to* the canonical term, not vice versa

---

### Layer 3 — Change Discipline

The **change discipline** governs how meaning evolves over time.

Mechanisms:
- Semantic versioning
- Deprecation notices
- Replacement mappings
- Migration notes

Constraints:
- No silent changes
- No deletion without record
- All changes are versioned and traceable

---

## Relationships

The CMC model enforces the following relationships:

- **Term Authority → Definition Boundary**  
  Authority publishes and maintains the boundary.

- **Definition Boundary → Change Discipline**  
  Boundary changes are governed by explicit change rules.

There is **no inference** from popularity or usage to authority.

---

## Alignment with sources

The CMC model is conceptually grounded in:
- controlled vocabulary governance (e.g. SKOS),
- semantic representation standards (RDF, OWL),
- constraint and validation patterns (SHACL),
- serialization and context discipline (JSON-LD).

Specific anchors are documented in `SOURCES.md`.

---

## Constraints

- No authority, trust, or reputation scoring is defined.
- No interpretation of natural language meaning is performed.
- No enforcement or legal claims are made.
- The model is classificatory and procedural only.

---

## Change discipline

- Any modification to this model requires:
  - an explicit update to this file, and
  - a corresponding entry in `CHANGELOG.md`.

Deprecated model elements are documented and not removed silently.

---

## Disclaimer

This model defines a governance structure only.  
It does not provide legal advice, enforcement mechanisms, or normative judgments.
