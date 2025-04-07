# Microsoft
Classifying Cybersecurity Incidents with Machine Learning
🔐 Triage Grade Prediction for Cybersecurity Incidents
🧠 Project Overview
This project aims to develop a robust machine learning classification model that predicts the triage grade of cybersecurity incidents — True Positive (TP), Benign Positive (BP), or False Positive (FP) — using the comprehensive GUIDE dataset provided by Microsoft. The goal is to support Security Operation Centers (SOCs) by automating incident triage and enabling faster, more accurate decision-making.

🚀 Problem Statement
Imagine you're working as a data scientist at Microsoft to enhance SOC efficiency. You're tasked with building a machine learning model that classifies security incidents based on historical evidence and customer responses.

You will train the model using the provided train.csv dataset and evaluate its performance on test.csv using:

Macro F1-score

Precision

Recall

🧩 Business Use Cases
Security Operation Centers (SOCs): Improve analyst productivity by automating triage grading.

Incident Response Automation: Guide systems to take timely, appropriate actions.

Threat Intelligence: Detect and classify threats accurately by learning from historical patterns.

Enterprise Security Management: Enhance organizational security posture by minimizing false positives and prioritizing real threats.

📊 Dataset Overview
The GUIDE dataset has a 3-level structure:

Evidence → smallest unit (e.g., IP, user, email)

Alert → group of evidences

Incident → group of alerts

Each incident is labeled as TP, BP, or FP, and comes with 45 features. The data is already split into:

Train (70%)

Test (30%) Stratified by triage grade, OrgID, and DetectorID to maintain consistency in incident grouping.

🧱 Project Structure

🧪 Approach
🔍 1. Data Exploration & Preprocessing
Initial inspection of structure and types

Visualizations and class distribution check

Handling missing values

Feature engineering (e.g., timestamp features)

Encoding categorical variables

🔀 2. Data Splitting
Train-validation split (80/20 with stratification)

🤖 3. Model Training
Baseline model (e.g., Logistic Regression)

Advanced models (Random Forest, XGBoost, LightGBM)

Cross-validation for reliable performance estimation

Class imbalance handling (e.g., SMOTE, class weights)

📈 4. Evaluation
Metrics: Macro F1-score, precision, recall

Error analysis and feature importance using SHAP

Comparison with baseline

✅ 5. Final Testing
Evaluate final model on test.csv

Record metrics for real-world applicability

📌 Results
A predictive model that accurately classifies triage grades (TP, BP, FP)

Balanced performance across all classes using macro-F1, precision, and recall

Clear documentation of important features and data-driven decision insights

📊 Evaluation Metrics
Metric	Description
Macro-F1	Balance of precision and recall across all classes
Precision	Accuracy of positive predictions
Recall	Ability to detect all true cases
🛠 Tech Stack
Python (Pandas, NumPy, Scikit-learn, XGBoost, LightGBM)

Jupyter Notebook

SHAP (Model Interpretability)

Matplotlib, Seaborn (Visualization)

🔖 Tags
Machine Learning Cybersecurity Classification SOC Threat Detection Model Evaluation Data Science Feature Engineering

