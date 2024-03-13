**Overview**
This repository contains code and documentation for building a lead conversion model for X Education, an online education company. The model is developed using logistic regression to predict the likelihood of lead conversion based on various features such as lead source, lead origin, last activity, and more. The goal is to assist X Education in identifying high-potential leads and improving their lead conversion rate.

**Approach**
1. Data Pre-processing
Read and comprehend data structure.
Clean data by handling anomalies, correcting column names, and imputing null values using appropriate techniques.
Handle outliers using the IQR technique.

**2. Data Visualization**
Perform univariate and bivariate analysis to understand data distributions, identify important features, and visualize relationships between features and lead conversion.
3. Feature Scaling
Convert categorical columns to numerical format using binary mapping and one-hot encoding.
Rescale numerical columns using the Standard Scaler approach.

**4. Model Building**
Utilize Recursive Feature Elimination (RFE) to select significant features for model training.
Ensure model stability by checking Variance Inflation Factor (VIF) and p-values.
Train logistic regression model and optimize performance using appropriate threshold values.

**5. Model Evaluation**
Evaluate model performance on train set using accuracy, sensitivity, specificity, and other metrics.
Determine optimal cut off for predictions based on precision-recall trade-off.
Forecast lead conversion probabilities on test dataset.

**Results**

**Train Data Metrics**
Accuracy: 93%
Sensitivity: 89%
Specificity: 96%

**Test Data Metrics**
Accuracy: 92%
Sensitivity: 88%
Specificity: 93%

**Recommendations**
Based on model insights and analysis:
Prioritize leads with specific tags like "Closed by Horizon" and "Will revert after reading the email" for higher conversion chances.
Focus on leads originating from Landing Page Submissions and Lead Add Forms for potential conversions.
Improve lead conversion rates for certain lead sources such as Olark Chat and organic search.
Enhance last activity engagement, particularly through SMS Sent, for better conversion rates.
