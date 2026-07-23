# Predictive Maintenance System

A Machine Learning-based Predictive Maintenance System that analyzes machine operating conditions and predicts potential machine failures before they occur. The project aims to help industries reduce unplanned downtime, improve operational efficiency, and support proactive maintenance strategies.

---

# Project Status

**Current Phase:** Model Optimization & Evaluation

The project has successfully completed data preparation, preprocessing, feature selection, and baseline model development using a Random Forest classifier.

Current efforts are focused on evaluating additional machine learning models, comparing performance metrics, and selecting the best-performing model before proceeding to explainability and deployment stages.

## Progress Tracker

| Phase                           | Status         |
| ------------------------------- | -------------- |
| Problem Definition              | ✅ Completed    |
| Dataset Understanding           | ✅ Completed    |
| Exploratory Data Analysis (EDA) | ✅ Completed    |
| Data Preprocessing              | ✅ Completed    |
| Feature Selection               | ✅ Completed    |
| Train-Test Split                | ✅ Completed    |
| Baseline Random Forest Model    | ✅ Completed    |
| Initial Performance Assessment  | ✅ Completed    |
| XGBoost Model Development       | 🔄 In Progress |
| Model Comparison & Selection    | ⏳ Pending      |
| Hyperparameter Tuning           | ⏳ Pending      |
| Final Model Evaluation          | ⏳ Pending      |
| SHAP Explainability             | ⏳ Pending      |
| Streamlit Dashboard             | ⏳ Pending      |
| FastAPI Backend                 | ⏳ Pending      |
| Deployment                      | ⏳ Pending      |

**Estimated Completion:** ~50%

---

# Problem Statement

Unexpected machine failures can result in production delays, increased maintenance costs, and operational disruptions. Traditional maintenance approaches are often reactive and address issues only after failures occur.

This project aims to develop a machine learning solution capable of predicting machine failures in advance, enabling maintenance teams to take preventive actions before breakdowns occur.

---

# Dataset

**Dataset Used:** AI4I 2020 Predictive Maintenance Dataset

## Features Used

* Type
* Air Temperature [K]
* Process Temperature [K]
* Rotational Speed [rpm]
* Torque [Nm]
* Tool Wear [min]

## Target Variable

Machine Failure

* 0 → No Failure
* 1 → Failure

## Dataset Statistics

| Metric           | Value  |
| ---------------- | ------ |
| Total Samples    | 10,000 |
| Training Samples | 8,000  |
| Testing Samples  | 2,000  |

---

# Development Journey

## Phase 1: Problem Understanding

* Studied predictive maintenance use cases.
* Defined machine failure prediction as a binary classification problem.
* Identified evaluation metrics and project objectives.

## Phase 2: Data Exploration

* Analyzed dataset structure and quality.
* Examined failure distribution.
* Investigated class imbalance.
* Explored feature relationships.

## Phase 3: Data Preprocessing

* Removed unnecessary columns.
* Encoded categorical machine types.
* Selected relevant predictive features.
* Generated processed dataset.
* Created training and testing datasets.

## Phase 4: Baseline Model Development

* Built machine learning pipeline.
* Trained Random Forest classifier.
* Generated baseline predictions.

## Phase 5: Initial Model Assessment

* Evaluated classification metrics.
* Generated confusion matrix.
* Performed feature importance analysis.

---

# Current Baseline Results (Random Forest)

The following metrics represent the current baseline model and serve as a benchmark for future improvements.

## Target Distribution

| Class          | Training | Testing |
| -------------- | -------- | ------- |
| No Failure (0) | 7,729    | 1,932   |
| Failure (1)    | 271      | 68      |

## Classification Report

| Class          | Precision | Recall | F1-Score |
| -------------- | --------- | ------ | -------- |
| No Failure (0) | 0.99      | 0.99   | 0.99     |
| Failure (1)    | 0.77      | 0.72   | 0.74     |

## Overall Performance

| Metric          | Value |
| --------------- | ----- |
| Accuracy        | 98%   |
| Macro Precision | 0.88  |
| Macro Recall    | 0.86  |
| Macro F1-Score  | 0.87  |

## Confusion Matrix

```text
[[1926, 6],
 [26, 42]]
```

---

# Feature Importance Analysis

| Rank | Feature                 | Importance |
| ---- | ----------------------- | ---------- |
| 1    | Torque [Nm]             | 0.330      |
| 2    | Rotational Speed [rpm]  | 0.224      |
| 3    | Tool Wear [min]         | 0.164      |
| 4    | Air Temperature [K]     | 0.130      |
| 5    | Process Temperature [K] | 0.127      |
| 6    | Type                    | 0.024      |

## Key Insight

The current baseline model indicates that Torque, Rotational Speed, and Tool Wear are the most influential factors in predicting machine failures.

---

# Current Repository Milestones

### Completed

* Dataset acquisition and understanding
* Exploratory Data Analysis
* Data preprocessing pipeline
* Feature selection
* Train-test split
* Random Forest baseline model
* Initial performance evaluation
* Feature importance analysis

### In Progress

* XGBoost model implementation
* Model comparison framework

### Upcoming

* Hyperparameter tuning
* SHAP explainability
* Streamlit dashboard
* FastAPI backend
* Model deployment

---

# Project Structure

```text
Predictive-Maitainace-System/

├── data/
│   ├── raw/
│   └── processed/
│
├── notebooks/
│
├── models/
│
├── README.md
│
└── requirements.txt
```

---

# Technology Stack

## Programming Language

* Python

## Data Processing

* Pandas
* NumPy

## Data Visualization

* Matplotlib
* Seaborn

## Machine Learning

* Scikit-Learn
* Random Forest
* XGBoost (In Progress)

## Explainable AI

* SHAP (Planned)

## Deployment

* Streamlit (Planned)
* FastAPI (Planned)

---

# Installation

```bash
git clone https://github.com/Houvered/Predictive-Maitainace-System.git

cd Predictive-Maitainace-System

pip install -r requirements.txt
```

---

# Future Roadmap

## Short-Term Goals

* Train and evaluate XGBoost model
* Compare Random Forest and XGBoost performance
* Improve minority-class detection
* Perform hyperparameter tuning

## Medium-Term Goals

* Integrate SHAP explainability
* Build Streamlit dashboard
* Develop FastAPI prediction API

## Long-Term Goals

* Real-time sensor integration
* Remaining Useful Life (RUL) estimation
* Failure type prediction
* Automated maintenance alerts
* Cloud deployment

---

# Expected Impact

Predictive maintenance enables organizations to transition from reactive maintenance to proactive maintenance. By identifying potential failures before they occur, industries can reduce downtime, optimize maintenance schedules, and improve overall equipment reliability.

<<<<<<< HEAD
---
=======
---

