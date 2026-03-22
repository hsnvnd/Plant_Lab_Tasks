## Overview
This repository contains the source code for the paper **"Iron Deficiency Detection in Plants: Machine Learning to Uncover Significant Wavelengths in Reflectance Spectra"**. The project focuses on iron deficiency detection in Hyperspectral-imaging datasets for tomato, cucumber, barley, maize, and lupine.


## Dataset Overview

## Phase 1
- **Train Dataset:** `Dati_HIS_Serra_Cs_Hv_Sl_Zm_no_Fe.txt` *(known as "Original Dataset")*
- **Test Datasets:**  
  - `Exp_I_Anna_Fe_Tomato.txt` *(known as "Anna1")*  
  - `Exp_II_Anna_Fe_Tomato.txt` *(known as "Anna2")*  
  - `Exp_Marco_tesista_Fe_Lupino.txt` *(known as "Marco1")*  
  - `Marco_lupin_Polypen_last_day_24_0_2025.txt` *(Known as Marco2. It has fewer columns/features and hence, can not be used in merged-dataset experiments)* 
  - `Merged_Anna1_Anna2_Marco1_as_test.txt`
  - `Merged_Anna1_Anna2_Marco1_Michele_as_test.txt` *(here we have also merged all samples of "Michele_test.txt" which which consist of 71 samples of young leaves with the "-N+Fe" condition)*
      
## Phase 2
- **Train Dataset:** `Dati_HIS_Serra_Cs_Hv_Sl_Zm_no_Fe_add36_randomly`  
  - This modified train set includes **36 randomly-added samples** from the refined version of `"Michele_test"` titled `"Michele_column_names_editted"` to `"Dati_HIS_Serra_Cs_Hv_Sl_Zm_no_Fe"`.

- **Test Dataset:** `Merged_Anna1_Anna2_Marco1_Random_Michele_fornew_trainSet`  
  - This test set was constructed as follows:  
    1. **Created `"Michele_test3"`** by removing the 36 samples of `"Michele_column_names_editted"` that were added to the train set (`Dati_HIS_Serra_Cs_Hv_Sl_Zm_no_Fe_add36_randomly`).  
    2. **Merged** the following datasets to form the new test set:  
       - `Exp_I_Anna_Fe_Tomato` *(known as "Anna1")*  
       - `Exp_II_Anna_Fe_Tomato` *(known as "Anna2")*  
       - `Exp_Marco_tesista_Fe_Lupino` *(known as "Marco1")*  
       - `Michele_test3`

## Implementation
- **Notebook:** `Hyperspectral_FeDeficiency_BiClassification_IndexCreation.ipynb`
- This notebook contains the implementation and is used for both Phase 1 and Phase 2.

## Environment
Python version: 3.11.5
This project was developed and tested using:
- Core libraries include:
- NumPy  
- Pandas  
- Scikit‑learn  
- SHAP
- Matplotlib  
- Seaborn

## Citation
If you use this repository, please cite:
**"Iron Deficiency Detection in Plants: Machine Learning to Uncover Significant Wavelengths in Reflectance Spectra"**
(BibTeX entry will be added once available.)
