# 🩺 Diabetes Prediction: Machine Learning Classification

## 📝 Project Overview
This project is focused on predicting the presence of diabetes in patients using Machine Learning classification models. The dataset used is the "Basic of Kaggle Diabetes" dataset. The goal of this project is to build a robust model that can accurately classify whether a patient is positive or negative for diabetes based on various medical predictor variables.

## 🛠️ Tools & Technologies
* **Language:** Python 3
* **Data Manipulation:** Pandas, NumPy
* **Data Visualization:** Matplotlib, Seaborn
* **Machine Learning:** Scikit-Learn (Logistic Regression, Random Forest Classifier)

## 🚀 Workflow & Key Steps

### 1. Exploratory Data Analysis (EDA)
* Checked for missing values (`null` counts) in both training and testing datasets.
* Visualized the target variable (`class`) distribution using Matplotlib bar charts to understand the balance between Positive and Negative cases.

### 2. Data Preprocessing
* **Label Encoding:** Converted categorical text data into numerical format using `LabelEncoder`.
* **Feature Scaling:** Applied **Min-Max Normalization** to the `age` column to bring the values between 0 and 1, ensuring better model performance.
* **Feature Selection:** Analyzed correlations and dropped features with little to no predictive value, such as `ID` and `gender`, to prevent noise in the model.

### 3. Machine Learning Models
The dataset was split into an 80/20 train-test ratio (`test_size=0.2`). Two classification models were trained and evaluated:
1. **Logistic Regression:** Used as a baseline linear classification model.
2. **Random Forest Classifier:** Used as a complex ensemble method (`n_estimators=100`) to capture non-linear relationships.

## 🏆 Results
* The **Random Forest Classifier** achieved an outstanding accuracy of **98.63%** on the test data.
* A final submission CSV file was generated to predict the test set.

## 📂 Project Structure
* `train.csv`: Training dataset containing patient features and target classes.
* `test.csv`: Testing dataset used for final model predictions.
* `sample_submission.csv`: Template for the Kaggle submission format.
* `main.py` / `notebook.ipynb`: The main Python script containing EDA, preprocessing, and model training.

---
*Created by [Ismingiz] - Data Analyst & Python Developer*
