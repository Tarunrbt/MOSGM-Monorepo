# Decision Log — κ Audit

## Decision Template
- **Decision ID:**
- **Status:** [Proposed / Accepted / Rejected / Superseded]
- **Reason:**
- **Impact:**
- **Alternatives Considered:**
- **Date:**

---

## Decision 001

- **Decision ID:** DEC-001
- **Status:** Accepted
- **Reason:** All four evaluation criteria (Supports Directionality,
  Supports Non-local Formulation, Can Admit GR as a Limiting Case,
  Observational Testability) have been populated in
  REPRESENTATION_EVALUATION.md for all four candidate representations
  (Scalar field, Vector field, Tensor field, Potential gradient),
  using the canonical provisional categories established in the
  Methodology Notes. This completes the evaluation phase of Step 1.

- **Impact:** No representation has been selected at this stage.
  The completed evaluation documents the strengths and trade-offs of
  each candidate without determining a preferred representation.
  Representation selection remains a separate decision.

- **Recorded Observations:**
  - No candidate is uniformly strongest across all evaluated criteria.
  - Tensor field is the only candidate currently assessed as
    "Potentially Compatible" under the GR Limiting Case criterion.
  - Tensor field remains "Undetermined" for Observational
    Testability within the current evaluation.
  - Vector field and Potential gradient show similar evaluation
    profiles, with the Potential gradient additionally constrained
    by its conservative (curl-free) structure.

- **Alternatives Considered:** N/A. This decision records completion
  of the evaluation phase only; it does not select a representation.

- **Date:** 2026-08-01

### Next Objective

Conduct a dedicated representation-selection review using the completed
evaluation table. Any representation selected shall be documented as a
separate decision (DEC-002), including the rationale for how trade-offs
between evaluation criteria were weighed.

---

## Decision 002

- **Decision ID:** DEC-002
- **Status:** Proposed
- **Reason:** Following DEC-001 (evaluation phase completion), a method
  was needed to weigh the four evaluation criteria in
  REPRESENTATION_EVALUATION.md against each other for eventual
  representation selection, since no candidate is uniformly strongest
  across all criteria. Each criterion was cross-referenced against
  ASSUMPTIONS.md (PA-01 through PA-06, MA-01, MA-02) to determine
  which criteria are directly mandated by canonical assumptions versus
  which are only weakly or indirectly suggested.

  Findings from this cross-reference:
  - Observational Testability is explicitly and doubly mandated by
    PA-03 ("observable signatures... testable against astronomical
    observations") and PA-04 ("committed to producing falsifiable,
    quantitatively testable predictions").
  - Can Admit GR as a Limiting Case is explicitly addressed by PA-06,
    which states the MOSGM-GR relationship is intentionally left
    unresolved until after mathematical derivation and observational
    validation. Using this criterion as a discriminating factor at
    this stage would risk prematurely resolving PA-06, which is
    explicitly against the Excluded Assumptions ("That MOSGM replaces
    General Relativity").
  - Supports Directionality and Supports Non-local Formulation are
    only indirectly suggested by the wording of PA-01 (the terms
    "gradient" and "LΣ"), which itself states its mathematical
    representation is deferred. Neither criterion is directly
    mandated by any canonical assumption.

- **Impact:** For the purpose of representation selection,
  Observational Testability shall be treated as the primary weighting
  factor, as it is the only criterion with a direct, dual mandate from
  PA-03 and PA-04. Can Admit GR as a Limiting Case shall NOT be used
  as a discriminating factor in selection, consistent with PA-06.
  Supports Directionality and Supports Non-local Formulation shall be
  treated as secondary, context-informing factors only, since their
  connection to canonical assumptions is indirect.

- **Alternatives Considered:**
  - Equal weighting of all four criteria — rejected, as it would give
    the GR Limiting Case criterion undue influence despite PA-06's
    explicit instruction not to resolve that question yet.
  - Elimination-based approach (excluding any candidate weak on any
    single criterion) — not adopted at this stage, but not ruled out
    as a supplementary check during the selection review.

- **Date:** 2026-08-01

### Next Objective

Using Observational Testability as the primary lens (per this decision),
review the completed REPRESENTATION_EVALUATION.md table and proceed to a
representation-selection discussion. Any selection made shall be recorded
as DEC-003, referencing this weighting rationale.

<!-- Additional decisions appended in sequence -->
