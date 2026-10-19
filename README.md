# Heart_Disease_Prediction
603 Term Project


### download_data.py

1. Download four csv files from UCI database
    1. processed.cleveland.data
    2. processed.hungarian.data
    3. processed.switzerland.data
    4. processed.va.data

2. Merge the data into a single pandas dataframe + add column headers +  saves the data to a single csv file.

### Processing_data.ipynb
check dataset info
drop Na rows
converting columns from float to int, and then check datatypes

#### data preprocessing
One-Hot Encoding

Creating Dummy Variables for cp, thal and slope
Merge Dummy Variables to Main Data Frame 
drop unnecessary variables
save to new csv file (processed_data.csv)

<!-- problem-framing:start -->

## Problem and evidence

> **Do standard tabular classifiers outperform a simple baseline on held-out heart-disease records when preprocessing is fitted only on training data and dataset-source differences are respected?**

**Why it matters:** A course-project classifier is useful when its evaluation demonstrates reproducible learning rather than leakage from data preparation or source-specific patterns.

**Central tension:** Combining sources can increase sample size, but source differences and missing-value removal can change the population being evaluated. More complex classifiers need not transfer better.

[Full problem and verification plan](PROBLEM.md) · [Reusable framing prompt](PROBLEM_PROMPT.md)

<!-- problem-framing:end -->

