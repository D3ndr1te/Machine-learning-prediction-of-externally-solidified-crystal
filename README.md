# ESC Prediction in Aluminum Die Casting — Machine Learning Framework

This repository contains the machine learning code and processed dataset used in the paper:

**“Machine Learning Prediction of Externally Solidified Crystal Formation in Aluminum Die Casting”**

The notebook reproduces model training, hyperparameter tuning, cross-validated evaluation, and SHAP-based feature importance analysis.

Full methodological details are described in the paper.

---

## Repository Structure

```
Cleaned_ML_MechanicalProperties_melt.csv
ESC_Casting_Notes.xlsx
Machine_learning_prediction_of_externally_solidified_crystal_formation_...
README.md
```

### Files

**Cleaned_ML_MechanicalProperties_melt.csv**  
Processed dataset used directly for machine learning modeling.

**ESC_Casting_Notes.xlsx**  
Original casting dataset before preprocessing.  
Provided for transparency and for researchers interested in alternative data processing workflows.

**Machine_learning_prediction_of_externally_solidified_crystal_formation_…**  
Main Jupyter notebook (exported from Google Colab) containing all ML pipelines and analysis.

**README.md**  
Repository documentation.

---

## Usage

1. Load the cleaned dataset:

```
Cleaned_ML_MechanicalProperties_melt.csv
```

as a pandas DataFrame named:

```python
full_df
```

2. Open the notebook and run cells sequentially:

```
Machine_learning_prediction_of_externally_solidified_crystal_formation_…
```

Each model block (MLP, SVM, KNN, Naive Bayes) is independent.

---

## Methods (Summary)

- 5-fold cross-validation
- Hyperparameter sweep
- Out-of-fold evaluation
- Confusion matrices
- SHAP global feature importance

See the paper for full methodology.

---

## Dependencies

```bash
pip install numpy pandas matplotlib seaborn scikit-learn shap
```

---

## Reproducibility

- Fixed random seeds
- Cross-validation prevents data leakage
- SHAP explanations include preprocessing pipelines

---

## License

MIT License
