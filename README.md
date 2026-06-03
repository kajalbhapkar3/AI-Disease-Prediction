# AI-Disease-Prediction
# Responsible AI-Driven Medical Diagnostic System
## 🏥 A Design Thinking + Generative AI Approach to Healthcare Analytics

[![Python](https://img.shields.io/badge/Python-3.9+-blue.svg)](https://www.python.org/)
[![Machine Learning](https://img.shields.io/badge/ML-Random%20Forest%20%7C%20HistGradientBoosting-green)](https://scikit-learn.org/)
[![Framework](https://img.shields.io/badge/Framework-Design%20Thinking-orange)](https://en.wikipedia.org/wiki/Design_thinking)

## 📌 Project Overview
This project shifts away from traditional machine learning workflows by pairing **Design Thinking Principles** with **Generative AI** to build an ethical, user-centric medical diagnostic system. The system maps **132 unique symptoms** to predict **42 distinct disease outcomes (prognoses)** while explicitly prioritizing model interpretability, clinical usability, and demographic fairness.

By implementing custom preprocessing pipelines and advanced ensemble models, this diagnostic tool achieves flawless classification metrics while retaining structural transparency for healthcare providers.

---

## 💡 The Design Thinking + GenAI Framework
Rather than just coding an isolated pipeline, Generative AI was leveraged as an active collaborative teammate across all 5 stages of the Design Thinking process:

### 1. Empathize (User-Centric Insights)
* **Objective:** Understand the functional and psychological needs of patients and medical practitioners.
* **GenAI Role:** Simulated clinical diagnostic scenarios and patient-doctor dialogues to identify crucial non-functional requirements, identifying that **explainability** is just as critical to doctors as raw predictive power.

### 2. Define (Problem Framing)
* **Objective:** Establish clear technical criteria based on human requirements.
* **GenAI Role:** Assisted in symptom-disease correlation analysis to identify key diagnostic features, solidifying a dual project focus: absolute technical accuracy paired with transparent feature interpretation.

### 3. Ideate (Model Exploration)
* **Objective:** Evaluate potential multi-class algorithmic alternatives.
* **GenAI Role:** Brainstormed classification frameworks optimized for high-dimensional, sparse binary data. Based on performance trade-offs, **Random Forest** (for structural transparency) and **HistGradientBoostingClassifier** (for handling rapid gradient steps) were chosen.

### 4. Prototype (Pipeline Development)
* **Objective:** Build, clean, and optimize end-to-end code structures.
* **GenAI Role:** Assisted in formulating streamlined data preparation workflows (mapping structural targets, feature encoding validation) and accelerating hyperparameter optimization for tree constraints and estimators.

### 5. Test (Robust Validation)
* **Objective:** Ensure performance generalizability and eliminate demographic blind spots.
* **GenAI Role:** Generated edge-case validation profiles to systematically challenge the models, confirming consistent performance across simulated patient groups.

---

## 🛠️ Tech Stack & Implementation Details
* **Language:** Python 3.9+
* **Libraries:** `scikit-learn`, `pandas`, `numpy`, `matplotlib`, `seaborn`
* **Data Dimension:** 132 symptom variables (Binary 0/1 inputs) ➡️ 1 target column (`prognosis` representing 42 medical conditions).

### The Pipelines
1. **Random Forest Classifier:** Selected for native explainability via feature importance matrices, enabling doctors to verify *why* a specific prediction was rendered.
2. **HistGradientBoostingClassifier:** Selected for accelerated gradient boosting capabilities on large feature sets, providing highly optimized decision boundaries.

---

## 📊 Performance & Key Findings

Both models were rigorously tested and achieved **perfect classification boundaries** due to clear separation parameters within the clean symptom matrices:

### 1. Random Forest Results
* **Training Accuracy:** 100%
* **Test Accuracy:** 100%
* **Precision / Recall / F1-Score:** 1.00 across all 42 target classes.

### 2. HistGradientBoosting Results
* **Training Accuracy:** 100%
* **Test Accuracy:** 100%
* **Precision / Recall / F1-Score:** 1.00 across all 42 target classes.

```text
               precision    recall  f1-score   support

    Accuracy                           1.00        42
   Macro Avg       1.00      1.00      1.00        42
Weighted Avg       1.00      1.00      1.00        42
