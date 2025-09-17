# MCMC Fitting in Astrophysics

This repository contains reproducible code and notebooks for MCMC-based parameter inference in astrophysics.  
It focuses on two related topics:

- **MCMC scaling method** for estimating black hole masses from X-ray binary spectral parameters (two files / notebook).
- **MCMC for cosmological parameter estimation** (one file / notebook).
- **Data selection & preprocessing** used to prepare the samples for scaling-curve fitting (one file / notebook).

---

---

## Short descriptions

### 1. `Scaling GRO D05-bmc-GP.ipynb` & `Scaling GRO D05-bmc-GP.ipynb`
- Demonstrate the **scaling method** used on X-ray binary data to infer the black hole mass.
- Implement an MCMC sampler (e.g., `emcee`) to fit the empirical scaling curve and report posterior distributions.
- Include: data ingestion, masking of invalid values (`np.isfinite`), parameter priors, likelihood, MCMC setup, corner plots, trace plots, and saving of flattened samples.

### 2. `Cosmological Parameter.ipynb`
- Uses MCMC to estimate cosmological parameters (example: Ω_m, H0, etc.).
- Shows a full Bayesian workflow: model, likelihood for observables, MCMC sampling, diagnostics, and posterior visualization.

### 3. `data_selection.py` / `data_selection.ipynb`
- Documents the data cleaning and selection pipeline used for the scaling-curve fits.
- Includes detailed filters: NaN/inf removal, error handling, selection cuts, and final sample export.
- This file ensures reproducibility and that only physically meaningful points enter the MCMC fits.

---
