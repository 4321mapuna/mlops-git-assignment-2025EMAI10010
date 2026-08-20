# MLOps Experiment Tracking with Git

A coursework project demonstrating **manual machine learning experiment tracking and Git-based version control practices** using Decision Tree experiments on the Palmer Penguins dataset.

This project was completed as part of **DSC524 – Designing MLOps for Enterprises** in the M.Tech Artificial Intelligence and Data Science program at IIIT Kottayam.

---

## 🎯 Project Objective

The objective of this project was to understand foundational MLOps practices by tracking changes across multiple machine learning experiments.

The project focuses on:

* Git-based version control
* Experiment tracking
* Hyperparameter experimentation
* Preprocessing variations
* Feature-selection variations
* Model evaluation
* Comparing experiment results

---

## 🐧 Dataset

The experiments use the **Palmer Penguins dataset**, containing observations of three penguin species:

* Adelie
* Chinstrap
* Gentoo

The dataset includes physical and categorical characteristics such as bill measurements, flipper length, body mass, island, and sex.

Detailed dataset information is available in [`dataset_info.md`](dataset_info.md).

---

## 🧪 Experiment Tracking

Four Decision Tree experiments were manually tracked with variations in:

* Hyperparameters
* Preprocessing
* Feature selection
* Precision
* ROC-AUC

The best recorded experiment achieved:

* **Precision: 0.99**
* **ROC-AUC: 0.99**

The complete experiment table is available in:

[`experiment_tracking.md`](experiment_tracking.md)

---

## 📊 Experiment Summary

| Experiment | Configuration                              | Precision |  ROC-AUC |
| ---------- | ------------------------------------------ | --------: | -------: |
| EXP-01     | Baseline Decision Tree                     |      0.97 |     0.97 |
| EXP-02     | Max Depth = 5 + preprocessing              |      0.98 |     0.98 |
| EXP-03     | Max Depth = 7 + preprocessing + imputation |  **0.99** | **0.99** |
| EXP-04     | Pruned Decision Tree                       |      0.98 | **0.99** |

---

## 🔄 MLOps Workflow Demonstrated

```text
Baseline Experiment
        ↓
Record Configuration & Metrics
        ↓
Modify Hyperparameters / Preprocessing
        ↓
Run New Experiment
        ↓
Compare Results
        ↓
Track Changes with Git
        ↓
Document Findings
```

---

## 📂 Repository Structure

```text
mlops-git-experiment-tracking/
├── README.md
├── analysis.md
├── dataset_info.md
├── experiment_tracking.md
└── .gitignore
```

### Files

* `README.md` — Project overview and experiment summary
* `analysis.md` — Findings from the recorded experiments
* `dataset_info.md` — Palmer Penguins dataset information
* `experiment_tracking.md` — Manual experiment tracking table

---

## 💡 What This Project Demonstrates

This project demonstrates foundational MLOps concepts including:

* Tracking ML experiments systematically
* Comparing model configurations
* Recording evaluation metrics
* Managing experiment changes using Git
* Documenting model-development decisions

---

## ⚠️ Project Scope

This repository focuses on **Git-based workflow and manual experiment tracking**.

The model-training implementation is not included in this repository. More advanced experiment tracking using tools such as MLflow is covered in later MLOps projects.

---

## 👤 Author

**Anupam K Ajith**
AI/ML & GenAI | M.Tech AI & Data Science @ IIIT Kottayam | Python | RAG | MLOps
