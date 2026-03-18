# Machine Learning Framework for Bulk Modulus Prediction

## Overview
This repository presents a comprehensive machine learning pipeline for predicting the **bulk modulus of inorganic materials**. It compares multiple regression models and validates predictions using first-principles Density Functional Theory (DFT), enabling a scalable and cost-effective approach for materials property prediction.

## Key Features
- Comparative analysis of:
  - Random Forest (RF)
  - Support Vector Regression (SVR)
  - Gradient Boosted Regressor (GBR)
  - XGBoost
  - CatBoost
- Feature engineering using:
  - Matminer (Magpie descriptors)
  - Pymatgen (structure validation & parsing)
- Hyperparameter optimization with GridSearchCV
- Model interpretability via SHAP analysis
- DFT validation using GPAW (Birch–Murnaghan EOS)

## Workflow
1. Data preprocessing and cleaning  
2. Feature extraction (compositional + structural)  
3. Train-validation-test split (70-15-15)  
4. Model training and tuning  
5. Performance evaluation (R², RMSE)  
6. SHAP-based interpretation  
7. DFT validation  

## Results
- All models achieved strong performance (R² > 0.92)  
- XGBoost showed best accuracy–efficiency balance  
- Valence Potential Average (VPA) identified as key feature  
- Good agreement between ML and DFT results (e.g., BC₂N)

## Installation
```bash
pip install numpy pandas scikit-learn matplotlib pymatgen matminer shap xgboost catboost ase gpaw
```


## Authors 

- Sabyasachi Roy
- Bhupratim Roy
- Md. Tanvir Ahmed 

