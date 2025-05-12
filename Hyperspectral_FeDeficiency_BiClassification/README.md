# Dataset Overview

## Phase 1
- **Train Dataset:** `Dati_HIS_Serra_Cs_Hv_Sl_Zm_no_Fe` *(known as "Original Dataset")*
- **Test Datasets:**  
  - `Exp_I_Anna_Fe_Tomato.txt` *(known as "Anna1")*  
  - `Exp_II_Anna_Fe_Tomato.txt` *(known as "Anna2")*  
  - `Exp_Marco_tesista_Fe_Lupino.txt` *(known as "Marco1")*  
  - `Marco_lupin_Polypen_last_day_24_0_2025.txt` *(Known as Marco2. It has fewer columns/features and hence, can not be used in merged-dataset experiments)* 
  - `Merged_Anna1_Anna2_Marco_as_test.txt`
  - `Merged_Anna1_Anna2_Marco1_Michele_as_test.txt` *(here we have merged all samples of "Michele_test.txt" which are 143 samples of "-N+Fe")*

## Phase 2
- **Train Dataset:** `Dati_HIS_Serra_Cs_Hv_Sl_Zm_no_Fe_modified`  
  - This modified train set includes **36 manually-added samples** from `"Michele_test"` to `"Dati_HIS_Serra_Cs_Hv_Sl_Zm_no_Fe"`considering first 9 samples of each plant.

- **Test Dataset:** `Merged_Anna1_Anna2_Marco1_Michele_fornew_trainSet`  
  - This test set was constructed as follows:  
    1. **Created `"Michele_test2"`** by removing the 36 samples of `"Michele_test"` that were added to the train set (`Dati_HIS_Serra_Cs_Hv_Sl_Zm_no_Fe_modified`).  
    2. **Merged** the following datasets to form the new test set:  
       - `Exp_I_Anna_Fe_Tomato` *(known as "Anna1")*  
       - `Exp_II_Anna_Fe_Tomato` *(known as "Anna2")*  
       - `Exp_Marco_tesista_Fe_Lupino` *(known as "Marco1")*  
       - `Michele_test2`
      
## Phase 3
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
