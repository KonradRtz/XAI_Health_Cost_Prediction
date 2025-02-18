# XAI_Health_Cost_Prediction

## Project Overview
This project explores different regression methods for predicting health costs using a Kaggle dataset. Initially, data preprocessing was performed using EPA analysis and by creating Label Encoded (LE) and One-Hot Encoded (OHE) datasets. A baseline Linear Regression (LR) model was trained, followed by more advanced models including Random Forest (RF), XGBoost (XGB), LightGBM, CatBoost, Support Vector Regression (SVR), and an Artificial Neural Network (ANN).

## Model Outcomes
- **XGBoost:** Achieved the best performance.
- **Tree-based methods (RF, LightGBM, CatBoost):** Slightly behind XGBoost.
- **ANN:** Performed at a mid-level and requires significant fine tuning and extended training time.
- **SVR:** Also produced mid-range performance.

## Explainable AI Analysis
To understand the model decisions, Partial Dependence Plots (PDP) and SHAP values were computed for the best XGBoost model. The insights highlighted that the diabetes feature was highly skewed: instead of the expected ~11% prevalence, around 80% of the data had diabetes. Attempts to fix this via bootstrapping further limited the number of data points, resulting in worsened model performance and no significant change in the model reasoning.

## Conclusion
Overall, the Kaggle dataset used in this project is extremely problematic, leading to unreliable outcomes. This emphasizes the need for better data quality and increased collaboration between insurance companies and scientists to mitigate biases and improve predictive reliability.
