# Machine Learning-Based Screening and Ranking of Geological CO₂ Storage Reservoirs in the Niger Delta and Dahomey Basins
 
## Overview
 
This repository presents an integrated machine-learning workflow for screening, ranking, and evaluating potential geological CO₂ storage reservoirs using well-log-derived petrophysical properties and explainable artificial intelligence.
 
The project focuses on depleted and mature hydrocarbon reservoirs within the Niger Delta Basin and provides a framework that can be extended to the Dahomey Basin and other emerging Carbon Capture, Utilization and Storage (CCUS) regions.
 
The workflow combines reservoir characterization, storage suitability assessment, storage-capacity estimation, GIS-based fairway mapping, and explainable machine learning to support early-stage geological storage decision-making.
 
---
 
## Research Motivation
 
Geological Carbon Storage (GCS) is expected to play a critical role in achieving global net-zero emissions targets. While substantial storage characterization efforts have been undertaken in North America and Europe, comparatively limited machine-learning-driven storage assessments have been conducted within African sedimentary basins.
 
This project investigates whether well-log-derived petrophysical attributes can be integrated with explainable machine-learning workflows to rapidly identify and rank reservoirs suitable for long-term CO₂ sequestration.
 
---
 
## Research Question
 
Can well-log-derived petrophysical properties and explainable machine-learning techniques be integrated to reliably screen and rank depleted hydrocarbon reservoirs for geological CO₂ storage?
 
---
 
## Study Area
 
### Basin
 
- Niger Delta Basin
- Dahomey Basin (future expansion)
 
### Formation
 
- Agbada Formation
 
### Dataset
 
Well-log datasets from twelve wells containing:
 
- Gamma Ray (GR)
- Spontaneous Potential (SP)
- Resistivity
- Density (RHOB)
- Neutron Porosity (NPHI)
- Sonic Logs
 
Depth interval:
 
- 1,500–3,500 m
 
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
 
### Petrophysical Analysis
 
Derived parameters include:
 
- Effective Porosity (PHIE)
- Volume of Shale (Vsh)
- Permeability (K)
- Net-to-Gross Ratio (NTG)
- Seal Thickness
 
### Screening Criteria
 
Reservoir candidates are evaluated using:
 
- Reservoir depth
- Effective porosity
- Permeability
- Caprock thickness
- Structural integrity
- Storage-containment potential
 
### Machine Learning
 
Models include:
 
- Random Forest
- XGBoost
- K-Means Clustering
 
### Explainable AI
 
Interpretability is assessed using:
 
- SHAP (SHapley Additive Explanations)
- Feature Importance Analysis
- Blind-Well Validation
 
---
 
## Key Results
 
### Reservoir Quality
 
| Parameter | Range |
|------------|--------|
| Porosity | 18–31% |
| Permeability | 458–3251 mD |
| Reservoir Thickness | 6–73 m |
| Caprock Thickness | 3.3–102 m |
| Storage Capacity | 2.58–22.4 MM tonnes CO₂ |
 
### Storage Classification
 
- Excellent: 3 reservoirs
- Intermediate: 4 reservoirs
- Poor: 3 reservoirs
 
### Machine Learning Performance
 
| Metric | Value |
|----------|--------|
| Accuracy | 0.89 |
| F1 Score | 0.87 |
 
---
 
## Figures
 
### Reservoir Characterization
 
images/fig0_reservoir_characterisation.png
 
### Workflow Architecture
 
images/fig1_workflow_architecture_corrected.png
 
### SHAP Analysis
 
images/fig2_shap_analysis.png
 
### Storage Fairway Map
 
images/fig3_fairway_map.png
 
### Integrated Assessment
 
images/fig4_integrated_assessment.png
 
### Reservoir Quality Assessment
 
images/fig1b_reservoir_quality_assessment.png
 
---
 
## Research Portfolio
 
A complete research portfolio is available in:
 
```text
docs/portfolio.pdf
```
 
The portfolio includes:
 
- Research motivation
- Research gap
- Workflow architecture
- Reservoir ranking results
- SHAP analysis
- Storage fairway mapping
- Canadian CCS research alignment
- Proposed MSc research objectives
 
---
 
## Repository Structure
 
```text
CO2-Storage-Niger-Delta-Dahomey/
 
├── README.md
├── images/
├── notebooks/
├── src/
├── data/
├── docs/
├── LICENSE
├── requirements.txt
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
 
### Run Classification Workflow
 
```bash
jupyter notebook notebooks/02_xgboost_classification.ipynb
```
 
### Run SHAP Analysis
 
```bash
jupyter notebook notebooks/03_shap_explainability.ipynb
```
 
---
 
## Future Work
 
- Dahomey Basin assessment
- Dynamic CO₂ injection simulation
- Reservoir uncertainty quantification
- Geochemical modeling
- Seismic attribute integration
- Storage Suitability Index development
 
---
 
## Citation
 
If you use this repository or workflow, please cite:
 
> Ibe, U. (2026). Machine Learning-Based Screening and Ranking of Geological CO₂ Storage Reservoirs in the Niger Delta and Dahomey Basins. GitHub Repository.
 
---
 
## Author
 
**Umaru Ibe**
 
Geophysicist | Reservoir Characterization | Formation Evaluation | 3D Seismic Interpretation
 
Current Research Interests:
 
- Geological Carbon Storage
- Carbon Capture, Utilization and Storage (CCUS)
- Reservoir Characterization
- Explainable Artificial Intelligence
- Machine Learning for Subsurface Systems
- Subsurface Energy Systems
 
GitHub:
https://github.com/Umaru-Ibe
