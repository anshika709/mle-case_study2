# mle-case_study2
# Financial Intelligence: Credit Card Fraud Detection via XGBoost & SMOTE

An end-to-end machine learning architecture utilizing synthetic oversampling and gradient boosting to detect anomalies in highly imbalanced transaction networks.

---

## 📋 Executive Summary

Credit card fraud represents a massive financial risk but forms an extreme minority of transaction data (~0.17%). This repository provides an end-to-end operational pipeline to safely balance heavily skewed transaction streams using **SMOTE** and classify risks using an optimized **XGBoost Framework**.

---

## 🎯 Core Objectives

High-precision binary classification of transactional risk profiles:
* **`0`**: Authorized (Legitimate transaction)
* **`1`**: Compromised (Fraudulent anomaly)

---

## 📊 Feature Architecture & Data Schema

Ingests highly dimensional transaction records (284,807 total rows) across 31 features:
* **Temporal & Fiscal Metrics:** `Time`, `Amount` (Normalized via `StandardScaler`)
* **Anonymized Identifiers:** `V1` through `V28` (PCA-transformed latent structural variables)
* **Target Vector:** `Class` (Highly imbalanced: 284,315 legitimate vs. 492 fraudulent records)

---

## ⚙️ Model Architecture & Pipeline

