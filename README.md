# Clinical Decision Support Model for Hypertension Management

## Project Overview

This project is a healthcare analytics and machine learning solution designed to support clinical decision-making in hypertension management.

Using a cohort of **350 hypertensive patients**, the study combines **Python-based predictive modeling** with **Power BI-driven clinical analytics** to identify patients at risk of blood pressure control failure within a three-month period and uncover key drivers of treatment outcomes.

The goal is to move from descriptive reporting to a **clinical decision support system that enables early intervention and personalized treatment strategies**.

---

## Clinical Problem Statement

Uncontrolled hypertension is a major risk factor for cardiovascular complications and long-term morbidity.

In this dataset:
- Approximately **91% of patients failed to achieve blood pressure control**
- Only **9% achieved successful BP control within 3 months**

This raises two critical clinical questions:

- What factors predict blood pressure control failure?
- Which antihypertensive treatments are most effective for different patient profiles?

---

## Project Structure

healthcare-analytics-project/

│

├── notebooks/ → Machine Learning notebooks (Random Forest Classifier)

├── assets/ → Visuals (dashboard screenshots, model outputs, presentation)

├── powerpoint_presentation ([structured executive-style presentation](https://drive.google.com/file/d/1oTVWKHrvHAJoAtvlOmIowgl54abUct9j/view?usp=sharing(https://drive.google.com/file/d/1PZ1aG1DxE72M4E3851FHBU7p37K2Z7J5/view?usp=drive_link))

└── README.md

---

## Project Objectives

- Build a predictive model to identify patients at risk of treatment failure
- Analyze key clinical and behavioral drivers of blood pressure control
- Evaluate effectiveness of antihypertensive drug classes
- Develop insights for personalized treatment strategies
- Support early clinical intervention using data-driven methods

---

## Tech Stack

### Data Analysis & Processing
- Python
- Pandas
- NumPy

### Data Visualization
- Matplotlib
- Seaborn
- Power BI

### Machine Learning
- Scikit-learn
- Random Forest Classifier
- Predictive Modeling

### Data Preprocessing & Evaluation
- SMOTE (Synthetic Minority Oversampling Technique)
- StandardScaler
- Label Encoding
- Train-Test Split (80/20)
- Confusion Matrix
- Recall Evaluation
- Cross-Validation
- Feature Importance Analysis

---

## Methodology

### 1. Data Preparation
The dataset was cleaned and prepared for analysis, including encoding categorical variables such as medication adherence and clinical indicators.

### 2. Train-Test Split
The dataset was split into **80% training and 20% testing** to ensure unbiased evaluation.

### 3. Handling Class Imbalance
Due to severe class imbalance (only 9% success cases), SMOTE was applied **only on the training dataset** to prevent data leakage and ensure realistic evaluation.

### 4. Feature Scaling
StandardScaler was used to normalize numerical features for improved model performance.

---

## Predictive Modeling

A **Random Forest Classifier** was used to predict blood pressure control outcomes.

- Model trained on balanced training data
- Fixed random state used to ensure reproducibility
- Evaluated using confusion matrix and recall metrics

### Model Performance
- Achieved approximately **80% recall on positive cases**
- Strong performance in identifying high-risk patients
- Reduced risk of missed clinical interventions

---

## Key Clinical Insights

### 1. Major Predictors of Blood Pressure Control
- Baseline Systolic Blood Pressure
- Medication Adherence
- Chronic Kidney Disease (CKD)

### 2. Medication Adherence Impact
- Poor adherence strongly correlated with treatment failure
- Good adherence significantly improved patient outcomes
- Behavioral factors were as important as clinical variables

### 3. Drug Class Effectiveness
- Combination Therapy and Thiazide Diuretics showed strongest outcomes
- ACE Inhibitors showed no observed success in this cohort (requires further investigation)

### 4. Comorbidity-Based Response Patterns
- Diabetic patients responded best to Combination Therapy
- CKD patients showed improved outcomes with Thiazide Diuretics
- High-risk multimorbidity patients benefited from tailored treatment strategies

---

## Power BI Analytics

Power BI was used to complement machine learning insights through:

- Treatment outcome distribution analysis
- Patient segmentation by risk profile
- Drug effectiveness comparison
- Clinical trend visualization across comorbidities

This enabled better communication of insights for non-technical stakeholders.

---

## Business & Clinical Recommendations

- Implement predictive screening at point of care to identify high-risk patients early
- Strengthen medication adherence monitoring systems
- Adopt personalized treatment strategies based on comorbidity profiles
- Use data-driven insights to guide prescription decisions
- Improve follow-up and patient engagement strategies

---

## Impact

This project demonstrates how healthcare systems can transition from:

**Reactive care → Proactive clinical decision support**

By combining machine learning and clinical analytics, this system enables:
- Early identification of at-risk patients
- Improved treatment planning
- Better resource allocation
- Enhanced patient outcomes

---

## Limitations

- Dataset size was relatively small (350 patients)
- Analysis was observational, not clinical trial-based
- Results may require validation on larger populations
- External generalization may be limited

---

## Author

**Mary Udo**  
Data Science & Analytics | Healthcare AI | Predictive Modeling | Python & Power BI  
