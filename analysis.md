# Experiment Analysis

Multiple Decision Tree configurations were evaluated on the Palmer Penguins classification task.

## Key Observations

* The baseline Decision Tree recorded a Precision and ROC-AUC of **0.97**.
* EXP-02 improved the recorded Precision and ROC-AUC to **0.98** after modifying the model configuration and preprocessing.
* EXP-03 produced the highest recorded Precision of **0.99** and ROC-AUC of **0.99**.
* The pruned Decision Tree in EXP-04 retained a ROC-AUC of **0.99** while recording a Precision of **0.98**.
* Recording each experiment separately made it easier to compare changes in model configuration, preprocessing, and evaluation metrics.

## MLOps Learning

The project demonstrates the importance of maintaining a structured history of machine learning experiments.

Instead of modifying a model without recording previous results, each experiment captures:

* Model configuration
* Hyperparameters
* Preprocessing choices
* Feature-selection choices
* Evaluation metrics

Git-based version control provides an additional history of changes made during experimentation.

## Conclusion

Among the recorded experiments, **EXP-03 achieved the strongest overall result**, with both Precision and ROC-AUC reaching **0.99**.

The project provided a foundational introduction to experiment tracking before moving to automated tools such as MLflow in more advanced MLOps workflows.
