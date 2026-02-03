# Clinical ML Transportability & Data Quality Audit (Planned)

**Status:** Not started (proposal / design complete)  
**Start date:** [Feb 2026]  
**Goal:** Stress-test a clinical ML model under dataset shift and data-quality issues, and report reliability (calibration) alongside discrimination.

## What’s done
- [x] Project scope + evaluation design drafted
- [x] Metrics + reporting plan defined (AUROC, AUPRC, Brier score, calibration curve)
- [x] Shift/perturbation taxonomy drafted (missingness, measurement noise, demographic shift)

## What’s planned
- [ ] Baseline pipeline (data split, preprocessing, model training)
- [ ] Reliability evaluation + calibration (train-only preprocessing; no leakage)
- [ ] Synthetic perturbations (controlled missingness, noise, shift scenarios)
- [ ] Shift detection / drift monitoring (optional)
- [ ] Reproducible report (notebook + figures)

## Method (high level)
- **Metrics:** AUROC, AUPRC, Brier score, calibration curve / ECE  
- **Shift tests:** 
  - Missingness (MCAR/MAR-style simulations)
  - Measurement noise / rounding / unit shifts
  - Demographic shift (reweighting / subgroup resampling)
- **Reporting:** performance + calibration drift across scenarios

## Notes
This repository currently contains the **evaluation plan only**. Code and experiments will be added once implementation begins.


