# Machine Learning-Based Screening and Ranking of Geological CO₂ Storage Reservoirs in the Niger Delta and Dahomey Basins

<div align="center">

[![Research Portfolio](https://img.shields.io/badge/📄%20Research%20Portfolio-View-blue?style=for-the-badge)](docs/portfolio.pdf)
![Python](https://img.shields.io/badge/Python-3.11-blue?style=for-the-badge&logo=python)
![Focus](https://img.shields.io/badge/Focus-CCUS-darkgreen?style=for-the-badge)
![Machine Learning](https://img.shields.io/badge/ML-XGBoost-orange?style=for-the-badge)
![Explainable AI](https://img.shields.io/badge/XAI-SHAP-red?style=for-the-badge)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

<br>

![Storage Capacity](https://img.shields.io/badge/Storage%20Capacity-2.58--22.4%20MMt%20CO₂-success?style=flat-square)
![Wells Analyzed](https://img.shields.io/badge/Wells%20Analyzed-12-informational?style=flat-square)
![Accuracy](https://img.shields.io/badge/Accuracy-89%25-success?style=flat-square)

</div>

---

## Overview

This repository presents an integrated machine-learning workflow for screening, ranking, and evaluating potential geological CO₂ storage reservoirs using well-log-derived petrophysical properties and explainable artificial intelligence.

The framework combines:

- Reservoir Characterization
- Storage Capacity Estimation
- Explainable AI (SHAP)
- GIS-Based Fairway Mapping
- Machine Learning Classification

to support data-driven geological carbon storage assessment.

The workflow was developed using datasets from the **Agbada Formation of the Niger Delta Basin** and is designed to be transferable to the **Dahomey Basin** and other emerging Carbon Capture, Utilization and Storage (CCUS) regions.

---

## Research Portfolio

📄 **Research Portfolio**

The complete MSc research portfolio is available here:

```text
docs/portfolio.pdf
```

The portfolio includes:

- Research Motivation
- Research Gap
- Workflow Architecture
- Reservoir Characterization
- Machine Learning Classification
- SHAP Explainability
- Storage Fairway Mapping
- Canadian CCS Research Alignment
- Proposed MSc Research Objectives

---

## Research Question

> **Can well-log-derived petrophysical properties and explainable machine-learning techniques be integrated to reliably screen and rank depleted hydrocarbon reservoirs for geological CO₂ storage?**

---

## Study Area

### Basin

- Niger Delta Basin
- Dahomey Basin *(future expansion)*

### Formation

- Agbada Formation

### Data Sources

The workflow uses well-log-derived petrophysical attributes including:

- Gamma Ray (GR)
- Spontaneous Potential (SP)
- Resistivity
- Bulk Density (RHOB)
- Neutron Porosity (NPHI)
- Sonic Logs

### Depth Interval

```text
1,500–3,500 m
```

---

## Workflow Architecture

```text
Well Logs
    ↓
Petrophysical Analysis
    ↓
Storage Screening Criteria
    ↓
Feature Engineering
    ↓
Random Forest / XGBoost
    ↓
SHAP Explainability
    ↓
Reservoir Ranking
    ↓
Storage Capacity Estimation
    ↓
GIS Fairway Mapping
    ↓
CCUS Decision Support
```

---

## Methodology

### Reservoir Characterization

Derived parameters:

- Effective Porosity (PHIE)
- Volume of Shale (Vsh)
- Permeability (K)
- Net-to-Gross Ratio (NTG)
- Seal Thickness

### Geological Screening

Reservoir candidates are evaluated using:

- Reservoir Depth
- Effective Porosity
- Permeability
- Caprock Thickness
- Structural Integrity
- Storage-Containment Potential

### Machine Learning

Algorithms:

- Random Forest
- XGBoost

### Explainable AI

Interpretability tools:

- SHAP
- Feature Importance Ranking
- Blind-Well Validation

---

## Key Results

### Reservoir Quality

| Parameter | Range |
|------------|--------|
| Effective Porosity | 18–31% |
| Permeability | 458–3251 mD |
| Reservoir Thickness | 6–73 m |
| Caprock Thickness | 3.3–102 m |
| Storage Capacity | 2.58–22.4 MM tonnes CO₂ |

### Reservoir Classification

| Classification | Count |
|---------------|--------|
| Excellent | 3 |
| Intermediate | 4 |
| Lower Priority | 3 |

### Model Performance

| Metric | Value |
|----------|--------|
| Accuracy | 0.89 |
| F1 Score | 0.87 |

---

## Results and Figures

### Figure 0 — Reservoir Characterisation

```text
images/fig0_reservoir_characterisation.png
```

### Figure 1 — Workflow Architecture

```text
images/fig1_workflow_architecture_corrected.png
```

### Figure 1B — Reservoir Quality Assessment

```text
images/fig1b_reservoir_quality_assessment.png
```

### Figure 2 — SHAP Analysis

```text
images/fig2_shap_analysis.png
```

### Figure 3 — Storage Fairway Map

```text
images/fig3_fairway_map.png
```

### Figure 4 — Integrated Storage Assessment

```text
images/fig4_integrated_assessment.png
```

---

## Repository Structure

```text
CO2-Storage-Niger-Delta-Dahomey/

├── README.md
├── images/
│   ├── fig0_reservoir_characterisation.png
│   ├── fig1_workflow_architecture_corrected.png
│   ├── fig1b_reservoir_quality_assessment.png
│   ├── fig2_shap_analysis.png
│   ├── fig3_fairway_map.png
│   └── fig4_integrated_assessment.png
│
├── notebooks/
│   ├── 01_petrophysics.ipynb
│   ├── 02_xgboost_classification.ipynb
│   └── 03_shap_explainability.ipynb
│
├── src/
│   └── storage_capacity.py
│
├── data/
│   └── sample/
│       └── example_porosity_perm.csv
│
├── docs/
│   └── portfolio.pdf
│
├── requirements.txt
├── LICENSE
└── CITATION.cff
```

---

## Reproducibility

### Install Dependencies

```bash
pip install -r requirements.txt
```

### Run Petrophysical Workflow

```bash
jupyter notebook notebooks/01_petrophysics.ipynb
```

### Run Machine Learning Workflow

```bash
jupyter notebook notebooks/02_xgboost_classification.ipynb
```

### Run SHAP Analysis

```bash
jupyter notebook notebooks/03_shap_explainability.ipynb
```

---

## Future Work

- Dahomey Basin Comparative Assessment
- Dynamic CO₂ Injection Simulation
- Reservoir Uncertainty Quantification
- Geochemical Modelling
- Seismic Attribute Integration
- Storage Suitability Index (SSI)
- AI-Assisted Injectivity Forecasting

---

## Research Significance

This project contributes to:

- Geological Carbon Storage (GCS)
- Carbon Capture, Utilization and Storage (CCUS)
- Reservoir Characterization
- Explainable Artificial Intelligence (XAI)
- Machine Learning Applications in Geoscience
- Storage Capacity Assessment
- Subsurface Decision-Support Systems

---

## Citation

If you use this repository, please cite:

```text
Ibe, U. (2026).

Machine Learning-Based Screening and Ranking of Geological
CO₂ Storage Reservoirs in the Niger Delta and Dahomey Basins.

GitHub Repository.
```

---

## Author

**Umaru Ibe**

Geophysicist | Reservoir Characterization | Formation Evaluation | 3D Seismic Interpretation

### Research Interests

- Geological Carbon Storage
- Carbon Capture, Utilization and Storage (CCUS)
- Reservoir Characterization
- Explainable Artificial Intelligence
- Machine Learning for Subsurface Systems
- Subsurface Energy Systems

### Contact

📧 umaruibe@gmail.com carbon storage assessment and subsurface decision-support systems.*
