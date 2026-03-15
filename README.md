
# AD Drug Discovery AI Pipeline

QSAR Modeling and Generative AI for Alzheimer's Drug Discovery

This repository contains a computational pipeline for **Alzheimer’s disease (AD) drug discovery** integrating:

- QSAR modeling  
- Machine learning  
- Deep learning (Chemprop)  
- Generative AI (REINVENT)  
- Medicinal chemistry filtering  
- ADMET and toxicity screening  

The goal of this project is to **identify and generate novel molecules with potential activity against Alzheimer's disease–relevant targets using data-driven approaches.**

---

# Project Overview

The workflow combines **traditional QSAR modeling** with **generative molecular design**.

Pipeline:

Bioactivity Data Collection  
↓  
Data Cleaning and Standardization  
↓  
Exploratory Data Analysis (EDA)  
↓  
Descriptor Calculation  
↓  
Feature Selection  
↓  
QSAR Model Development  
↓  
Model Optimization and Evaluation  
↓  
Ensemble QSAR Models  
↓  
Generative AI Molecule Generation (REINVENT)  
↓  
Medicinal Chemistry Filtering  
↓  
ADMET and Toxicity Screening  

---

# Repository Structure

```
notebooks/

├── QSAR/
│   ├── pipeline/
│   ├── eda/
│   └── experiments/

└── GenAI/
    └── pipeline/
```

---

# QSAR Workflow

## Data Preparation

- notebooks/QSAR/pipeline/1-download_bioactivity_data_AD_targets.ipynb
- notebooks/QSAR/pipeline/2-data_cleaning.ipynb
- notebooks/QSAR/pipeline/4-data_preprocessing_smiles.ipynb

---

## Exploratory Data Analysis (EDA)

- notebooks/QSAR/eda/3-activity_classification_and_visualization.ipynb
- notebooks/QSAR/eda/6-EDA-pIC50-Normality.ipynb
- notebooks/QSAR/eda/9-count the number of features in each dataset.ipynb
- notebooks/QSAR/eda/10-performance_of_RF_model_with_different_feature_subsets.ipynb

---

## Descriptor Calculation and Feature Selection

- notebooks/QSAR/pipeline/5-descriptor_calculation_rdkit_mfp.ipynb
- notebooks/QSAR/pipeline/7-feature_filtering_by_collinearity_variance_and_pca_plotting.ipynb
- notebooks/QSAR/pipeline/8-rfecv_feature_selection.ipynb

---

## Traditional Machine Learning Models

- notebooks/QSAR/pipeline/13-hyperparameter_optimization_traditional_ml_models_with_nested_cv_bayesian_opt.ipynb
- notebooks/QSAR/pipeline/14-Trad_ML_models_rerun_with_opt_hyperparameters.ipynb
- notebooks/QSAR/pipeline/15-Trad_ML_model-saving.ipynb
- notebooks/QSAR/pipeline/16_trad_ML_final_model_performance.ipynb

---

## Chemprop Modeling

- notebooks/QSAR/pipeline/17_chemprop_data_preparation.ipynb
- notebooks/QSAR/pipeline/18_chemprop_hyperparameter_optimization.ipynb
- notebooks/QSAR/pipeline/19_chemprop_training_and_predictions.ipynb

---

## Ensemble Modeling and Model Comparison

- notebooks/QSAR/pipeline/20-ensemble-QSAR-model.ipynb
- notebooks/QSAR/pipeline/21_QSAR_performance_comparison.ipynb

---

## Experimental Notebooks

- notebooks/QSAR/experiments/12-hyperparameter_optimization_traditional_ml_models_no_nested_cv.ipynb
- notebooks/QSAR/experiments/13-hyperparameter_optimization_traditional_ml_models_with_nested_cv.ipynb

---

# Generative AI Workflow

## Training Data Preparation

- notebooks/GenAI/pipeline/1-prepare_training_data.ipynb

## Molecular Generation (REINVENT)

- notebooks/GenAI/pipeline/2-REINVENT_transfer_learning_and_sampling_workflow.ipynb

## Cleaning and Evaluation of Generated Molecules

- notebooks/GenAI/pipeline/3-Cleaning,_evaluation_and_selection_of_generated_molecules.ipynb

## Medicinal Chemistry Hygiene Filtering

- notebooks/GenAI/pipeline/4_Medicinal_chemistry_hygiene_filtering_of_generated_molecules.ipynb

## ADMET and Toxicity Screening

- notebooks/GenAI/pipeline/5_ADMET_and_toxicity_screening.ipynb

---

# Targets Used in This Study

The following Alzheimer's disease–relevant targets were included:

- BACE1
- Acetylcholinesterase (AChE)
- Butyrylcholinesterase (BuChE)
- Monoamine oxidase B (MAO-B)
- 5-HT6 receptor



---

# Methods and Tools

**Cheminformatics**
- RDKit

**Machine Learning**
- Scikit-learn
- XGBoost

**Deep Learning**
- Chemprop (D-MPNN)

**Generative AI**
- REINVENT

**Data Analysis**
- Pandas
- NumPy
- Matplotlib
- Seaborn

---

# Key Features

- Multi-target QSAR modeling
- Nested cross-validation with Bayesian optimization
- Ensemble modeling across ML and deep learning models
- Generative molecule design
- Medicinal chemistry filtering (PAINS and structural alerts)
- ADMET and toxicity screening


---

# Author

Erandi K  




---

# License

This repository is intended for **research and educational purposes**.
