# The Lovelace Threshold Dataset

**Author:** Bhavyatta Bhardwaj  
**Version:** 1.0  
**Date:** April 2026  
**DOI:** 10.5281/zenodo.19741055

## What this repository contains

This repository supports the working paper The Lovelace Threshold: A Governance Measurement Instrument. It contains the empirical dataset underpinning the paper's applied demonstration, along with reproducible analysis in Python.

A dataset of 240 material drivers of AI governance outcomes, compiled through independent research into AI development lifecycles, existing regulatory frameworks, and practitioner knowledge.

| Column | Description |
|---|---|
| ID | Unique variable identifier |
| Variable | Name of the governance variable |
| Short definition | Plain language description |
| Stage | Lifecycle stage (Data, Training, Model Design, etc.) |
| Governed | Governance status: No / Partial |
| Regulatory gap | Size of gap: Small / Moderate / Large |
| Rate of risk | Urgency: Low / Medium / High / Critical/Urgent |
| Suggested mitigation | Recommended action |

### Governance coding criteria

Each variable was coded against the following reference frameworks:
- EU AI Act (2024)
- GDPR (2018)
- NIST AI Risk Management Framework (2023)
- ISO/IEC 42001 (2023)

**No:** no existing provision in the reference frameworks directly addresses this variable  
**Partial:** a provision exists but applies only to high-risk systems, covers only part of the variable, or lacks enforcement mechanisms  

No variable in the dataset is fully governed across all reference frameworks.

### Key findings

- 240 material drivers of AI governance outcomes identified
- 149 (62%) are entirely ungoverned across all reference frameworks
- 91 (38%) are partially governed
- 0 (0%) are fully governed
- 38 ungoverned variables are rated Critical/Urgent
- 67 ungoverned variables (Data, Training, Model Design, Infrastructure)

`Lovelace Gap (EU AI Act) = 149 / 240 = 0.62`

## Analysis

Reproducible analysis: `analysis/lovelace_gap_analysis.ipynb` — Python (Pandas)

## Citation

If you use this dataset, please cite:

> Bhardwaj, B. (2026). *The Lovelace Threshold Dataset* (v1.0). GitHub. 10.5281/zenodo.19741055 

## License

CC BY 4.0 — you may use and build on this dataset with attribution.
