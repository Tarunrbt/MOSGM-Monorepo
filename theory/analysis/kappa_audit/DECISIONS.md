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

---

## Decision 002

- **Decision ID:** DEC-002
- **Status:** Accepted
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
  connection to canonical assumptions is indirect. This methodology
  was subsequently applied in DEC-003 to reach a representation
  selection.

- **Alternatives Considered:**
  - Equal weighting of all four criteria — rejected, as it would give
    the GR Limiting Case criterion undue influence despite PA-06's
    explicit instruction not to resolve that question yet.
  - Elimination-based approach (excluding any candidate weak on any
    single criterion) — not adopted as the primary method, but
    incorporated as a supplementary tie-break check in DEC-003.

- **Date:** 2026-08-01

---

## Decision 003

- **Decision ID:** DEC-003
- **Status:** Accepted
- **Reason:** Per DEC-002, Observational Testability was applied as the
  primary weighting criterion. Three candidates (Scalar field, Vector
  field, Potential gradient) were tied at "Potentially Compatible" on
  this primary criterion; Tensor field was the only candidate rated
  "Undetermined" on it and was therefore not preferred under this
  weighting.

  A two-step tie-break was applied to the three tied candidates:
  - Step 1 (unjustified constraints): Potential gradient imposes an
    additional curl-free (conservative field) constraint that has not
    been derived or explicitly justified at this stage, consistent
    with the Excluded Assumptions principle against assuming
    structures "not derived or explicitly justified." Potential
    gradient was therefore set aside at this step. Scalar field and
    Vector field impose no such additional constraint and proceeded
    to Step 2.
  - Step 2 (raw secondary criteria strength): Between Scalar field and
    Vector field, Vector field rated "Strong" on both Supports
    Directionality and Supports Non-local Formulation, versus
    "Limited" and "Moderate" respectively for Scalar field.

  Vector field is therefore the selected candidate representation
  under the methodology established in DEC-002 and this decision's
  tie-break rules.

- **Impact:** The effective spacetime-gradient field referenced in
  PA-01 and DERIVATION_LOG.md Step 0 shall be represented as a vector
  field, G(r), for the purpose of continuing the κ derivation. This
  selection remains subject to revision if subsequent derivation
  steps (Step 2 onward) reveal internal mathematical inconsistency or
  conflict with any canonical assumption (PA-01 through PA-06, MA-01,
  MA-02). This decision does NOT resolve PA-06; the GR Limiting Case
  criterion was explicitly excluded from this selection per DEC-002.

- **Alternatives Considered:**
  - Tensor field — set aside due to "Undetermined" status on the
    primary weighting criterion (Observational Testability),
    notwithstanding its "Potentially Compatible" status on the
    non-discriminating GR Limiting Case criterion.
  - Potential gradient — set aside at the tie-break stage due to its
    unjustified additional curl-free constraint.
  - Scalar field — set aside at the tie-break stage due to weaker
    performance on secondary criteria relative to Vector field.

- **Date:** 2026-08-01

### Next Objective

Update DERIVATION_LOG.md Step 0's Decision Gate to reflect that a
representation has now been selected (Vector field, G(r)), and proceed
to Step 1 of the derivation: formally defining κ in terms of G(r), LΣ,
and β.

<!-- Additional decisions appended in sequence -->
