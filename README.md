# PHIISHING_DETECTION_SYSTEM
# 🛡️ PHISHING DETECTION SYSTEM

This project is a **machine learning-based phishing URL detection system**. It utilizes feature engineering, TF-IDF vectorization, and ensemble learning to classify URLs as **legitimate** or **phishing**.

## 📌 Features

- URL-based feature extraction
- TF-IDF vectorization
- Random Forest.
- Real-time URL classification with confidence score
- Optional SMOTE for handling imbalanced datasets
- Deployable via command line or web API

---
.
├── dataset_phishing.csv
├── balanced_url_dataset.csv
├── rf_model.pkl
├── rf_model_tfidf.pkl
├── lr_model.pkl
├── voting_classifier.pkl
├── tfidf_vectorizer.pkl
├── scaler.pkl
├── scaler_domain_features.pkl
├── expected_features.pkl
├── predict_url.py
├── preprocessing_and_training.py
└── README.md

## 🧪 Sample Prediction

```bash
🔗 Enter a URL to classify: https://www.google.com

 Random Forest says:  Legitimate (Confidence: 98.2%)


