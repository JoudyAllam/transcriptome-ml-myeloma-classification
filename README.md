# Transcriptome-Guided Machine Learning Prediction of Myeloma and Precursor States

**Author**: Joudy Allam  
**Institution**: Lebanese American University  
**Course**: BIF599H - Capstone Project

---

This repository hosts the reproducible computational pipeline developed for a capstone research project investigating transcriptomic signatures across multiple myeloma and its precursor states using supervised machine learning.

## Project Summary

Multiple myeloma (MM) is a hematologic malignancy consistently preceded by asymptomatic precursor conditions, including monoclonal gammopathy of undetermined significance (MGUS) and smoldering multiple myeloma (SMM). This project presents a machine learning framework for classifying clinical stages based on gene expression microarray data. The analytical workflow integrates rigorous preprocessing, differential expression analysis, biological enrichment, and classification modeling using Random Forest and Support Vector Machines.

The study aims to explore stage-specific transcriptomic patterns and evaluate the feasibility of minimal gene panels for accurate classification. The pipeline supports reproducible research and provides a modular structure suitable for adaptation to similar problems in oncology or transcriptomic biomarker discovery.

## Pipeline Highlights

- Preprocessing and normalization of microarray data (Affymetrix U133 Plus 2.0)
- Dual-stage quality control using `arrayQualityMetrics`, PCA, and manual review
- Differential gene expression across MGUS, SMM, NDMM, and Healthy controls
- Feature engineering using PCA, recursive feature elimination (RFE), GSVA, and RF importance
- Multi-class classification models with stratified train/test split and ROC analysis
- Modular design supporting reproducibility and extension

## Dependencies

This project was developed in **R (≥ 4.2)** using the following packages:

**Data Handling and Visualization**: `dplyr`, `ggplot2`, `ggrepel`, `gplots`, `grid`, `gridExtra`, `colorspace`, `DT`, `knitr`, `EnhancedVolcano`

**Microarray Preprocessing and Annotation**: `oligo`, `limma`, `affy`, `arrayQualityMetrics`, `genefilter`, `pd.hg.u133.plus.2`, `hgu133plus2.db`, `annotate`, `GEOquery`

**Statistical Modeling and Machine Learning**: `caret`, `randomForest`, `e1071`, `pROC`, `pvca`

**Functional Enrichment and Pathway Analysis**: `ReactomePA`, `GSVA`, `GSEABase`, `biomaRt`

**Miscellaneous**: `rvest`, `uwot`

---

## Requesting Access

This repository is private and not intended for public release. For academic or professional inquiries, or to request access for evaluation or collaboration, please contact the repository owner (joudyallam1000@gmail.com). 

Upon request, access may be granted to the full R code, analytical pipeline, key results and figures, and the final project report.
