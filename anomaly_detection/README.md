# 🕵️‍♂️ Credit Card Fraud Detection (Anomaly Detection)

This project demonstrates **unsupervised anomaly detection** applied to the famous **credit card fraud dataset**.
It is part of the **`ml-unsupervised`** repository, which contains projects showcasing different unsupervised learning techniques.

---

## 📌 Project Overview

* Fraud detection is a **highly imbalanced classification problem** where fraudulent transactions represent less than 0.2% of the dataset.
* We apply **Gaussian Anomaly Detection** using two approaches:

  1. **Manual Multivariate Gaussian Implementation** → full mathematical intuition.
  2. **EllipticEnvelope (sklearn)** → robust covariance estimation (black-box approach).
* The notebook walks through:

  * Dataset exploration & visualization (EDA)
  * Preprocessing (scaling, splitting)
  * Anomaly detection (manual + sklearn)
  * Model evaluation (confusion matrix, ROC curve, metrics)
  * Comparison & insights

---

## 📂 Folder Structure

```
ml-unsupervised/
│
├── anomaly_detection/
│   ├── credit_card_fraud_detection.ipynb   # Main notebook
│   └── README.md                           # This file
│
└── other_subfolders... (future projects)
```

---

## ⚙️ Requirements

* Python 3.8+
* Install dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy
```

---

## 🚀 How to Run

1. Clone the repo:

```bash
git clone https://github.com/Ersatz-xD/ml-unsupervised.git
cd ml-unsupervised/anomaly_detection
```

2. Place the dataset (`creditcard.csv`) inside the folder .

3. Open the notebook:

```bash
jupyter notebook credit_card_fraud_detection.ipynb
```

---

## 📊 Results

* **Manual Gaussian**:

  * AUC ≈ 0.74
  * Detected almost all frauds but many false positives.

* **EllipticEnvelope**:

  * AUC ≈ 0.51
  * Very few false positives but missed nearly all fraud cases.

👉 Trade-off between **recall** (catching fraud) and **precision** (avoiding false alarms).

---

## 🏁 Conclusion

* Manual Gaussian anomaly detection is more **transparent and effective** for this dataset compared to EllipticEnvelope.
* Fraud detection requires **threshold tuning** and often combines anomaly detection with **supervised classifiers** for better performance.
* This project highlights how unsupervised learning can uncover rare fraudulent patterns without relying on labeled data.

---

