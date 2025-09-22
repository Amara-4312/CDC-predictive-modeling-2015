# CDC-predictive-modeling-2015
Chronic Disease Prediction using Machine Learning – A pipeline project exploring data cleaning, feature engineering, and modeling (Logistic Regression, Random Forest, and Balanced Classifiers) with imbalanced health survey data.

 Project Overview
 Goal: Explore the relationship between past behaviors (sleep, stress, lifestyle factors) and the risk
 of chronic diseases (hypertension, diabetes). Why it matters: Chronic diseases are on the rise in
 Nigeria, but predictive models can help with preventive care. Challenge: Dataset was highly
 imbalanced, making prediction of positive cases difficult. Approach: Data cleaning → feature
 engineering → multiple ML models → addressing class imbalance.
 
 Dataset Description
 Source: CDC. Size: ~ X samples, Y features (replace
 with actual numbers). Features considered: lifestyle (sleep, stress, diet, activity, etc.),
 demographics, and health indicators. Target: Chronic disease presence (binary classification: 0 =
 no disease, 1 = disease).
 
 Methodology
 The project was broken down into three notebooks: 
 1. Data Cleaning Notebook: handled missing
 values, encoded categorical variables, normalized continuous variables.
 2. Feature Engineering
 Notebook: created derived features, applied feature selection.
 3. Weighted EDA vs Unweighted EDA:
 4. Modeling Notebook: tested
 Logistic Regression, Random Forest, applied SMOTE, tuned thresholds, and evaluated ROC-AUC.
 Results- Class Imbalance Issue: Models biased toward predicting "no disease". - Baseline Logistic
 Regression: High accuracy, poor recall for positive class. - Random Forest: Improved but still
 struggled with minority class. - Threshold tuning: Improved recall (up to ~83%) at the cost of
 precision.

Overall insight: With imbalanced health datasets, accuracy is misleading recall and ROC-AUC matter more.
 
 Key Takeaways- 
Dataset imbalance is a critical barrier in health prediction. 
Recall is more important than accuracy for disease detection.  
Oversampling (SMOTE) helps, but still not perfect.
Future work: uselarger/balanced datasets (e.g., CDC balanced risk dataset) for stronger generalization.

 Future Directions
- Test with larger datasets (CDC/Kaggle).
- Explore ensemble methods (XGBoost, LightGBM).
- Consider explainability (SHAP, LIME) for healthcare adoption.
- Deploy as a web app for public health researchers

 
