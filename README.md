# Predictive Analysis of Heart Failure Mortality

## Introduction

Cardiovascular diseases (CVDs) are the leading cause of death worldwide, claiming an estimated 17.9 million lives each year, which represents 31% of all deaths globally. This project analyzes a heart failure dataset to predict mortality using machine learning techniques.

## Context

Heart failure is a common event caused by CVDs. The dataset used contains 12 features that can be used to predict mortality from heart failure. This analysis aims to contribute to the early detection and management of patients at high cardiovascular risk.

## Methodology

The analysis was performed using Orange, a visual data mining tool. The process followed is detailed below:

### 1. Data preparation
- Loading the heart failure dataset
- Review and selection of relevant features

### 2. Application of classification algorithms
Multiple algorithms were implemented and evaluated:
- Logistic Regression
- Random Forest
- Naive Bayes
- SVM (Support Vector Machine)
- Decision Tree
- kNN (k-Nearest Neighbors)

Each model was evaluated using cross-validation to determine its accuracy, recall, and other performance metrics.

### 3. Model evaluation
- Generation of confusion matrices to visualize true/false positives and negatives
- Comparison of metrics such as precision, recall, and F1-score to identify the best model

### 4. Exploratory analysis
- Creation of data tables classified according to model predictions
- Filtering data to separately analyze cases with positive and negative death events
- Visualization of the distribution of variables such as anemia in relation to fatal outcome

### 5. Advanced visualization
- Scatter plot relating age and time, colored according to death event
- Analysis and interpretation of patterns observed in the visualizations

## Results and analysis of the scatter plot

The scatter plot relating age vs. time shows significant patterns:

1. **Distribution by Survival**: Patients who survived (blue points) are distributed across the entire age range but concentrated in higher values of "time".

2. **Mortality Patterns**: Death cases (red points) tend to concentrate at low "time" values, especially below 100, regardless of age.

3. **Age Impact**: There is no strong linear correlation between age and time, but there is a slight trend of higher mortality in advanced ages (>70 years).

4. **Temporal Factors**: The higher density of red points at the bottom of the graph suggests that mortality risk is particularly high in the early follow-up periods.

5. **Atypical Cases**: Some older patients (>80 years) with high time values survived, indicating that factors other than age significantly influence the prognosis.

## Conclusions

The analysis reveals that time (possibly follow-up time or survival time) is a critical factor related to fatal outcomes in heart failure cases, more so than age itself. Early mortality is a common pattern among those who died, regardless of their age.

The predictive models developed can help identify high-risk patients who require early intervention, contributing to more effective prevention strategies in the management of cardiovascular diseases.

## Next steps

- Explore additional features that may improve predictive accuracy
- Implement data balancing techniques to address possible class imbalances
- Evaluate the clinical applicability of the model in real healthcare settings