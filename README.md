# STUDENT PERFORMANCE CLASSIFICATION

## OVERVIEW
This project builds a multi-class classification model to predict student performance levels (Low, Moderate, High) using a dataset of 8,000+ records and 26 features.  
The model incorporates academic behavior, lifestyle factors, and AI usage patterns to generate accurate predictions.

## OBJECTIVES 
- Predict student performance categories  
- Analyze impact of AI usage on academic outcomes  
- Identify key factors affecting performance  
- Build an optimized machine learning pipeline  

## DATASET
The dataset contains 26 features grouped as:

**Academic:** Study hours, consistency, concept understanding, improvement rate  
**AI Usage:** Usage time, tools used, dependency score, purpose  
**Lifestyle:** Sleep hours, social media usage, tutoring  
**Engagement:** Class participation, grade level  

**Target:** Performance category (Low / Moderate / High)

## METHODOLOGY

### Data Processing  
- Encoding categorical variables  
- Feature scaling  
- Handling missing values  

### Feature Selection  
- SelectKBest used  
- Reduced features from 26 to 10  
- Maintained ~99% performance  

### Models Evaluated  
- Logistic Regression  
- Gradient Boosting  
- XGBoost  
- SVM  
- CatBoost  
- LightGBM  
- Random Forest  
- Decision Tree  
- KNN (baseline)  

## RESULTS

### Before Tuning  
- KNN: 70.3%  
- Logistic Regression: 84.4%  
- Gradient Boosting: 84.4%  
- CatBoost: 84.1%  

### Final Model (CatBoost)  
- Accuracy: **84.7%**  
- F1-score: **0.87**  
- Recall: **88.5%**  

## Key Insights  
- Study consistency and concept understanding are strongest predictors  
- Moderate AI usage improves performance; high dependency reduces it  
- Lifestyle factors like sleep and social media affect outcomes  
- High-performing students are easier to predict  

## PROJECT STRUCTURE

```text
.
├── README.md
├── Student Performance Classification.ipynb
└── dataset.csv
```
