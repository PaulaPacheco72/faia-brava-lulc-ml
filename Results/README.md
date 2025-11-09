
# Classification Results — Faia Brava LULC

This folder contains the main analytical results generated during the land use/land cover (LULC) classification of the Faia Brava Reserve.  
All figures originate from the experiments described in the Master’s Dissertation and serve as a visual summary of model performance.

The goal of this directory is to:
- Organize the key evaluation outputs
- Provide concise explanations to help interpret each figure
- Complement the full discussion available in the dissertation

---

## Contents of this Folder

### **1. F1-Score Plots**
Graphs showing per-class F1-scores for each dataset and classifier.
- Useful to compare the reliability of predictions across classes.
  
📍 *Insert file here (e.g., `final_map_over_ortho.png`)*

### **2. Cohen’s Kappa Comparison**
Bar plots summarizing the overall agreement between predictions and validation data.
- Highlights which dataset + classifier combination performed best.

📍 *Insert file here (e.g., `final_map_over_ortho.png`)*

---

## Interpretation Notes

- **UAV imagery** consistently produced higher accuracy than satellite imagery.  
- **Random Forest** was more stable and accurate than SVM across most tests.  
- **Haralick texture metrics** improved performance for both classifiers.  
- Best overall results were obtained with  
  **UAV RGB + GLI + Entropy + Random Forest**.

These findings are documented in detail in the dissertation.

---

## 📄 Full Thesis

For full methodology, data preparation, sampling procedures, and extended discussion of results, refer to:

`Dissertation/Dissertacao.pdf`

---

## Notes

Large imagery files and rasters are **not included** due to GitHub size limits.  
All figures in this folder can be reproduced using the workflow described in the dissertation.

---
