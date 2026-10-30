Machine Learning-Based Screening and Ranking of Geological CO₂ Storage Reservoirs in the Niger Delta and Dahomey Basins
Overview
This repository presents an integrated machine-learning workflow for screening, ranking, and evaluating potential geological CO₂ storage reservoirs using well-log-derived petrophysical properties and explainable artificial intelligence.

The project focuses on depleted and mature hydrocarbon reservoirs within the Niger Delta Basin and provides a framework that can be extended to the Dahomey Basin and other emerging Carbon Capture, Utilization and Storage (CCUS) regions.

The workflow combines reservoir characterization, storage suitability assessment, storage-capacity estimation, GIS-based fairway mapping, and explainable machine learning to support early-stage geological storage decision-making.

Research Motivation
Geological Carbon Storage (GCS) is expected to play a critical role in achieving global net-zero emissions targets. While substantial storage characterization efforts have been undertaken in North America and Europe, comparatively limited machine-learning-driven storage assessments have been conducted within African sedimentary basins.

This project investigates whether well-log-derived petrophysical attributes can be integrated with explainable machine-learning workflows to rapidly identify and rank reservoirs suitable for long-term CO₂ sequestration.

Research Question
Can well-log-derived petrophysical properties and explainable machine-learning techniques be integrated to reliably screen and rank depleted hydrocarbon reservoirs for geological CO₂ storage?

Study Area
Basin
Niger Delta Basin
Dahomey Basin (future expansion)
Formation
Agbada Formation
Dataset
Well-log datasets from twelve wells containing:

Gamma Ray (GR)
Spontaneous Potential (SP)
Resistivity
Density (RHOB)
Neutron Porosity (NPHI)
Sonic Logs
Depth interval:

1,500–3,500 m
Workflow Architecture
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
Methodology
Petrophysical Analysis
Derived parameters include:

Effective Porosity (PHIE)
Volume of Shale (Vsh)
Permeability (K)
Net-to-Gross Ratio (NTG)
Seal Thickness
Screening Criteria
Reservoir candidates are evaluated using:

Reservoir depth
Effective porosity
Permeability
Caprock thickness
Structural integrity
Storage-containment potential
Machine Learning
Models include:

Random Forest
XGBoost
K-Means Clustering
Explainable AI
Interpretability is assessed using:

SHAP (SHapley Additive Explanations)
Feature Importance Analysis
Blind-Well Validation
Key Results
Reservoir Quality
Parameter	Range
Porosity	18–31%
Permeability	458–3251 mD
Reservoir Thickness	6–73 m
Caprock Thickness	3.3–102 m
Storage Capacity	2.58–22.4 MM tonnes CO₂
Storage Classification
Excellent: 3 reservoirs
Intermediate: 4 reservoirs
Poor: 3 reservoirs
Machine Learning Performance
Metric	Value
Accuracy	0.89
F1 Score	0.87
Figures
Reservoir Characterization
