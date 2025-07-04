# 🔄 User Churn Prediction System

A machine learning pipeline for predicting user churn based on subscription, usage, and engagement data. This project involves complete EDA, feature engineering, model building, evaluation.

---

## 📌 Project Overview

Churn prediction is critical for businesses to proactively retain users. This project leverages user behavior, engagement, and subscription metadata to predict churn using classification models. The best-performing model is then deployed for real-time inference.

---

## 📊 Features

- 📁 EDA: Manual and visual exploration of user demographics, behavior, and subscription trends.
- ⚙️ Feature Engineering: Encoding, derived features (Age, Duration), balancing, and selection.
- 🧠 Model Building:
  - Baseline models: Logistic Regression, KNN, Naive Bayes, Decision Tree, SVM
  - Advanced models: Random Forest, XGBoost, LightGBM, CatBoost
  - Evaluation via Accuracy, Precision, Recall, F1 Score, ROC AUC, Confusion Matrix, ROC Curve
- 🔍 Hyperparameter Tuning: Grid/RandomizedSearchCV on top models
- 🏆 Final model: LightGBM (best F1 Score)
- 📦 Exported model: `lightgbm_churn_model.pkl`

---

## 🛠️ Tech Stack

| Category       | Tools / Libraries              |
|----------------|-------------------------------|
| Language       | Python                         |
| EDA            | Pandas, Seaborn, Matplotlib    |
| ML Models      | Scikit-learn, XGBoost, LightGBM, CatBoost |
| Evaluation     | Scikit-learn metrics           |
| Tuning         | GridSearchCV, RandomizedSearchCV |
| Serialization  | Joblib                         |

---

## 📁 Folder Structure

📂 Amazon_Prime_Users/
│
├── 📊 data/
│ └── amazon_prime_users.csv
  └──  Amazon_Prime_Users_updated_dataset
│
├── 📦 models/
│ └── lightgbm_churn_model.pkl
│
├── 📈 notebooks/
│ └── EDA_and_Modeling.ipynb
├── requirements.txt
└── README.md

---

## 🚀 Running the Project

### 1️⃣ Clone the repo
git clone https://github.com/yourusername/Amazon_users_Churn-Prediction.git
cd churn-prediction


## 📊 Final Model Performance
![image](https://github.com/user-attachments/assets/37e4ea39-2902-4bdb-a038-d2538a4a76d4)

## 📌 Future Improvements
Handle class imbalance using SMOTE or focal loss

Add SHAP/ELI5 model explainability

Time-series modeling of user behavior

Batch prediction via CSV uploads in Streamlit

Dockerize for production deployment

## 🙋‍♂️ Author
Chinmay Deshpande

## 📄 License
This project is licensed under the MIT License.
