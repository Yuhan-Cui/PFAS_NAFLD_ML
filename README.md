# PFAS_NAFLD_ML

This repository provides the analysis notebooks for the study on
PFAS-induced non-alcoholic fatty liver disease (NAFLD) risk
prioritization using an integrated adverse outcome pathway (AOP)
framework and machine learning / deep learning models.

The workflow combines cross-barrier exposure modeling, quantitative
AOP construction, unsupervised risk tiering, and model-based validation
and extrapolation to identify high-risk PFASs associated with NAFLD.

---

## Repository contents

The analyses are primarily implemented as Jupyter notebooks located
in the root directory of this repository:

- `molecular_descriptor_processing.ipynb`  
  Molecular descriptor calculation, feature filtering, and dimensionality
  reduction used for model construction.

- `GMM.ipynb`  
  Gaussian mixture model (GMM)-based unsupervised risk tiering of PFASs.

- `LOO.ipynb`  
  Leave-one-out sensitivity analysis for evaluating the robustness of
  the AOP construction.

- `LightGBM_DL.ipynb`  
  Machine learning validation of PFAS risk tiers using gradient boosting
  models.

- `train_transformer_10fold_ablation.ipynb`  
  Deep learning model training with stratified 10-fold cross-validation
  and ablation analysis.

- `Deep_Learning_Extrapolation.ipynb`  
  Application of the trained deep learning model to extrapolate NAFLD
  risk levels for a large external PFAS dataset.

- `SHAP.ipynb`  
  Model interpretability analysis based on SHAP values.

---

## Notes on reproducibility

All analyses were conducted using Jupyter notebooks, which are provided
for transparency and reproducibility.

Due to file size limitations and software licensing constraints, raw
molecular dynamics trajectories and docking project files are not
included. The derived interaction energies, processed descriptors, and
intermediate results used in all analyses are sufficient to reproduce
the reported findings.

---

## Environment

The analyses were performed in a Python environment. Required packages
and dependencies are documented in the accompanying environment or
requirements configuration file.
