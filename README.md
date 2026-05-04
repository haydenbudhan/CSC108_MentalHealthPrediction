# CSC108_MentalHealthPrediction
A data science project analyzing mental health risk using lifestyle, stress, and psychological factors. Includes exploratory data analysis, visualization, and a logistic regression model to evaluate how well mental health risk can be predicted.

# Mental Health Risk Prediction

## Overview
This project explores whether mental health risk can be predicted using lifestyle, stress, and psychological factors. Using data analysis and machine learning techniques, the project identifies key patterns and evaluates how well mental health risk can be modeled.

---

## Dataset
The dataset includes variables related to:
- Lifestyle (e.g., sleep hours, screen time, physical activity)
- Stress (e.g., work stress, financial stress)
- Psychological factors (e.g., anxiety score, depression score)

**Target Variable:**
- `mental_health_risk`
  - 0 = Low Risk  
  - 1 = Medium Risk  
  - 2 = High Risk  

---

##  Exploratory Data Analysis
Several visualizations were created to understand relationships between variables:
- Boxplots comparing features against mental health risk
- Correlation heatmap to identify strong relationships

### Key Findings:
- Sleep has a negative relationship with mental health risk  
- Anxiety and depression have strong positive relationships with risk  
- Screen time showed little to no meaningful relationship  

---

## Model
A **Logistic Regression** model was used to predict mental health risk.

### Features Used:
- Sleep hours  
- Anxiety score  
- Depression score  
- Work stress level  
- Financial stress level  
- Social support score  

### Approach:
- Data split into 80% training and 20% testing  
- Model trained on selected features  
- Predictions evaluated using accuracy and confusion matrix  

---

## Results
- **Model Accuracy:** ~61%  
- The model performs best when predicting medium risk  
- It struggles to distinguish between low and high risk levels  

---

## Feature Importance
The most influential variables in predicting mental health risk were:
- Sleep hours  
- Anxiety score  
- Depression score  

Stress-related variables had moderate impact, while screen time had little influence.

---

## Conclusion
Mental health risk can be partially predicted using lifestyle and psychological data. However, the moderate accuracy highlights the complexity of mental health and suggests that important factors (such as personal experiences, biological influences, and environment) are not fully captured in the dataset.

---

## Technologies Used
- Python  
- Pandas  
- Matplotlib / Seaborn  
- Scikit-learn  

---

## Future Improvements
- Test additional models (e.g., decision trees, random forests)  
- Include more comprehensive datasets with additional variables  
- Improve feature selection and model tuning  

---

## Author
Hayden Budhan
