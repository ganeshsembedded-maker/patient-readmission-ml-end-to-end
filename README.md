# 🤖 Patient Readmission Prediction  
### End-to-End Machine Learning Project

## 📌 Overview
This project demonstrates a **complete end-to-end Machine Learning workflow** using Python.  
The objective is to predict **patient readmission** using structured healthcare data by applying data preprocessing, feature encoding, model training, and evaluation techniques.

The project follows **real-world ML pipeline practices** commonly used in industry-level applications.

---

## 🛠️ Technologies Used
- **Python**
- **NumPy**
- **Pandas**
- **Matplotlib**
- **Seaborn**
- **scikit-learn**
- **XGBoost**

---

## 📊 Dataset
- **Training Dataset:** 66,587 records × 49 features  
- **Test Dataset:** 48 features  
- **Target Variable:** `readmitted` (Binary Classification)

The dataset includes:
- Patient demographic information  
- Hospital stay details  
- Lab procedures and medication data  
- Diagnostic and treatment indicators  

---

## 🔄 Machine Learning Workflow

### 1️⃣ Data Loading & Exploration
- Loaded training and test datasets using Pandas  
- Inspected dataset structure, data types, and missing values  
- Verified dataset size and feature distributions  

---

### 2️⃣ Exploratory Data Analysis (EDA)
Performed visual analysis to understand the impact of features on patient readmission:
- **Time in hospital vs readmission**
- **Number of medications vs readmission**
- **Lab procedures and age impact**

📊 Visualizations created using **Seaborn** and **Matplotlib**.

---

### 3️⃣ Data Preprocessing
- Removed unnecessary and highly missing columns  
- Identified **36 categorical features**  
- Applied **Label Encoding** consistently to both training and test datasets  
- Prevented data leakage by fitting encoders on combined data  

---

### 4️⃣ Feature Engineering
- Separated features (`X`) and target (`y`)  
- Performed **80:20 train–validation split**  
- Used **stratified sampling** to handle class imbalance  

---

### 5️⃣ Model Training
Trained and evaluated multiple classification models:

#### 🔹 Logistic Regression
- Used as a baseline model  
- Increased max iterations to ensure convergence  

#### 🔹 Random Forest Classifier
- 300 estimators  
- Balanced class weights  
- Strong performance on non-linear patterns  

#### 🔹 XGBoost Classifier
- Gradient-boosted decision trees  
- Tuned hyperparameters for better generalization  

---

## 📈 Model Performance (F1 Score)

| Model               | F1 Score (%) |
|--------------------|-------------|
| Logistic Regression | 42.74 |
| Random Forest       | **76.50** |
| XGBoost             | 71.87 |

✅ **Random Forest achieved the best performance**

---

## 🧮 Confusion Matrix
- Evaluated predictions using a **confusion matrix**  
- Visualized results with a heatmap  
- Analyzed false positives and false negatives  

---

## 📌 Key Learnings
- Importance of **proper categorical encoding**
- Handling **class imbalance** effectively
- Strength of **tree-based ensemble models**
- End-to-end ML pipeline implementation
- Using **F1-score** instead of accuracy for imbalanced data  

---

## 🚀 Future Improvements
- Hyperparameter tuning using GridSearch / RandomSearch  
- Feature selection techniques  
- Advanced imbalance handling (SMOTE, class weighting)  
- Model deployment using **Flask / FastAPI**  
- Cloud deployment using **AWS**  

---

## ▶️ Open in Google Colab
This project can be executed directly in **Google Colab** for easy experimentation.

---

## 📂 Repository Link
🔗 https://github.com/ganeshsembedded-maker/ml-end-to-end-project

---

⭐ If you find this project useful, feel free to **star ⭐ the repository**!
