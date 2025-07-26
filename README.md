# ml-project-premium-prediction
# Try Web APP

(click here see web app)[https://insurancepricepredictionbyzaidnaeem.streamlit.app/]

!(screenshot)[gitimg.png]
Built a regression-based AI system that predicts the insurance premium a customer may be charged — based on their demographics, medical history, lifestyle, and regional information.
This model supports insurance companies in offering fair and data-driven pricing.

📊 Features Used:

Categorical Inputs:

Gender, Marital Status, Employment Status

BMI Category, Smoking Status, Medical History

Region, Insurance Plan

Numerical Inputs:

Age

Number of Dependents

Genetical Risk Score

⚠️ Key Insight from Data Analysis:
During deep EDA, I uncovered a major issue:
👉 Customers under the age of 25 displayed high variance and unpredictable pricing patterns — significantly impacting model performance and interpretability.

💡 Solution:
To address this challenge, I:
🔹 Split the dataset based on age into two distinct groups:
 📍 Customers aged < 25
 📍 Customers aged ≥ 25
🔹 Built separate regression models for each group
🔹 Tailored preprocessing for younger individuals to account for anomalies in lifestyle and employment data
🔹 Combined predictions using smart model-switching logic based on input age

📌 Model Highlights:

✅ Age-based dual-model architecture

✅ Feature encoding (Label & One-Hot)

✅ Outlier treatment in BMI & Genetical Risk

✅ Regression models: Linear Regression vs Random Forest Regressor

✅ Evaluation metrics: MAE, RMSE, R² Score

🎯 Model Accuracy:
🔹 Achieved an impressive 99.2% R² Score on the validation set — indicating excellent prediction performance.

🔍 Techniques Applied:
✅ Exploratory Data Analysis (EDA)
✅ Regression Modeling
✅ Data Segmentation by Demographics
✅ Feature Engineering for Lifestyle Risk
✅ Model Evaluation and Comparison
✅ Visualization of Prediction Trends

🛠️ Tech Stack:
Machine Learning | Python | pandas | scikit-learn | matplotlib | seaborn

🌐 Use Case Impact:
Perfect for health insurance providers, this app intelligently adjusts premium predictions based on both medical risk and customer demographics — ensuring personalized and fair pricing strategies.


