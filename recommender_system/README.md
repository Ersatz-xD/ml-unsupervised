
# 🎬 Movie Recommender System

This project demonstrates how to build a **Movie Recommender System** using the **MovieLens 100k dataset**.  
It is a sub-project of the main repository **[`ml-unsupervised`](../)**, where we explore different unsupervised machine learning techniques.

Notebook: **`movie_recommender_system.ipynb`**

---

## 📌 Project Overview

Recommender systems are one of the most widely used applications of machine learning.  
They help suggest movies, songs, products, and more based on user preferences.

In this notebook, we cover two classical approaches:

1. **Content-Based Filtering**
   - Uses **movie metadata (genres)**.
   - Recommends movies similar to a given one.
   - Example: `"Toy Story (1995)"` → suggests other **Animation/Comedy** movies.

2. **Collaborative Filtering**
   - Uses **user ratings** to find patterns between movies.
   - Suggests movies liked by similar users.
   - Example: `"Star Wars (1977)"` → suggests other **Sci-Fi/Action** movies popular among similar audiences.

---

## 📂 Project Structure

```

ml-unsupervised
│
├── anomaly_detection             
│   └── credit_card_fraud_detection.ipynb  
│   └── README.md
│
├── recommender_system            
│   ├── movie_recommender_system.ipynb  
│   └── README.md
│
└── ...

```

---

## 🚀 How to Run

1. Clone the main repo:
   ```bash
   git clone https://github.com/Ersatz-xD/ml-unsupervised.git
   cd ml-unsupervised/recommender_system
    ```

2. Install requirements:

   ```bash
   pip install pandas numpy scikit-learn
   ```

3. Open the notebook:

   ```bash
   jupyter notebook movie_recommender_system.ipynb
   ```

---

## 📊 Results

* **Content-Based Filtering** recommends movies based on **genres & similarity**.
* **Collaborative Filtering** recommends movies based on **user preferences**.
* Both methods have strengths and weaknesses:

  * Content-Based → works well for **new users**, but limited by available metadata.
  * Collaborative → captures **community taste**, but suffers from **cold-start problem**.

---

## 🙌 Acknowledgements

* Dataset: [MovieLens 100k](https://grouplens.org/datasets/movielens/100k/)
* Libraries: **pandas, numpy, scikit-learn**

---

💡 This project is designed for **learning and practice** in unsupervised ML.
Feel free to explore, tweak, and extend it!
