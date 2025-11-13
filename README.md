
Credit Card Fraud Detection

An end-to-end machine learning project to detect fraudulent credit-card transactions using supervised learning techniques. This project includes data preprocessing, EDA, handling class imbalance, model training, evaluation, and prediction.

📌 Overview

Credit-card fraud is a major financial threat, and early detection is crucial. This project builds a machine-learning pipeline that classifies transactions as fraud or non-fraud using statistical features and ML algorithms.

The project is built completely inside a Jupyter/IPython notebook (credit_card_fraud_sony.ipynb).

🚀 Features

✔ Data loading & cleaning
✔ Exploratory Data Analysis (EDA)
✔ Class-imbalance handling (SMOTE / class weights)
✔ Feature scaling
✔ Model building (Logistic Regression, Random Forest, XGBoost, etc.)
✔ Performance evaluation (ROC-AUC, PR-AUC, confusion matrix)
✔ Fraud probability prediction
✔ Exporting trained models

📂 Project Structure
.
├── credit_card_fraud_sony.ipynb     # Main ML notebook
├── data/                            # Dataset folder (not included in repo)
├── models/                          # Saved model files (joblib/pickle)
├── README.md                        # Project documentation
└── requirements.txt                 # Dependencies

📊 Dataset

Source: Commonly from Kaggle: Credit Card Fraud Detection Dataset

Samples: ~284,807 transactions

Fraud cases: ~492 (highly imbalanced)

Columns:

V1–V28 – PCA-transformed features

Amount – transaction amount

Time – seconds from first transaction

Class – 1 = Fraud, 0 = Genuine

⚠️ Raw dataset is NOT included due to size & privacy. Add it manually inside /data.

🔧 Tech Used

Python 3.x

Scikit-Learn

Pandas / NumPy

Matplotlib / Seaborn

Imbalanced-Learn (SMOTE)

Joblib (for saving models)

🧠 Machine Learning Pipeline
1️⃣ Data Preprocessing

Remove duplicates

Scale numerical features (StandardScaler)

Handle class imbalance using:

SMOTE, or

class_weight='balanced'`

2️⃣ Exploratory Data Analysis

Class distribution visualization

Correlation heatmap

Amount & Time distribution

3️⃣ Model Training

Algorithms used typically include:

Logistic Regression

Random Forest

XGBoost / LightGBM

SVM / KNN (optional)

4️⃣ Evaluation Metrics

Imbalanced classification requires special metrics:

ROC-AUC

PR-AUC

F1-Score

Recall (important for fraud detection)

Confusion Matrix

Precision@K
