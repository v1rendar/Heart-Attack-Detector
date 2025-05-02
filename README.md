❤️ Heart Attack Predictor 🩺

Predicting risk before it strikes – powered by Python, data science, and a little healthcare magic.

📌 Project Overview
This project predicts whether a patient is at risk of a heart attack using machine learning. We crunched real medical data, trained multiple models, and now we can help flag high-risk cases before it’s too late.

📂 Dataset
File: Medicaldataset.csv

Features:

Age

Gender (1 = Male, 0 = Female)

Heart rate

Systolic blood pressure

Diastolic blood pressure

Blood sugar

CK-MB

Troponin

Result (positive = Heart Attack, negative = No Heart Attack)

Source: Provided medical dataset

🛠️ Tech Stack
Python 🐍

Pandas & NumPy 📊

Scikit-learn 🤖

Matplotlib & Seaborn 📈

Jupyter Notebook 📓

🚦 How It Works
Data Cleaning & Preprocessing

Handle missing values

Encode categorical variables

Feature scaling for ML models

Exploratory Data Analysis (EDA)

Visualize feature distributions

Correlation analysis

Spot trends in heart attack risk

Model Training & Selection

Tried out Logistic Regression, Random Forest, and more

Compared models using accuracy, precision, recall, and F1-score

Random Forest gave the best results!

Prediction

Predict risk for new patients

Evaluate with confusion matrix and classification report

📁 How to Use
Clone the repo:

bash
git clone https://github.com/yourusername/heart-attack-predictor.git
cd heart-attack-predictor
Install requirements:

bash
pip install -r requirements.txt
Run the notebook:

bash
jupyter notebook Heart_Attack_Predictor.ipynb
Upload your dataset:

Place Medicaldataset.csv in the project directory or upload in Colab

📊 Results
Model	Accuracy
Logistic Regression	83%
Random Forest	87%
Top predictors: Age, Heart Rate, CK-MB, Troponin

Random Forest had the best performance!

🩺 Sample Prediction
python
# Example: Predict for a new patient (edit values as needed)
sample = np.array([[55, 1, 80, 120, 80, 110, 2.5, 0.01]])
sample_scaled = scaler.transform(sample)
prediction = model.predict(sample_scaled)
print("Prediction (1: Heart Attack, 0: No Heart Attack):", prediction[0])
🚀 Future Work
 Add more ML models (SVM, XGBoost, Neural Nets)

 Build a web app for instant predictions

 Deploy as a cloud API

🙏 Credits
Medicaldataset.csv (provided)

Thanks to the open-source Python ML community!

License: MIT
