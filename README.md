# 💳 Credit Card Fraud Detection

> A comprehensive machine learning analysis of credit card transactions to detect fraudulent activity.  
> Demonstrates best practices for handling **extremely imbalanced datasets** and building **production‑ready** fraud detection models.

---

## 📊 Executive Summary

**Dataset:** 284,807 transactions  
**Fraud Cases:** 492 (0.17%)  
**Imbalance Ratio:** 1:579  

This project applies advanced machine learning techniques to identify fraudulent credit card transactions with high recall and interpretable insights.

---

## 🎯 Objectives

- ✅ Detect fraudulent transactions with high accuracy  
- ✅ Handle extreme class imbalance (99.83% legitimate, 0.17% fraud)  
- ✅ Build interpretable, actionable, and robust models  
- ✅ Optimize decision thresholds for different business goals  

---

## 🧠 Methodology Overview

1. **Data Preprocessing**
   - Removed time feature (not predictive)
   - Scaled transaction amount with `RobustScaler`
   - Handled 284,807 transactions with zero missing values

2. **Class Imbalance Handling**
   - Random oversampling to achieve 50–50 balance
   - Stratified train–test split (30% test set)
   - Integrity preserved for minority (fraud) class

3. **Model Training and Evaluation**
   - Compared three algorithms: Logistic Regression, Random Forest, Gradient Boosting
   - Used stratified sampling and consistent metrics
   - Evaluated ROC‑AUC, F1‑Score, Precision, and Recall

---

## 📈 Model Performance Comparison

| Model | ROC-AUC | F1-Score | Precision | Recall |
|-------|---------|----------|-----------|--------|
| **Logistic Regression** | 0.9699 | 0.1180 | 0.06 | 0.87 |
| **Random Forest** | 0.9441 | 0.8276 | 0.96 | 0.73 |
| **Gradient Boosting** ⭐ | **0.9734** | **0.3414** | **0.21** | **0.86** |

**🏆 Best Model:** Gradient Boosting  
- Excellent ROC‑AUC (0.9734)  
- Strong recall (0.86)  
- Balanced fraud detection capabilities

---

## 🔍 Detailed Model Analysis

### Gradient Boosting Classification Report
