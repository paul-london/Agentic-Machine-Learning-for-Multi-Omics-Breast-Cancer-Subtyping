<p align="center">
  <a href="https://www.meetup.com/tampa-bay-biotech/">
    <img src="https://github.com/user-attachments/assets/a2b2d193-58b1-44f1-90dd-2ce633b6c141" width="729" height="410">
  </a>
</p>

# Agentic Machine Learning for Multi-Omics Breast Cancer Subtyping

This project implements a machine learning pipeline to classify breast cancer samples into intrinsic molecular subtypes using the PAM50 gene expression panel. The PAM50 signature uses expression levels from 50 genes to categorize tumors into biologically distinct subtypes including Luminal A, Luminal B, HER2-enriched, Basal-like, and Normal-like. These subtypes are associated with differences in prognosis, tumor biology, and treatment response.

The workflow processes gene expression data from publicly available cancer genomics datasets such as The Cancer Genome Atlas and Molecular Taxonomy of Breast Cancer International Consortium, performs preprocessing and feature extraction, and applies statistical and machine learning techniques to reproduce or approximate PAM50 subtype classification. Dimensionality reduction and visualization methods such as PCA are used to explore clustering patterns among tumor samples, while model outputs are evaluated to assess classification accuracy and biological consistency.

The goal of the project is to demonstrate how genomic data can be integrated with machine learning techniques to support molecular subtype prediction and exploratory analysis in cancer genomics.

## Table of Contents

- Background
- Data Engineering
- Contact

## Background

Breast cancer is a biologically heterogeneous disease, meaning tumors that appear similar under a microscope can behave very differently at the molecular level. Advances in gene expression profiling have enabled researchers to classify breast tumors into molecular subtypes that better reflect underlying tumor biology and clinical outcomes. One widely used approach is the PAM50 gene expression signature, which measures the expression of 50 genes to categorize tumors into intrinsic subtypes: Luminal A, Luminal B, HER2-enriched, Basal-like, and Normal-like. These subtypes are associated with differences in prognosis, treatment response, and biological characteristics such as proliferation, hormone receptor signaling, and growth factor pathway activation.

Large cancer genomics initiatives have made it possible to study these molecular subtypes at scale. Projects such as The Cancer Genome Atlas and Molecular Taxonomy of Breast Cancer International Consortium provide publicly available datasets containing gene expression measurements from thousands of tumor samples. Researchers use these datasets to explore subtype-specific patterns, validate molecular classifiers, and develop computational methods for cancer subtype prediction.

In this project, gene expression data are used to explore and reproduce PAM50-based breast cancer subtype classification using computational and machine learning techniques. By applying data preprocessing, dimensionality reduction, and classification methods, the project demonstrates how genomic data can be leveraged to identify biologically meaningful tumor subtypes and support data-driven insights in cancer genomics.

## Data Engineering

The data engineering pipeline prepares gene expression data for downstream analysis and subtype classification. Raw expression data from large-scale cancer genomics datasets such as The Cancer Genome Atlas and Molecular Taxonomy of Breast Cancer International Consortium were imported and processed to ensure consistency and usability for analysis. Initial steps included cleaning the dataset, handling missing values, and aligning gene identifiers to match the 50 genes defined in the PAM50 panel.

After filtering for the PAM50 genes, the data were transformed into a structured format where each row represents a tumor sample and each column represents the expression level of a specific gene. Normalization and scaling were applied to reduce technical variability across samples and ensure that gene expression levels were comparable. These preprocessing steps help stabilize the data distribution and improve the performance of downstream statistical and machine learning analyses.

Additional feature preparation steps included verifying gene coverage across samples and removing samples with incomplete data. The resulting dataset represents a clean expression matrix suitable for dimensionality reduction, visualization, and subtype classification using the PAM50 gene set. This engineered dataset serves as the foundation for the modeling and exploratory analysis stages of the project.

## Contact
[Paul London](https://www.linkedin.com/in/palondon)
