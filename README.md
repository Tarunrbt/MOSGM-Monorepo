# Matter-Originated Spacetime Gradient Model (MOSGM)

[![Repository Status](https://img.shields.io/badge/Status-Active_Research-blue.svg)](https://github.com/Tarunrbt/MOSGM-Theory)

**Author:** Tarun Kumar Saxena (Independent Researcher)
**Canonical Repository:** `Tarunrbt/MOSGM-Theory`

<!-- DOI badge pending Zenodo record verification — do not hardcode until confirmed -->

---

## Overview

MOSGM is a phenomenological framework proposing that spacetime properties arise
from large-scale matter distributions rather than existing as an independent
background. It explores environment-dependent corrections to galactic
gravitational dynamics as an alternative to particle dark matter, without
claiming a complete relativistic theory of gravity.

The framework is intentionally conservative in scope and designed to be
explicitly testable and falsifiable.

---
## Repository Status

- Active Research
- Current Phase: κ Derivation Audit
- Repository Status: Under Active Scientific Review

## Core Structure

MOSGM has two distinct layers, and it is important not to conflate them:

**1. MOSGM-I — Rotation curve formula**
g_obs = g_bar [1 + κ(μ(x) − 1)]
```text
g_obs = g_bar [1 + κ(μ(x) − 1)]
```
This layer reproduces SPARC-type rotation curves. **It is currently
numerically close to MOND on rotation curves alone** and does not, by itself,
constitute evidence for a distinct mechanism.

**2. Environmental correction layer — where MOSGM's novelty lives**
g_eff(r) = g_N(r) [1 + α F(∇Σ_env)]

This layer predicts a **directional (vector-dependent) lopsidedness** tied to
the orientation of the local environmental density gradient — structurally
different from MOND's scalar External Field Effect. This is the only
component of MOSGM that offers a result distinguishable from MOND, and it is
tested via a sign-test against MaNGA data (not yet executed — see below).

---

## Current Status (verified, as of this update)

| Item | Status |
|---|---|
| κ derivation (action → weak-field limit) | **Unresolved.** Published value κ = 1/(e−1) ≈ 0.5820 breaks the deep-field recovery condition (g_obs → √(g_bar·a₀) requires κ = 1). This is a structural inconsistency, under active audit. |
| Five-galaxy pilot re-run (κ = 1) | Not yet executed. Blocked on κ audit. |
| Full SPARC run (175 galaxies, M/L = 0.5 correction) | Not yet executed. Blocked on pilot re-run. |
| α lock via SPARC | Not yet performed. |
| MaNGA directional sign test | Not yet executed. Pre-registration timestamp and ∇Σ₀ normalization (Tempel et al. 2014) are frozen ahead of data access, per pre-registration discipline. |
| Cluster-scale claims (5.1σ / 3.9σ) | **Removed from active evidence base.** These relied on MOND's a₀ in a way incompatible with MOSGM's own governing equations and are archived — see `archive/superseded/`. |

**No result in this repository should be cited as a validated MOSGM detection
beyond the SPARC rotation-curve fitting described above.** The environmental
layer is the framework's central claim and remains untested pending the
pipeline sequence below.

---

## Mandatory Analysis Sequence

κ audit → 5-galaxy pilot re-run (κ = 1) → full SPARC run (M/L = 0.5) →
α lock → MaNGA sign test → Results section writable

This order is enforced for scientific integrity: α must be anchored via SPARC
*before* MaNGA data is opened. Reversing this order would constitute
post-hoc analysis.

---

## Repository Structure

```text
MOSGM-Theory/
├── README.md
├── CHANGELOG.md
├── docs/
│   ├── MOSGM_theory.pdf              # v3.0 hard-locked theory specification
│   └── MOSGM_Yukawa_Calculation.pdf
├── analysis/
│   ├── kappa_audit/                  # Active: action -> weak-field derivation
│   ├── sparc_pilot/                  # 5-galaxy calibration (DDO 154, UGC 128,
│   │                                  #   NGC 3198, NGC 2403, NGC 6503)
│   ├── sparc_full/                   # Full 175-galaxy benchmark
│   └── manga_sign_test/              # Placeholder — locked pending α anchor
├── results/                          # Tracked plots, residuals, metrics
└── archive/
    └── superseded/
        └── cluster_5.1sigma_claim_ARCHIVED.md
```

---

## Datasets

- **SPARC** (Lelli et al. 2016) — 175-galaxy catalog; rotation curve fitting
- **MaNGA DR17** — for the environmental directional sign test (not yet accessed)
- **Tempel et al. 2014** SDSS filament catalog — ∇Σ₀ normalization (frozen)
- **Pan et al. 2012** — void catalog cross-match

---
## Scientific Principles

- Reproducibility before claims
- Evidence over narrative
- Pre-registered analysis sequence
- Transparent revision history
- Archived claims remain accessible but are not treated as current evidence
## Scientific Discipline

- No numerical result is reported without a traceable, reproducible local
  output file.
- No result appears in the manuscript without completed analysis, code,
  uncertainty estimates, and statistical validation.
- The productive path is rigor and independent replication — not narrative
  positioning.

---

## Citation

Please cite this repository and the associated Zenodo archival record.
Zenodo DOI badges will be added once the canonical version DOI and
concept (all-versions) DOI are confirmed against the live Zenodo dashboard.

(Do not cite the archived cluster-scale claim as representative of current
MOSGM results — see `archive/superseded/`.)
