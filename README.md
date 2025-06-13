
# 🛡️ PHISHING DETECTION SYSTEM

This project is a **Machine Learning-based Phishing Detection System** developed in Python. It detects whether a given URL is **legitimate** or **phishing** using trained classifiers and ensemble learning techniques. The system includes feature engineering, TF-IDF vectorization, and real-time prediction with confidence scoring.

---

## 📌 Key Features

-  URL-based feature extraction (length, IP, symbols, etc.)
-  TF-IDF vectorization of raw URL strings
-  Random Forest & 📈 Logistic Regression models
-  Ensemble Voting Classifier (Soft Voting)
- SMOTE for class imbalance (optional)
-  Real-time prediction with confidence score
-  Model saving and loading with `joblib`
-  Easily testable and extendable

---

##  Example Output

```

🔗 Enter a URL to classify: [https://www.google.com](https://www.google.com)

🌲 Random Forest says: ✅ Legitimate (Confidence: 98.2%)




```

---

##  Project Structure

```

📦PHISHING\_DETECTION\_SYSTEM/
├── dataset\_phishing.csv
├── balanced\_url\_dataset.csv
├── rf\_model.pkl
├── rf\_model\_tfidf.pkl
├── tfidf\_vectorizer.pkl
├── scaler.pkl
├── expected\_features.pkl
├── preprocessing\_and\_training.py
├── predict\_url.py
└── README.md

````

---

## ⚙️ How to Run

###  1. Install Requirements

```bash
pip install pandas scikit-learn joblib
````

###  2. Train the Model

Run this in your Python environment or Colab:

```bash
python preprocessing_and_training.py
```

This will save:

* `rf_model.pkl`
* `tfidf_vectorizer.pkl`
* `scaler.pkl`
* `expected_features.pkl`

### 🔍 3. Predict URLs

Run the prediction script:

```bash
python predict_url.py
```

Then input a URL like:

```
🔗 Enter a URL to classify: https://example.com
```

---

## 🧠 Machine Learning Models

* `RandomForestClassifier`

---

## 🔬 Techniques Used

*  Feature Engineering (URL length, dots, hyphens, digits, etc.)
* TF-IDF Vectorization of raw URL text
*  SMOTE (Synthetic Minority Oversampling) to balance phishing vs. legit classes
*  Probability calibration for soft voting confidence

---

## 🗃 Dataset Info

* The dataset contains URLs labeled as either `legitimate` (0) or `phishing` (1).
* Preprocessed to include key URL characteristics for ML training.

---

## 💡 Sample URLs for Testing

### ✅ Legitimate URLs

* [https://www.google.com](https://www.google.com)
* [https://www.wikipedia.org](https://www.wikipedia.org)
* [https://www.amazon.com](https://www.amazon.com)
* [https://github.com](https://github.com)

### ⚠️ Phishing URLs

* [http://login.secure-update-verification.com](http://login.secure-update-verification.com)
* [http://bankofamerica.account.verify-user.com](http://bankofamerica.account.verify-user.com)
* [http://paypal.user-security-alert.tk](http://paypal.user-security-alert.tk)
* [http://bit.ly/verify-now](http://bit.ly/verify-now)

*(Use responsibly for testing only — do not click suspicious links.)*

---

## 🚀 Deployment Ideas

* Deploy as a **Flask/FastAPI Web App**
* Convert to a **browser extension**
* Package as a **microservice for enterprise use**
* Build a **dashboard** using Streamlit or Dash

---

## 👨‍💻 Author

**ShadowStriker**
GitHub: [@shadowstriker663](https://github.com/shadowstriker663)

---

## 📄 License

This project is released under the **MIT License** — free for personal and commercial use.

---

## 🔭 Future Enhancements

* Integrate WHOIS and DNS-based features
* Live phishing lookup with VirusTotal/PhishTank APIs
* Build RESTful microservice or web extension
* Add database and logging support

---

## 📌 Repository

🔗 GitHub Repo: [PHIISHING\_DETECTION\_SYSTEM](https://github.com/shadowstriker663/PHIISHING_DETECTION_SYSTEM)

```

---

Let me know if you’d like this README translated into French or turned into a `.md` file automatically in Colab.
```
