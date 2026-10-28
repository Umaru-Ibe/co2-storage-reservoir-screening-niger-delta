# Machine Learning-Based Screening and Ranking of Potential CO₂ Storage Reservoirs in the Niger Delta

## Overview

This project develops an integrated workflow for identifying, screening, and ranking potential geological CO₂ storage reservoirs using well-log-derived petrophysical properties and machine learning techniques.

The study focuses on depleted and mature reservoirs within the Agbada Formation of the Niger Delta Basin, Nigeria, and is designed as a transferable framework for Carbon Capture, Utilization and Storage (CCUS) projects in other sedimentary basins, including the CaMI Field Research Station (Canada), Aquistore (Saskatchewan), and the Jeanne d'Arc Basin (Atlantic Canada).

This repository represents the preliminary research framework for a proposed MSc study in Geological Carbon Storage, Reservoir Characterization, and Machine Learning Applications in Geoscience.

---

## Research Motivation

Geological Carbon Storage (GCS) is a critical component of global decarbonization strategies and climate-change mitigation efforts. Depleted hydrocarbon reservoirs offer attractive storage targets due to their proven containment capacity, established geological understanding, and existing subsurface data.

Traditional reservoir screening methods are often deterministic and time-intensive. This project investigates whether machine learning can improve the speed, consistency, and reliability of storage-site selection while maintaining geological rigor.

### Research Question

Can well-log-derived petrophysical attributes be combined with explainable machine learning algorithms to identify and rank geological formations suitable for long-term CO₂ sequestration?

---

## Study Area

**Basin:** Niger Delta Basin, Nigeria

**Formation:** Agbada Formation

**Data Source:**
- 12 exploration and appraisal wells
- Depth interval: 1,500–3,500 m
- Wireline logs:
  - Gamma Ray (GR)
  - Spontaneous Potential (SP)
  - Resistivity
  - Neutron Porosity (NPHI)
  - Bulk Density (RHOB)
  - Sonic Logs

---

## Objectives

The project aims to:

- Characterize potential CO₂ storage reservoirs using petrophysical properties.
- Develop screening criteria for geological carbon storage.
- Apply machine learning models for reservoir classification and ranking.
- Identify key geological controls affecting storage suitability.
- Establish a transferable workflow for future CCUS site-selection studies.

---

## Methodology

### 1. Petrophysical Analysis

Reservoir properties are calculated from well-log data, including:

- Volume of Shale (Vsh)
  - Larionov Method
- Effective Porosity (PHIe)
  - Density-Neutron Crossplot Method
- Permeability (K)
  - Timur-Coates Relationship
- Net-to-Gross Ratio (NTG)

### 2. Geological Screening Criteria

Reservoir intervals are screened according to commonly accepted CCS requirements:

| Parameter | Screening Threshold |
|------------|--------------------|
| Depth | 1,500–3,500 m |
| Effective Porosity | >15% |
| Permeability | >100 mD |
| Seal Thickness | >10 m |
| Residual Oil Saturation | <0.40 |

### 3. Machine Learning Analysis

Algorithms evaluated include:

- Random Forest
- XGBoost
- K-Means Clustering

Applications:

- Reservoir suitability classification
- CCS fairway identification
- Reservoir ranking
- Pattern recognition

### 4. Explainable AI

Model interpretability is assessed using:

- SHAP (SHapley Additive Explanations)
- Feature Importance Analysis
- Blind-Well Validation

---

## Workflow

```text
Well Logs
    │
    ▼
Petrophysical Evaluation
    │
    ▼
Reservoir Screening
    │
    ▼
Feature Engineering
    │
    ▼
Machine Learning Classification
    │
    ▼
SHAP Explainability
    │
    ▼
Reservoir Ranking
    │
    ▼
CCUS Decision Support
```

---

## Key Results

### Reservoir Quality

- Reservoirs evaluated: 10
- Wells analyzed: 12
- Porosity range: 18–31%
- Mean porosity: 26%
- Permeability range: 458–3,251 mD
- Net reservoir thickness: 6–73 m
- Caprock thickness: 3.3–102 m
- Pressure regime: 9.5–10.4 ppg

---

### Reservoir Classification

| Storage Class | Reservoir Count |
|--------------|----------------|
| Excellent | 3 |
| Intermediate | 4 |
| Poor | 3 |

Two reservoir candidates were excluded due to depth constraints and seal integrity concerns.

---

### Machine Learning Performance

| Model | Accuracy | F1 Score |
|---------|----------|----------|
| XGBoost | 0.89 | 0.87 |

#### Most Influential Parameters

1. Effective Porosity (PHIe)
2. Reservoir Depth
3. Volume of Shale (Vsh)
4. Permeability

---

### Storage Capacity Estimates

Preliminary storage-capacity calculations indicate potential CO₂ storage volumes ranging from:

**2.58 to 22.4 million tonnes**

using a conservative storage efficiency factor of 10%.

---

## Visualization

### SHAP Feature Importance

images/shap_summary.png

### CCS Fairway Mapping

images/gis_fairway.png

### Project Overview

images/overview.png

---

## Scientific Contributions

This work contributes to:

- Geological Carbon Storage (GCS)
- Carbon Capture, Utilization and Storage (CCUS)
- Reservoir Characterization
- Explainable Artificial Intelligence (XAI)
- Subsurface Energy Systems
- Machine Learning Applications in Geoscience

The proposed workflow provides a reproducible framework for early-stage screening of CO₂ storage opportunities in emerging CCS regions.

---

## Future Work

Planned developments include:

- Integration of 3D seismic attributes
- Dynamic reservoir simulation
- Uncertainty quantification
- Comparative analysis with the Dahomey Basin
- Validation against Canadian CCS analogues (Aquistore and CaMI-FRS)
- Development of a basin-scale storage suitability index

---

## Reproducibility

### Installation

```bash
pip install -r requirements.txt
```

### Petrophysical Workflow

```bash
jupyter notebook notebooks/01_petrophysics.ipynb
```

### Machine Learning Workflow

```bash
jupyter notebook notebooks/02_ml_screening.ipynb
```

---

## Author

**Umaru Ibe**

Geophysicist | Reservoir Characterization | Formation Evaluation | 3D Seismic Interpretation | Geological Carbon Storage Research

GitHub: https://github.com/Umaru-Ibe

---

## Citation

If you use this workflow, dataset structure, or methodology, please cite:

> Ibe, U. (2026). Machine Learning-Based Screening and Ranking of Potential CO₂ Storage Reservoirs in the Niger Delta Basin. Research Repository, GitHub.
