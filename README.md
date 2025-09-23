# 🤖 ml-unsupervised

A collection of projects demonstrating **unsupervised machine learning techniques**.  
Each sub-folder is a self-contained project with its own notebook and README.

The goal of this repo is to provide **hands-on, beginner-friendly examples** of unsupervised ML applied to real-world datasets.

---

## 📂 Repository Structure

```

ml-unsupervised
│
├── anomaly_detection
│   ├── credit_card_fraud_detection.ipynb   # Fraud detection project
│   └── README.md
│
├── recommender_system/
│   ├── movie_recommender_system.ipynb      # Recommender system project
│   └── README.md
│
└── ... (future projects)

```

---

## 📌 Projects

### 🕵️‍♂️ Credit Card Fraud Detection (Anomaly Detection)

This project applies **unsupervised anomaly detection** to the famous **credit card fraud dataset**.

**Key Points:**
- Fraudulent transactions ≈ **0.2%** of dataset.
- Approaches used:
  - **Manual Multivariate Gaussian** (step-by-step math + implementation).
  - **EllipticEnvelope** (sklearn’s robust covariance method).
- Covers:
  - Exploratory Data Analysis (EDA).
  - Preprocessing (scaling, splitting).
  - Anomaly detection (manual + sklearn).
  - Evaluation: Confusion Matrix, ROC, metrics.
  - Comparison & insights.

**Results:**
- Manual Gaussian: **AUC ≈ 0.74** → good fraud detection, higher false positives.
- EllipticEnvelope: **AUC ≈ 0.51** → very few false positives, but missed most fraud.

👉 Conclusion: Unsupervised anomaly detection is useful, but balancing **recall vs precision** is critical in fraud detection.

📓 Notebook: [`anomaly_detection/credit_card_fraud_detection.ipynb`](anomaly_detection/credit_card_fraud_detection.ipynb)

---

### 🎬 Movie Recommender System

This project builds a **Movie Recommender System** using the **MovieLens 100k dataset**.

**Key Points:**
- Two classical approaches implemented:
  1. **Content-Based Filtering**
     - Uses movie genres with **TF-IDF similarity**.
     - Example: `"Toy Story (1995)"` → suggests other **Animation/Comedy** movies.
  2. **Collaborative Filtering**
     - Uses **user–movie ratings**.
     - Example: `"Star Wars (1977)"` → suggests other **Sci-Fi/Action** movies liked by similar audiences.
- Includes:
  - Dataset EDA (ratings distribution, popular movies, sparsity heatmap).
  - Functions to recommend movies by title.
  - Side-by-side comparison of methods.

**Results:**
- Content-Based → works well for **new users** but limited by metadata.
- Collaborative → captures **community taste** but suffers from **cold-start problem**.

📓 Notebook: [`recommender_system/movie_recommender_system.ipynb`](recommender_system/movie_recommender_system.ipynb)

---

## ⚙️ Requirements

All projects use **Python 3.8+**.  
Install common dependencies:

```bash
pip install numpy pandas matplotlib seaborn scikit-learn scipy
```

---

## 🚀 How to Run

1. Clone the repository:

   ```bash
   git clone https://github.com/Ersatz-xD/ml-unsupervised.git
   cd ml-unsupervised
   ```

2. Choose a project folder (e.g., `anomaly_detection` or `recommender_system`).

3. Place required dataset(s) in the folder (see project README).

4. Run the notebook:

   ```bash
   jupyter notebook notebook_name.ipynb
   ```

---

## 🙌 Acknowledgements

* Datasets:

  * [Credit Card Fraud Dataset (Kaggle)](https://www.kaggle.com/mlg-ulb/creditcardfraud)
  * [MovieLens 100k Dataset](https://grouplens.org/datasets/movielens/100k/)
* Libraries: **numpy, pandas, matplotlib, seaborn, scikit-learn, scipy**

---

💡 This repo is designed for **learning**.
Explore the notebooks, play with the code, and extend the projects!

