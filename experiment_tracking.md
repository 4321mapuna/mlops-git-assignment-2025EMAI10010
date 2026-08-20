# Manual Experiment Tracking

The following table records the Decision Tree experiments performed during the project.

| Experiment ID | Model         | Hyperparameters | Preprocessing        | Feature Selection | Train/Test Split | Precision |  ROC-AUC |
| ------------- | ------------- | --------------- | -------------------- | ----------------- | ---------------- | --------: | -------: |
| EXP-01        | Decision Tree | Default         | None                 | All Features      | 80/20            |      0.97 |     0.97 |
| EXP-02        | Decision Tree | Max Depth = 5   | Scaling              | Selected Features | 80/20            |      0.98 |     0.98 |
| EXP-03        | Decision Tree | Max Depth = 7   | Scaling + Imputation | Selected Features | 80/20            |  **0.99** | **0.99** |
| EXP-04        | Decision Tree | Pruned Tree     | Scaling              | Selected Features | 80/20            |      0.98 | **0.99** |

---

## Experiment Comparison

### EXP-01 — Baseline

The first experiment established the baseline using a Decision Tree with default parameters and all available features.

**Results**

* Precision: 0.97
* ROC-AUC: 0.97

---

### EXP-02 — Depth-Constrained Tree

The second experiment introduced a maximum tree depth of 5 together with preprocessing and selected features.

**Results**

* Precision: 0.98
* ROC-AUC: 0.98

---

### EXP-03 — Additional Preprocessing

The third experiment used a maximum depth of 7 together with scaling, missing-value imputation, and selected features.

**Results**

* Precision: 0.99
* ROC-AUC: 0.99

This produced the highest recorded Precision among the experiments.

---

### EXP-04 — Pruned Decision Tree

The fourth experiment evaluated a pruned Decision Tree configuration with preprocessing and selected features.

**Results**

* Precision: 0.98
* ROC-AUC: 0.99

---

## Summary

The manually tracked experiments demonstrate how changes to model configuration, preprocessing, and feature selection can be recorded and compared systematically during machine learning development.
