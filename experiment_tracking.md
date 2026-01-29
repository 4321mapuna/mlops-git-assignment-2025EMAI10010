## Manual Experiment Tracking Table

| Experiment ID | Model Type    | Hyperparameters | Preprocessing Steps | Feature Selection | Train/Test Split | Precision | AUC Score |
|--------------|---------------|-----------------|---------------------|-------------------|------------------|-----------|-----------|
| EXP-01       | Decision Tree | Default         | None                | All features      | 80/20            | 0.97      | 0.97      |
| EXP-02       | Decision Tree | Max depth = 5   | Scaling             | Selected          | 80/20            | 0.98      | 0.98      |
| EXP-03 | Decision Tree | Max depth = 7 | Scaling + Imputation | Selected | 80/20 | 0.99 | 0.99 |
| EXP-04 | Decision Tree | Pruned Tree | Scaling | Selected | 80/20 | 0.98 | 0.99 |
