# Analysis Pipeline Overview

This document serves as the canonical map, navigation hub, and governance outline for all observational and analytical pipelines in the repository.

---

## Analysis Modules

* **`kappa_audit/`**: Canonical κ derivation audit and verification workspace.
* **`sparc_pilot/`**: Initial validation pipeline on a subset of SPARC galaxy rotation curves.
* **`sparc_full/`**: Full-scale SPARC dataset analysis and statistical fitting.
* **`manga_sign_test/`**: Observational sign-test and field-gradient checks using MaNGA IFU kinematics.

---

## Pipeline Phases & Governance

### Phase 1 — κ Audit
* **Objective:** Validate the canonical κ derivation and mathematical consistency.
* **Entry Criteria:**
  * Repository cleanup complete
  * Canonical theory locked
  * Audit workspace initialized
* **Exit Criteria:**
  * Final derivation completed
  * Consistency checks passed
  * Reviewer sign-off recorded
* **Deliverables:**
  * `analysis/kappa_audit/DERIVATION_LOG.md`
  * `analysis/kappa_audit/DECISIONS.md`
  * `analysis/kappa_audit/CHECKLIST.md`

---

### Phase 2 — SPARC Pilot
* **Objective:** Test model pipeline on selected representative SPARC rotation curves.
* **Entry Criteria:**
  * Phase 1 (κ Audit) exit criteria fulfilled
  * Cleaned SPARC pilot dataset available
* **Exit Criteria:**
  * Residuals and parameter sensitivity verified on pilot sample
  * Execution scripts stabilized
* **Deliverables:**
  * Pilot fitting logs and diagnostic plots

---

### Phase 3 — Full SPARC
* **Objective:** Execute full sample analysis across the SPARC galaxy database.
* **Entry Criteria:**
  * Phase 2 (SPARC Pilot) successfully completed
  * Full dataset pipeline scripts locked
* **Exit Criteria:**
  * Global goodness-of-fit statistics compiled
  * Residual distributions and scatter metrics finalized
* **Deliverables:**
  * Complete SPARC analysis logs and output summary tables

---

### Phase 4 — α Lock
* **Objective:** Fix and lock the universal scaling parameter (α) bounds based on broad dataset fits.
* **Entry Criteria:**
  * Phase 3 (Full SPARC) completed
  * Global parameter constraints evaluated
* **Exit Criteria:**
  * Universal value/range for α locked with error bounds
  * Governance decision logged
* **Deliverables:**
  * Parameter lock decision document

---

### Phase 5 — MaNGA Sign Test
* **Objective:** Perform out-of-sample observational sign tests on MaNGA IFU kinematic field gradients.
* **Entry Criteria:**
  * Phase 4 (α Lock) completed
  * MaNGA kinematic selection cuts established
* **Exit Criteria:**
  * Statistical sign-test evaluation complete
  * Final observational validation status recorded
* **Deliverables:**
  * MaNGA sign-test results and audit log

---

### Final Phase — Publication & Synthesis
* **Objective:** Synthesize all validated results into a coherent, reviewable scientific record.
* **Entry Criteria:**
  * Phase 5 (MaNGA Sign Test) completed
  * All prior deliverables reviewed and signed off
* **Exit Criteria:**
  * Manuscript/report drafted and internally reviewed
  * All claims traceable to corresponding phase deliverables
* **Deliverables:**
  * Final synthesis document / manuscript

---

## Dependency Graph
