# 🩺 Symptom to Disease Prediction System

[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)
[![Pandas](https://img.shields.io/badge/Pandas-150458?style=for-the-badge&logo=pandas&logoColor=white)](https://pandas.pydata.org/)
[![NumPy](https://img.shields.io/badge/NumPy-013243?style=for-the-badge&logo=numpy&logoColor=white)](https://numpy.org/)
[![Scikit-Learn](https://img.shields.io/badge/Scikit--Learn-F7931E?style=for-the-badge&logo=scikitlearn&logoColor=white)](https://scikit-learn.org/)
[![NLTK](https://img.shields.io/badge/NLTK-76B900?style=for-the-badge)](https://www.nltk.org/)
[![XGBoost](https://img.shields.io/badge/XGBoost-AA0000?style=for-the-badge)](https://xgboost.ai/)
[![Jupyter](https://img.shields.io/badge/Jupyter-FA0F00?style=for-the-badge&logo=jupyter&logoColor=white)](https://jupyter.org/)

> A Natural Language Processing (NLP) based Machine Learning system that predicts diseases from user-provided symptoms.

---

## ✨ Description

The **Symptom to Disease Prediction System** uses NLP and Machine Learning to analyze textual symptom input and predict the most likely disease.

This project demonstrates:
- 🧠 NLP preprocessing  
- 🔍 Text vectorization using TF-IDF  
- 🤖 Classification using ML models  

---

## 🚀 Features

- 📝 **Text-based symptom input**
- 🧹 **Text preprocessing (stemming + stopword removal)**
- 🔠 **TF-IDF vectorization**
- 🤖 **Machine Learning classification**
- 📊 **Model evaluation (accuracy, confusion matrix)**
- ⚡ **Real-time disease prediction**

---

## 🛠️ Tech Stack

### 👨‍💻 Core
- **Python**

### 📊 Data Processing
- **Pandas**
- **NumPy**

### 🧠 NLP
- **NLTK**
  - Stopwords
  - Porter Stemmer  

### 📈 Visualization
- **Matplotlib**
- **Seaborn**

### 🤖 Machine Learning
- **Scikit-learn**
  - Logistic Regression  
  - TF-IDF Vectorizer  

- **XGBoost** *(optional / imported)*

---

## 📂 Dataset

- 📌 Symptom2Disease Dataset  
- Format: CSV  
- Columns:
  - `text` → Symptoms (text)
  - `label` → Disease  

🎯 Target:
- Predict disease from symptoms

---

## 🔄 Workflow

### 1️⃣ Data Preprocessing
- Remove unwanted columns  
- Handle missing values  
- Convert labels to numerical format  

---

### 2️⃣ NLP Processing
- Remove special characters  
- Convert to lowercase  
- Remove stopwords  
- Apply **Porter Stemming**  

---

### 3️⃣ Feature Engineering
- Convert text → numerical using **TF-IDF Vectorizer**

---

### 4️⃣ Model Training

- 📌 Logistic Regression (Primary Model)

---

### 5️⃣ Model Evaluation

- ✅ Accuracy Score  


---

## 📊 Results

- High training accuracy  
- Good generalization on test data  
- Efficient for real-time symptom prediction  

---

## 🧪 Example Usage

```bash
Enter your symptoms:
fever headache body pain fatigue
