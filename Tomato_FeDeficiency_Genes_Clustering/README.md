## Overview
This repository contains the source code for the paper **"The Early Response to Urea, Nitrate, or Ammonium and Iron Resupply in Tomato Roots Highlights the Induction of FER, bHLHs, UMAMITs and MATEs"**. The project focuses on analyzing iron deficiency gene enrichment in an RNA-Seq dataset for tomato plants.

## Purpose
The primary goal of this study is to investigate the enrichment of iron deficiency genes in an RNA-Seq dataset and identify meaningful patterns in gene expression.

## Methods
The analysis is performed using clustering techniques to categorize gene expression patterns efficiently:

1. **Row-Based Clustering (K-Means Clustering)**  
   - Genes are first clustered based on similarity using K-Means.
   - The optimal number of clusters (**K**) is determined using:
     - **Silhouette Score**
     - **Davies-Bouldin Index**
     - **Inertia**

2. **Hierarchical Column-Based Clustering**  
   - Once row-based clusters are formed, hierarchical clustering is applied to gene expression patterns.
   - This step is performed for:
     - **All genes**
     - **Only iron deficiency genes within each cluster**
   - The results are visualized using **heatmaps**.
   - **Similarity Measures & Linkage Methods**  
     - **Distance Metric**: Euclidean distance  
     - **Linkage Method**: Ward's method  

## Dataset Overview
- **FPKM_tomato.txt**: Contains gene expression values for 15 samples.  
- **Tomato_columns.txt**: Explains the treatment status of each column in `FPKM_tomato.txt`.  
- **iron_genes1.txt**:  
  - Column 1: Fe deficiency gene names.  
  - Column 2: Descriptions of Fe deficiency genes.  
  - Extracted from *"A Hitchhiker’s Guide to the Arabidopsis Ferrome."*  
- **GeneNames.txt**:  
  - Tomato gene names corresponding to `FPKM_tomato.txt`.  
  - Gene names found in `"annotation Solyc_ITAG4_0.xlsx"`.  
  - Important gene names located in Column L of `"annotation Solyc_ITAG4_0.xlsx"`.

## Citation
If you use this repository, please cite:
---
@article{lodovici2026earlyresponse, title={The Early Response to Urea, Nitrate, or Ammonium and Iron Resupply in Tomato Roots Highlights the Induction of FER, bHLHs, UMAMITs, and MATEs}, author={Lodovici, A. and Zhang, L. and Tomasi, N. and others}, journal={Physiologia Plantarum}, volume={178}, number={4}, pages={e70977}, year={2026}, doi={10.1111/ppl.70977} }
---
