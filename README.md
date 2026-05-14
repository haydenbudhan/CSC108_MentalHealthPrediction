# CSC108_MentalHealthPrediction
A data science project analyzing mental health risk using lifestyle, stress, and psychological factors. Includes exploratory data analysis, visualization, and machine learning models (Logistic Regression, Decision Tree, Random Forest) to evaluate how well mental health risk can be predicted.

# Mental Health Risk Prediction
## Overview
This project explores whether mental health risk can be predicted using lifestyle, stress, and psychological factors. Using a dataset of 25,000 individuals, the project identifies key patterns and evaluates how well mental health risk can be modeled using multiple machine learning approaches.

> **This project is open to be shared with future classes!**

## Dataset
The dataset (`mental_health_risk_dataset.csv`) contains **25,000 entries** and **25 features** related to:
- Lifestyle (e.g., sleep hours, screen time, physical activity)
- Stress (e.g., work stress, financial stress)
- Psychological factors (e.g., anxiety score, depression score)

**Target Variable:** `mental_health_risk`
- 0 = Low Risk
- 1 = Medium Risk
- 2 = High Risk

## Exploratory Data Analysis
Several visualizations were created to understand relationships between variables:
- Boxplots comparing features against mental health risk
- Correlation heatmap to identify strong relationships

### Key Findings:
- Sleep has a negative relationship with mental health risk
- Anxiety and depression have strong positive relationships with risk
- Screen time showed little to no meaningful relationship

## Models
Three machine learning models were built and compared to predict mental health risk.

### Features Used (all models):
- Sleep hours
- Anxiety score
- Depression score
- Work stress level
- Financial stress level
- Social support score

### Approach:
- Data split into 80% training and 20% testing
- Each model trained on selected features
- Predictions evaluated using accuracy and confusion matrix

### Models Compared:
| Model | Accuracy |
|---|---|
| Logistic Regression | ~61% |
| Decision Tree | ~61% |
| Random Forest | ~67% |

Random Forest achieved the highest accuracy, suggesting that more complex models better capture the relationships in the data.

## Results
- **Best Model:** Random Forest (~67% accuracy)
- Logistic Regression and Decision Tree each achieved ~61% accuracy
- All models perform best when predicting medium risk (class 1)
- All models struggle to distinguish between low and high risk levels, frequently misclassifying them as medium risk

## Feature Importance
Based on logistic regression coefficients:

| Feature | Direction |
|---|---|
| Sleep hours | Positive (associated with lower risk) |
| Social support score | Positive (associated with lower risk) |
| Anxiety score | Negative (associated with higher risk) |
| Depression score | Negative (associated with higher risk) |
| Work stress level | Negative (moderate impact) |
| Financial stress level | Negative (moderate impact) |

Anxiety and depression were the strongest predictors of higher mental health risk, while sleep hours had the largest positive contribution toward lower risk.

## Conclusion
Mental health risk can be partially predicted using lifestyle and psychological data. Anxiety, depression, and sleep are the most influential variables. The moderate accuracy across all models highlights the complexity of mental health and suggests that important factors — such as personal experiences, biological influences, and environment — are not fully captured in the dataset.

## Technologies Used
- Python
- Pandas
- Matplotlib / Seaborn
- Scikit-learn

## Future Improvements
- Tune hyperparameters for the Random Forest model to further improve accuracy
- Include more comprehensive datasets with additional variables
- Improve feature selection and experiment with additional model types

---
## Author
Hayden Budhan

GitHub: https://github.com/haydenbudhan/CSC108_MentalHealthPrediction
LinkedIn: https://www.linkedin.com/in/haydenbudhan1101/
