# Sleep Disorder Prediction

## 📌 Project Description
This project aims to predict sleep disorders (Insomnia, Sleep Apnea, or Healthy) using machine learning models based on lifestyle and health-related features. It utilizes the "Sleep Health and Lifestyle" dataset from Kaggle with features like age, gender, sleep duration, stress level, and more.

## 📊 Dataset
- **Source:** [Kaggle Dataset](https://www.kaggle.com/datasets/uom190346a/sleep-health-and-lifestyle-dataset)
- **Rows:** 3000 (after balancing)
- **Columns:** 13 (includes features like Sleep Duration, BMI Category, Stress Level, etc.)
- **Target Variable:** Sleep Disorder (Insomnia, Sleep Apnea, Healthy)

## 🛠️ Tools Used
- **Language:** Python
- **Libraries:** pandas, scikit-learn, joblib

## ⚙️ Methodology
1. Data Preprocessing
   - Handled missing/null values
   - Label encoding of categorical features
   - Standardization of numerical features
2. Model Building
   - Train-test splits: 70:30, 75:25, 80:20
   - Models used:
     - Logistic Regression
     - K-Nearest Neighbors (KNN)
     - Decision Tree
     - Support Vector Machine (SVM)
     - Random Forest
3. Evaluation Metrics
   - Accuracy
   - Precision
   - Recall
   - F1-Score

## 🧠 Algorithm Used
Multiple algorithms were evaluated, including Logistic Regression, KNN, Decision Tree, SVM, and Random Forest. Among them, **Random Forest** consistently achieved the highest accuracy across various train-test splits and was selected as the final model.

## ✅ Final Model
- **Algorithm:** Random Forest Classifier
- **Train-Test Split:** 80:20
- **Accuracy:** ~93.33%
- **Model File:** `sleep_disorder_model.pkl`
- **Scaler File:** `scaler.pkl`
- **Encoders:** `label_encoders.pkl`

## 🔍 Sample Prediction
The final model can predict sleep disorder types (Insomnia, Sleep Apnea, Healthy) using user input on health and lifestyle attributes.
