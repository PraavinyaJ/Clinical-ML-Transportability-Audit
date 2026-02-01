# Clinical-ML-Transportability-Audit

## Research Objective

To evaluate the operational robustness of a clinical risk model when subjected to simulated system-level variations. This audit focuses on the gap between "in-silico" performance and "at-the-bedside" reality.

## Synthetic "Hospital Setting" Framework

I am simulating three distinct deployment scenarios to test model stability:

The Low-Resource Setting: High feature missingness (simulating charting delays or lack of advanced lab equipment).

The Demographic Shift: Altered age/sex distribution (simulating a transition from a general hospital to a specialized geriatric or pediatric ward).

The Measurement Noise: Stochastic perturbations in continuous variables (simulating variability in different lab manufacturers or sensor brands).

## Evaluation Framework

Unlike standard ML projects, this audit prioritizes reliability over accuracy:

Discrimination: AUROC (Does the model still rank patients correctly?)

Calibration: Brier Score & Calibration Curves (Does a "20% risk" actually mean 2 out of 10 patients?)
