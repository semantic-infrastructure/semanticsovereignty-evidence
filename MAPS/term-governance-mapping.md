# Term Governance Mapping — Semantic Sovereignty

**Domain:** semanticsovereignty.com  
**Repository:** semanticsovereignty-evidence  
**Reference model:** Canonical Meaning Control (CMC)  
**Version:** v1.0  
**Last updated:** 2026-01-19

---

## Purpose

This mapping operationalizes the CMC model by defining **which governance elements apply to which semantic objects**.
It ensures consistency across scope, model, and repository artifacts.

This document is classificatory only.

---

## Semantic objects (in scope)

- **Canonical Term**
- **Definition Record**
- **Vocabulary Set**
- **Deprecated Term**
- **Replacement Term**
- **Version Release**

Objects outside this list are out of scope.

---

## Governance elements

- **Authority assignment**
- **Definition boundary**
- **Versioning**
- **Deprecation**
- **Replacement mapping**
- **Migration notes**
- **Publication status**

---

## Object–governance mapping

| Semantic object    | Authority assignment | Definition boundary | Versioning | Deprecation | Replacement | Migration notes |
|--------------------|----------------------|---------------------|------------|-------------|-------------|-----------------|
| Canonical Term     | Required             | Required            | Required   | Optional    | Optional    | Optional        |
| Definition Record  | Required             | Required            | Required   | Optional    | Optional    | Optional        |
| Vocabulary Set     | Required             | Required            | Required   | Optional    | Optional    | Optional        |
| Deprecated Term    | Required             | Frozen              | Required   | Required    | Optional    | Required        |
| Replacement Term   | Required             | Required            | Required   | Optional    | Optional    | Optional        |
| Version Release    | Required             | N/A                 | Required   | N/A         | N/A         | Optional        |

---

## Boundary constraints

- Every **canonical term** must have exactly one authoritative publisher.
- A **definition boundary** must explicitly state inclusions and exclusions.
- **Version changes** must be documented; silent changes are prohibited.
- **Deprecation** freezes meaning; deprecated terms remain referenceable.
- **Replacement mappings** must point from deprecated to active terms, never inversely.

---

## Explicit exclusions

The following are not permitted mappings:

- Meaning inferred from usage frequency or popularity
- Authority derived from adoption or community size
- Unversioned or implicit definition changes
- Deletion of terms without deprecation record

---

## Consistency rule

Any introduction of a new:
- semantic object, or
- governance element

requires synchronized updates to:
- this file,
- `SCOPE.md`, and
- `CHANGELOG.md`.

---

## Disclaimer

This document defines governance mappings only.  
It does not interpret meaning, enforce usage, or provide legal guarantees.
