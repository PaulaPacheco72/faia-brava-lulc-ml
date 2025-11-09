# Land Use and Land Cover Identification from Remote Sensing Imagery using Machine Learning  
### The Faia Brava Reserve Case Study

**Author:** Paula Pacheco  
**Year:** 2025

## Overview
This repository shares materials from the master’s dissertation “Identificação da Ocupação e Uso do Solo com Base em Imagens Provenientes de Deteção Remota e em Algoritmos de Machine Learning: a Reserva da Faia Brava como caso de estudo”.  
The study evaluates open-source workflows (QGIS + Orfeo Toolbox) to classify land use/land cover (LULC) in the Faia Brava Reserve (Portugal) using supervised ML and very-high-resolution imagery.

## Objectives
- Build an accessible, reproducible LULC workflow using open-source tools.  
- Compare **Random Forest (RF)** and **Support Vector Machine (SVM)**.  
- Use vegetation indices and texture features to improve accuracy.  
- Produce a final thematic LULC map for Faia Brava.

## Data
- **UAV orthomosaics (RGB)** at ~**2.7 cm/pixel**.  
- **Pléiades-Neo OrtoSat2023** satellite imagery at **30 cm/pixel** (RGB and IRG false color).  
- Ancillary GIS layers for sampling/validation. 

## Features & Methods
- Vegetation indices: **GLI, NDVI, SAVI, MSAVI**.  
- Texture: **Haralick (GLCM) metrics**.  
- Supervised ML: **Random Forest** and **SVM** (QGIS + **Orfeo Toolbox** plugin).  
- Evaluation: **confusion matrices, F1-score, Cohen’s Kappa**.

## Key Findings
- **UAV** imagery outperformed satellite inputs, especially when combined with texture.  
- **RF** showed more consistent performance; **SVM** was sensitive to spectral complexity.  
- Final map with **4 classes**: trees & shrubs, herbaceous vegetation, rocky outcrops, and other land uses.

## Repository Layout 
FaiaBrava_LULC/
├─ README.md
├─ Dissertation/
│ └─ Pacheco_Paula_Dissertation_2025.pdf
├─ Data/
├─ Scripts/
├─ Maps/
└─ Results/

## Software
- **QGIS** — used as the main GIS environment for visualization, sampling, and map production.  
- **Orfeo Toolbox (OTB)** — used through the QGIS interface for image processing, texture extraction, and machine learning classification (RF and SVM).  
- **GDAL/OGR** — core geospatial libraries underlying QGIS/OTB, supporting raster and vector operations.  
- **Optional Python tools** — used only for additional analysis or plotting (not required to reproduce the workflow).


## Citation
Pacheco, P. (2025). *Land Use and Land Cover Identification from Remote Sensing Imagery using Machine Learning: The Faia Brava Reserve Case Study*.  Master’s Dissertation, **Universidade do Algarve**.


