# Dataset Overview

## Phase 1
- **Train Dataset:** `Dati_HIS_Serra_Cs_Hv_Sl_Zm_no_Fe` *(known as "Original Dataset")*
- **Test Datasets:**  
  - `Exp_I_Anna_Fe_Tomato` *(known as "Anna1")*  
  - `Exp_II_Anna_Fe_Tomato` *(known as "Anna2")*  
  - `Exp_Marco_tesista_Fe_Lupino` *(known as "Marco1")*  
  - `Marco2`  
  - `Merged_Anna1_Anna2_Marco_as_test`
  - `Merged_Anna1_Anna2_Marco1_Michele_as_test`

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

- **Test Dataset:** The same as **Phase 2** 
