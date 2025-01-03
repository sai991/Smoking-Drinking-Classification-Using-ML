

# Alcoholic Classification Using Body Signals

**Author**: Sai Prathyusha Kanisetti  
**Institution**: George Washington University  
**Instructor**: Prof. David W. Trott  
**Course**: Machine Learning (CSCI 6364)  
**Date**: 05/08/2024  

---

## Project Overview

Alcohol consumption poses significant public health challenges, with links to a range of physical and mental health disorders. This project leverages machine learning to classify individuals' drinking habits based on body signal data, contributing to better understanding and potential health interventions.

---

## Dataset

The dataset, sourced from Kaggle, contains:
- **Observations**: 991,346 (after cleaning: 906,676)
- **Features**: 24 (22 numerical, 2 categorical)
- Key metrics include hemoglobin, glucose levels, height, weight, etc.

**Preprocessing**:
- Duplicate removal (26 entries)
- Outlier analysis and removal:
  - Waistline (e.g., 999.0)
  - Cholesterol levels (e.g., HDL 8110, LDL 5119)
- Feature engineering (e.g., identifying blindness from eyesight metrics)

---

## Exploratory Data Analysis (EDA)

1. **Class Distribution**: Balanced between drinkers and non-drinkers.
2. **Gender Analysis**: Male participants are more likely to drink than females.
3. **Age Trends**: Younger and middle-aged individuals consume more alcohol.
4. **Smoking-Alcohol Correlation**: Non-smokers exhibit higher alcohol consumption.

---

## SMART Questions

1. Which age group is most habituated to drinking alcohol?  
2. Does every individual who drinks also smoke?  
3. Is there a significant impact of alcohol on eyesight?  
4. Does regular alcohol consumption affect the liver?

---

## Model Building

Three algorithms were employed:
1. **Random Forest Classifier**  
2. **Gradient Boosting**  
3. **XGBoost**

### Key Features
- **Set 1**: Gamma-GTP, HDL-cholesterol, age, smoking status, etc.
- **Set 2**: Added variables like left/right eyesight, triglycerides, and hemoglobin.

### Results
- **XGBoost** outperformed others with robust predictive accuracy and efficiency.
- Cross-validation yielded a mean score of ~0.735 with minimal variance.

---

## Conclusion

XGBoost proved most effective due to its:
- High accuracy
- Resource efficiency
- Versatility in handling noisy and incomplete datasets

The insights derived from this project underscore the critical health impacts of alcohol and highlight the value of machine learning in public health research.

---

## Files and Usage

- **Data**: [Dataset from Kaggle] (not included here)
- **Scripts**: Preprocessing, EDA, and model training files
- **Models**: Trained models for Random Forest, Gradient Boosting, and XGBoost

### Instructions

1. Preprocess the dataset:
   - Remove duplicates and outliers.
   - Engineer relevant features.
2. Perform EDA to gain insights into class distributions and trends.
3. Train models using the scripts provided.
4. Evaluate models with metrics like F1-score and ROC-AUC curves.

---

## Future Work

1. Extend analysis to other health metrics.
2. Explore deep learning models for feature representation.
3. Implement real-time predictions in a healthcare setting.

---

