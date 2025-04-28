# README

## Stroke Survival Analysis using Lifelines

This project analyzes the survival time of patients based on health and demographic characteristics to predict stroke risks using **Survival Analysis techniques**, especially **Kaplan-Meier Estimation** and **Cox Proportional Hazards Model**.

---

## Dataset

- **Source**: [Stroke Prediction Dataset on Kaggle](https://www.kaggle.com/datasets/fedesoriano/stroke-prediction-dataset)
- **Description**:  
  The dataset includes features such as:
  - Gender
  - Age
  - Hypertension
  - Heart disease
  - Marital status
  - Type of work
  - Residence type (urban/rural)
  - Average glucose level
  - BMI
  - Smoking status
  - Stroke occurrence (target variable)

---

## Code Description

The attached Jupyter Notebook (`Untitled0.ipynb`) performs the following steps:

1. **Data Loading**:  
   - The stroke dataset is loaded into a pandas DataFrame.

2. **Data Preprocessing**:  
   - Missing values are handled (e.g., BMI imputation).
   - Categorical variables are encoded appropriately for survival analysis.

3. **Survival Analysis**:
   - **Kaplan-Meier Estimator** is used to estimate the survival function of different groups (e.g., smokers vs non-smokers, hypertensive vs non-hypertensive patients).
   - Survival curves are plotted for visual comparison.

4. **Cox Proportional Hazards Model**:
   - A **multivariate CoxPH model** is fitted to assess the impact of multiple factors (age, gender, glucose level, hypertension, heart disease, etc.) on stroke occurrence risk.
   - The model outputs hazard ratios (HR), p-values, and confidence intervals.

5. **Outcome**:
   - Identification of key risk factors that significantly affect stroke occurrence.
   - Visualization of survival probabilities across different patient groups.

---

## Requirements

- Python
- Jupyter Notebook
- pandas
- lifelines
- matplotlib
- seaborn

Install all dependencies using:

```bash
pip install pandas lifelines matplotlib seaborn
