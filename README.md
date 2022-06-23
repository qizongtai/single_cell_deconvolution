# Single-Cell Deconvolution of Head and Neck Squamous Cell Carcinoma
Published 11 March 2021 at Cancers (https://www.mdpi.com/2072-6694/13/6/1230)  

![image](https://user-images.githubusercontent.com/33009124/162630970-0c95beb8-9d41-4900-8bb7-0be03af23ed3.png)

# scRNA-seq analysis
Expression levels were quantified as Ei,j = log2(TPMi,j/10 + 1), where TPMi,j refers to transcript-per-million for gene i in sample j, as calculated by RSEM (RNA-Seq by Expectation-Maximization) [65]. Malignant cells were identified by a set of potential epithelial markers consisting of all cytokeratins, EPCAM (Epithelial Cellular Adhesion Molecule), and SFN (Stratifin), as well as the copy number variation (CNV) analysis. t-SNE analysis of the remaining non-malignant cells identified eight major clusters. Briefly, we defined the clusters by DBSCAN (Density-Based Spatial Clustering of Applications with Noise: parameters Epsilon = 3 and MinPoints = 5) using the normalized gene-count matrix. Clusters were assigned to cell types based on strong differentiation expression of known marker genes. The T-cell cluster was further subdivided into four subtypes, which were annotated based on the differential expression of T-cell markers to represent the main patterns of variability: CCR7 and TCF7 for conventional CD4 (CD4conv), GZMA/B/H/K and PRF1 for conventional CD8 (CD8conv), PD1, LAG3, TIGIT, and CTLA4 for exhausted CD8 (CD8exhaust), and FOXP3 and CD25 for T regulatory cells (Tregs).


# survival analysis and hazard ratio measurement 
This Rmarkdown file is used for survival anlaysis of gene expression and deconvoluted cell-type proporations in head and neck patients in TCGA  "   

A brief introduction can found at the Method section: Survival analysis and hazard ratio measurement  
Patients were split at the median for each estimated cell type. The prognosis of each group of patients was examined by Kaplan–Meier survival, and log-rank tests compared the survival outcomes. Kaplan–Meier plots are presented for all the cell-type proportions, and the cell types with log-rank p-values less than 0.05 were defined as a prognostic cell type. Hazard ratios (HRs) and corresponding 95% confidence intervals (CIs) for risk of disease progression and mortality associated with high and low percentage of cell types were estimated using the Cox proportional-hazards model. Multivariable Cox model was adjusted for tumor stage, race, smoking status, and age. All statistical analyses were performed using R version 3.6.

