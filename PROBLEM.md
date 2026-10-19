# Research and learning problem

> **Do standard tabular classifiers outperform a simple baseline on held-out heart-disease records when preprocessing is fitted only on training data and dataset-source differences are respected?**

**Why it matters:** A course-project classifier is useful when its evaluation demonstrates reproducible learning rather than leakage from data preparation or source-specific patterns.

**Central tension:** Combining sources can increase sample size, but source differences and missing-value removal can change the population being evaluated. More complex classifiers need not transfer better.

**Current evidence and gap:** [README.md](README.md) describes combining UCI tables, removing missing rows and encoding categories. It does not establish source-aware generalization or clinical usefulness. [Processing_data.ipynb](Processing_data.ipynb) and [Heart_Disease_Prediction.ipynb](Heart_Disease_Prediction.ipynb) are the documented analysis entry points.

**Decisive verification:** Audit duplicates and label definitions before splitting. Fit imputation and encoding within each training fold; compare a simple majority/logistic baseline with candidate classifiers using a common untouched test set and, where viable, source-held-out evaluation. Report discrimination, calibration, class-specific errors and exclusions. If improvement disappears after leakage controls, treat that as the main learning result.

This is a retrospective methods exercise and prospective verification plan, not a medical decision tool.
