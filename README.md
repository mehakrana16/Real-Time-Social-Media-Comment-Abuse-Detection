# 📌 Real-Time Social Media Comment Abuse Detection 🚀

## 📖 Overview
This project focuses on detecting abusive or toxic comments on social media platforms using **Natural Language Processing (NLP)** and **Machine Learning**.

The model classifies user comments into:
- ✅ Non-Toxic  
- ❌ Toxic  

It helps in:
- Content moderation  
- Improving online community safety  
- Reducing harmful interactions  

---

## 🧠 Project Objective
- Automatically detect abusive or toxic comments  
- Build a lightweight and efficient ML model  
- Enable real-time prediction for new comments  

---

## 📂 Dataset
- Dataset used: `train.csv` (compressed in zip file)  

### Features:
- `comment_text` → User comment  
- `toxic` → Label (1 = Toxic, 0 = Non-Toxic)  

---

## ⚙️ Technologies Used
- Python  
- Pandas & NumPy → Data handling  
- Scikit-learn → ML model & preprocessing  
- TF-IDF Vectorizer → Text feature extraction  
- Logistic Regression → Classification model  
- Regex & String Processing → Text cleaning  

---

## 🔄 Workflow

### 1️⃣ Data Preprocessing
- Convert text to lowercase  
- Remove:
  - URLs  
  - HTML tags  
  - Punctuation  
  - Numbers  
- Clean unwanted characters  

### 2️⃣ Feature Extraction
- Used TF-IDF Vectorization  
- Limited to 5000 features for efficiency  

### 3️⃣ Model Training
- Algorithm: Logistic Regression  
- Train-test split: 80% training / 20% testing  

### 4️⃣ Model Evaluation
- Metrics used:
  - Accuracy Score  
  - Classification Report  

### 5️⃣ Prediction System
Custom function for real-time prediction:

```python
predict_comment("Your comment here")
