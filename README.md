# Machine-learning-prediction-of-externally-solidified-crystal

# ESC Prediction in Aluminum Die Casting — Machine Learning Framework

This repository contains the machine learning code used in the paper:

**“Machine Learning Prediction of Externally Solidified Crystal Formation in Aluminum Die Casting”**

The notebook reproduces model training, hyperparameter tuning, cross-validated evaluation, and SHAP-based feature importance analysis.

---

## Usage

1. Prepare a dataset as a pandas DataFrame named:

```
full_df
```

with a binary target column:

```
%esc
```

All remaining numeric columns are treated as predictor features.

2. Open and run the notebook:

```
Machine_learning_prediction_of_externally_solidified_crystal_formation_in_aluminum_die_casting_process.ipynb
```

3. Execute cells sequentially.

Each model block (MLP, SVM, KNN, Naive Bayes) is independent.

---

## Methods (Summary)

- 5-fold cross-validation
- Hyperparameter sweep
- Out-of-fold evaluation
- Confusion matrices
- SHAP global feature importance

Full methodological details are provided in the paper.

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
