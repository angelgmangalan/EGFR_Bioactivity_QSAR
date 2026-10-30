# EGFR_Bioactivity_QSAR
# EGFR Bioactivity Prediction Using Molecular Descriptors and Machine Learning

## Project Overview

This project develops a Quantitative Structure–Activity Relationship (QSAR) machine learning workflow to predict the bioactivity of chemical compounds against the Epidermal Growth Factor Receptor (EGFR).

The project uses bioactivity measurements from a BindingDB-style dataset and applies molecular descriptors, molecular fingerprints, and machine learning algorithms to estimate compound potency.

## Objectives

- Explore and preprocess the bioactivity dataset.
- Clean molecular structures using RDKit.
- Convert IC50 values into pIC50.
- Generate molecular descriptors and Morgan fingerprints.
- Develop and compare machine learning models.
- Evaluate models using scaffold-aware train/test splitting and cross-validation.
- Interpret model predictions using SHAP.
- Assess the applicability domain of the predictions.

## Technologies Used

- Python
- Jupyter Notebook
- Pandas and NumPy
- RDKit
- Scikit-learn
- Random Forest
- LightGBM
- XGBoost
- SHAP
- Matplotlib and Seaborn

## Repository Structure

```text
EGFR_Bioactivity_QSAR/
│
├── AD_bioactivity_QSAR.ipynb
├── dataset.tsv
├── README.md
├── requirements.txt
├── .gitignore
└── .gitattributes
```

The trained models and generated results are distributed separately through GitHub Releases.

## Dataset

The project uses a BindingDB-style TSV dataset containing molecular structures, target information, and bioactivity measurements.

Primary bioactivity endpoint: IC50 (nM).

## Machine Learning Models

1. Random Forest
2. LightGBM
3. XGBoost

## Model Evaluation

The workflow uses:

- R² score
- Root Mean Squared Error (RMSE)
- Mean Absolute Error (MAE)
- Scaffold-aware train/test split
- Scaffold-grouped cross-validation
- Applicability domain analysis

## How to Run

1. Clone this repository.
2. Install the required Python packages.
3. Open `AD_bioactivity_QSAR.ipynb`.
4. Ensure `dataset.tsv` is in the project directory.
5. Execute the notebook cells sequentially.

## Outputs

The project generates:

- Cleaned bioactivity dataset
- Molecular descriptors
- Model comparison results
- Predicted candidate compounds
- Trained machine learning models
- Preprocessing and metadata files

Download the complete output package from the repository's Releases section.

## Disclaimer

This project is intended for academic and research purposes. Machine learning predictions are computational estimates and are not experimental measurements or clinical recommendations.

