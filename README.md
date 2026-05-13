# Decoding a 4000-Year-Old Economy: Analysis of Cuneiform Tablets of Old Babylon

## Summary

This project presents a computational analysis of Old Babylonian administrative cuneiform tablets using modern data science, distributed computing, and machine learning methodologies. Drawing upon digitized archaeological records from the Cuneiform Digital Library Initiative (CDLI), the study investigates whether the physical dimensions of clay tablets encode hidden administrative structures, production standardization, and institutional logic within ancient Mesopotamian economies.

The project operates at the intersection of:
- Economic history
- Computational archaeology
- Big data engineering
- Statistical learning

Rather than treating tablet measurements as passive archaeological descriptors, this work models tablet geometry as an economic signal. Through PySpark-based preprocessing pipelines, unsupervised anomaly detection, ensemble learning architectures, and SHAP interpretability analysis, the project reconstructs structural regularities embedded within bureaucratic production systems nearly four thousand years old.

The repository demonstrates how large-scale machine learning workflows can be adapted to historical and archaeological datasets while preserving interpretability and research transparency.

---

# Objectives

The primary objective of this study is to determine whether measurable geometric characteristics of Old Babylonian tablets reflect underlying administrative or economic organization.

Key questions include:

1. Can dimensional tablet features reveal standardized bureaucratic production?
2. Are anomalous tablets statistically distinguishable from ordinary administrative records?
3. Which geometric variables contribute most strongly to anomaly classification?


---
# Dataset Description

The analysis uses tablet metadata derived from the:

- **Cuneiform Digital Library Initiative (CDLI)** repository

The dataset contains archaeological records associated with:
- administrative tablets
- economic texts
- geometric measurements
- excavation metadata
- object classifications

Primary numerical features include:
- Tablet Height
- Tablet Width
- Tablet Thickness

Additional metadata fields were processed for filtering, normalization, and classification.

---

## Technical Architecture & Highlights
* **Phase 1: Distributed Data Engineering**
    * Ingested and vectorized 75,000+ raw CDLI metadata records using **PySpark**.
    * Deployed **K-Means clustering** and Euclidean distance mapping for unsupervised anomaly detection.
* **Phase 2: Ensemble Modeling & Explainable AI (XAI)**
    * Benchmarked non-linear classifiers (**Random Forest**, **AdaBoost**, **Decision Trees**) to isolate structural outliers.
    * Applied **SHAP TreeExplainer** to crack the "black box" of the ensemble models and identify the exact geometric rules defining specialized economic transactions.
---

## Technical Stack
* **Big Data:** Apache Spark (PySpark MLlib & SQL)
* **Machine Learning:** Scikit-Learn, Ensemble Methods
* **Explainable AI:** SHAP (SHapley Additive exPlanations)
* **Visualization:** Matplotlib, Seaborn 
* **Environment:** Python 3.x, Jupyter Notebooks
---

## Repository Structure
```text
├── Babylonia_Part_1.ipynb     
├── Babylonia_Part_2.ipynb          
├── babylon_anomalies.csv                
├── Babylonia_Notebook_1.pdf          
├── Babylonia ml part 2.pdf             
└── README.md
```
---

## Statistical Observations & Key Findings

**Phase 1: Unsupervised Clustering and Anomaly Detection**
* **Dimensional Vectorization:** Successfully processed 75,000+ raw CDLI records, establishing a standardized baseline for Old Babylonian administrative tablet geometries.
* **Anomaly Thresholding:** Deployed K-Means clustering, utilizing Euclidean distance from cluster centroids to mathematically isolate the top 5% of geometric outliers, proving the existence of non-standard administrative structures.

**Phase 2: Supervised Classification & Interpretability**
* **Ensemble Superiority:** The optimized Random Forest classifier achieved a cross-validated accuracy of **96.86%**, demonstrating that non-linear ensemble methods significantly outperform baseline logistic models in detecting complex structural anomalies.
* **Feature Importance (SHAP):** Model interpretability extracted via SHAP TreeExplainer revealed that **tablet width** (accounting for 76.1% of feature importance) was the dominant structural determinant for specialized economic ledgers, outweighing overall volume or thickness.

---

## Conclusion
This pipeline successfully bridges distributed computing and ancient economics, proving that millennia-old administrative systems possessed mathematically detectable standardization. By leveraging PySpark to handle the sheer scale of the CDLI archives and utilizing SHAP to decode our ensemble models, we move beyond theoretical historical assumptions into statistical proof. The data confirms that physical geometry, specifically tablet width, was intentionally manipulated by Babylonian administrators to categorize specialized economic ledgers. 

---

## About Me
I am *Abhilasha Das*, a Data Science student with a foundation in Economics, driven by a love for using computational research to solve real-world puzzles. From analyzing celestial spectral data to decoding ancient economic structures, I like to find the human story hidden inside big data.
