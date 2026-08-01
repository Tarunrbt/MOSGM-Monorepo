# REPRESENTATION_EVALUATION.md — MOSGM κ Audit, Step 1

## Purpose
This document evaluates candidate mathematical representations of the
effective spacetime-gradient field against the Entry Criteria established in
DERIVATION_LOG.md (Step 0 Decision Gate). No candidate is selected until all
criteria are populated and reviewed. Evaluation proceeds column-by-column
(one criterion at a time across all candidates) to minimize sequential bias.

## Evaluation Criteria (from Step 0 Entry Criterion)
- Consistency with PA-01 through PA-06
- Consistency with MA-01 and MA-02
- Internal mathematical consistency
- Observational testability

## Note on GR Compatibility
Per PA-06, the relationship between MOSGM and GR is intentionally unresolved.
The relevant column below evaluates only whether a representation is
*structurally capable* of admitting GR as a limiting case — it does not assert
that MOSGM is or is not a General Relativity extension.

## Methodology Note: "Can Admit GR as a Limiting Case?" Criterion

Per PA-06, the relationship between MOSGM and General Relativity is
intentionally unresolved during this audit. This criterion therefore does
NOT ask whether MOSGM reduces to GR — that question remains open.

Instead, it asks only whether a mathematical representation structurally
excludes or remains open to admitting a GR-like limiting case. This is an
exclusionary/permissive test, not a confirmatory one.

Sub-questions considered:
- Does the representation structurally exclude a GR-like limiting case?
- Does it remain structurally open to admitting one?
- Does its mathematical structure permit such a possibility without
  resolving PA-06?

Assessments shall therefore use only the following provisional categories:
- Potentially Compatible
- Potentially Incompatible
- Undetermined

Each assessment must include a brief structural justification.

---

## Table

| Candidate | Supports Directionality | Justification | Supports Non-local Formulation | Can Admit GR as a Limiting Case? | Observational Testability | Status |
|---|---|---|---|---|---|---|
| Scalar field | Limited | Directionality is not intrinsic to a scalar field but may arise through its spatial derivative. | Moderate | Undetermined | Pending | Under Review |
| Vector field | Strong | Directionality is intrinsic to a vector field. | Strong | Undetermined | Pending | Under Review |
| Tensor field | Strong (General) | Supports anisotropic and direction-dependent behavior beyond vectors. | Strong (Added Complexity) | Potentially Compatible | Pending | Under Review |
| Potential gradient | Strong (Constrained) | Directionality is present through the gradient, but restricted to conservative (curl-free) fields. | Strong (Constrained) | Undetermined | Pending | Under Review |

---

## Next Objective
Evaluate the final criterion — "Observational Testability" — across all
four candidates. Once populated, review the completed table as a whole
before proceeding to DECISIONS.md.

## Revision History
- 2026-07-31: Initial evaluation table created; first column
  ("Supports Directionality") populated for all four candidates.
- 2026-07-31: Second column ("Supports Non-local Formulation") populated for
  all four candidates; language kept non-committal regarding the role of LΣ,
  which remains under audit.
- 2026-08-01: Third column ("Can Admit GR as a Limiting Case?") populated for
  all four candidates using canonical categories (Potentially Compatible /
  Potentially Incompatible / Undetermined), per the Methodology Note. PA-06
  remains unresolved.
- 2026-08-01: Corrected document structure — restored Methodology Note
  (with canonical categories) to appear before the Table; removed a
  duplicated stray line; updated Next Objective to reflect current progress.
