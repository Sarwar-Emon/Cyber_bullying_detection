# Cyber Bullying Detection using Machine Learning and NLP

## 📌 Project Overview
Cyberbullying is a serious issue on online platforms that can negatively impact mental health.
This project implements a **machine learning–based text classification system** to automatically detect whether a given text contains **cyberbullying content or not**.

The system uses traditional NLP techniques combined with multiple supervised machine learning models to evaluate and compare performance.

---

## 🎯 Objectives
- Detect cyberbullying in user-generated text
- Apply NLP preprocessing techniques
- Train and compare multiple machine learning classifiers
- Build a simple prediction-ready application

---

## 📂 Dataset
- File: `dataset.csv`
- Type: Text classification dataset
- Target labels:
  - `Cyberbullying`
  - `Non-Cyberbullying`

### Preprocessing includes:
- Text cleaning
- Stopword removal
- Vectorization using TF-IDF

---

## ⚙️ Models Implemented
The following models were trained and evaluated:

- Logistic Regression  
- Linear Support Vector Classifier (LinearSVC)  
- Tuned LinearSVC  
- Multinomial Naive Bayes  
- Decision Tree Classifier  
- AdaBoost Classifier  
- Bagging Classifier  
- SGD Classifier  

All trained models are stored in the `models/` directory.

---

## 📊 Model Evaluation
Models were evaluated using the following metrics:
- Accuracy
- Precision
- Recall
- F1-score
- Confusion Matrix

The **tuned LinearSVC** achieved the best overall performance on the test set:

- **Accuracy:** 91%
- **Precision:** 0.90
- **Recall:** 0.89
- **F1-score:** 0.90

### Example Prediction
```text
Input: "You are useless and stupid"
Output: Cyberbullying

## Project Structure
cyber_bullying_detection/
│── data/          # Dataset files
│── models/        # Trained ML models (.pkl)
│── notebooks/     # EDA and experimentation notebooks
│── src/           # Application and ML pipeline code
│── templates/     # HTML templates (Flask app)
│── README.md
│── requirements.txt

## Installation & Usage
pip install -r requirements.txt
python src/app.py
