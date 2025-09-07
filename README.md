# 📊 ML Cross-Validation & Advanced Metrics  

## 🔎 Project Overview  
This repository provides a **reusable pipeline** for evaluating machine learning classification models using **cross-validation** and **advanced evaluation metrics**.  
It includes modular functions for metrics computation, confusion matrix visualization, and reporting.  

---

## 📂 Dataset Description  
- You can use any **preprocessed classification dataset (CSV)**.  
- The target column should contain class labels (binary or multi-class).  
- Example demo dataset: **Breast Cancer Wisconsin (Diagnostic)** from scikit-learn.  
- Expected format:  

| feature1 | feature2 | feature3 | ... | target |  
|----------|----------|----------|-----|--------|  
| 0.23     | 12.1     | 4.56     | ... | 0      |  
| 0.45     | 11.8     | 3.92     | ... | 1      |  

---

## 🤖 Model Description  
The pipeline supports **any scikit-learn classifier**, including:  
- Logistic Regression (default)  
- Random Forest Classifier  
- Support Vector Machine  
- Gradient Boosting, etc.  

You can change the model in the script by updating:  
```python
MODEL = LogisticRegression(max_iter=1000, random_state=42)
