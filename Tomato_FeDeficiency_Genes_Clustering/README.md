This folder contains the source code for the paper *"Roots in Action for the Fe Response: Early Response-Omics in Tomato Dependent on the Applied N-Form."*

## Overview
This repository contains the source code for the paper **"Roots in Action for the Fe Response: Early Response-Omics in Tomato Dependent on the Applied N-Form"**. The project focuses on analyzing iron deficiency gene enrichment in an RNA-Seq dataset for tomato plants.

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

## Similarity Measures & Linkage Methods
- **Distance Metric**: Euclidean distance  
- **Linkage Method**: Ward's method  

