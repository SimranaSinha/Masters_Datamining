# Predicting Diabetes Risk Using Health Indicators

This project applies machine learning to predict diabetes risk based on health, lifestyle, and demographic indicators. The goal is to classify individuals into three categories:
	•	Non-Diabetic
	•	Pre-Diabetic
	•	Diabetic

By building data-driven predictive models, this project supports early detection and helps healthcare professionals prioritize preventive care and timely intervention.  ￼

⸻

📊 Dataset
	•	Source: CDC Diabetes Health Indicators (UCI Repository)
	•	Records: ~253,000
	•	Features: 21 health and demographic attributes
	•	Target: Diabetes status encoded as 0, 1, or 2

Key predictors include:
	•	BMI
	•	Blood pressure
	•	General health rating
	•	Physical activity
	•	Age
	•	Income and education

⸻

🔍 Project Workflow

1️⃣ Exploratory Data Analysis

We examined:
	•	Feature distributions
	•	Class balance
	•	Correlations with diabetes risk
	•	Outliers and skewed variables

Several low-variability features were removed to reduce noise.

⸻

2️⃣ Feature Engineering & Preprocessing

Steps included:
	•	Encoding categorical features
	•	Handling imbalance
	•	Removing redundant or non-informative features
	•	Splitting data into training and test sets

⸻

3️⃣ Model Development

Three machine learning models were evaluated:
	•	Logistic Regression
	•	Random Forest
	•	XGBoost

Models were compared using:
	•	Accuracy
	•	Precision
	•	Recall
	•	F1-Score
	•	Confusion matrices
	•	ROC-AUC curves

Hyperparameter tuning was performed using GridSearchCV.

⸻

🏆 Model Selection

XGBoost achieved the best overall balance between performance and generalization, delivering strong accuracy while minimizing overfitting compared to Random Forest. It also performed best when identifying diabetic cases.

However, the dataset is imbalanced, and identifying pre-diabetic cases remains challenging, suggesting future improvement opportunities such as:

✔ class weighting
✔ oversampling
✔ alternate loss functions

⸻

📈 Results Snapshot

Model	Train Accuracy	Test Accuracy	Notes
Logistic Regression	~83%	~83%	Simple but limited
Random Forest	~99%	~82%	Overfitting observed
XGBoost	~85%	~83%	Best overall performer

Top predictors included:
	•	BMI
	•	Age
	•	General health
	•	Physical health
	•	Income

⸻

🧠 Key Insights

✔ Higher BMI strongly correlates with diabetes risk
✔ Poor general health increases risk
✔ Age remains an important non-modifiable factor
✔ Socioeconomic variables influence outcomes
✔ Walking difficulty signals potential complications

⸻

🚀 Impact & Applications

This work demonstrates how machine learning can:
	•	Support early diabetes screening
	•	Guide preventive care
	•	Reduce healthcare burden
	•	Enable scalable risk stratification

It has potential use in:

- 🏥 clinical settings
- 📱 health monitoring tools
- 📊 policy and population health analytics

