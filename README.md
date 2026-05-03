# 👗 What Makes Customers Recommend a Clothing Product?
**DSA 210 – Introduction to Data Science | Term Project**
**Selin Ildeniz | 35847 | Spring 2026**

---

## 📌 Overview
This project investigates **what drives customers to recommend a clothing product** on an e-commerce platform. Using a dataset of over 23,000 women's clothing reviews, the goal is to analyze and predict whether a customer will recommend a product based on attributes like age, rating, review sentiment, department, and review length.

---

## 📊 Dataset
The data comes from the [Women's Clothing E-Commerce Reviews](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews) dataset on Kaggle.

**Core fields:**

| Feature | Description |
|---|---|
| `Age` | Reviewer's age |
| `Rating` | 1–5 star product rating |
| `Recommended IND` | Binary — 1 if customer recommends the product |
| `Positive Feedback Count` | Number of customers who found the review helpful |
| `Division Name` | High-level product division |
| `Department Name` | Product department |
| `Class Name` | Product class |
| `Review Text` | Written review content |

### Derived Features
- **Review Length** — word count of the written review
- **Sentiment** — polarity score computed from review text using TextBlob
- **Age Group** — binned age categories

---

## 🔬 Methodology

1. **Exploratory Data Analysis** — distributions of ratings, age, sentiment, review length; engagement patterns across departments and divisions
2. **Hypothesis Testing** — statistical tests on age, sentiment, department rating differences, and review length vs. recommendation status
3. **Machine Learning** — supervised and unsupervised methods applied to customer and review features:
   - k-Nearest Neighbours (classification)
   - Decision Tree (classification + feature importances)
   - Logistic Regression (classification + ROC-AUC)
   - K-Means Clustering (customer segments)
   - PCA (dimensionality reduction & visualisation)

---

## 🚀 How to Reproduce

1. Clone this repository
2. Create a free [Kaggle](https://www.kaggle.com) account if you don't have one
3. Download the dataset from [here](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews)
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
5. Open `DSA210_EDA_HypothesisTesting_Colab.ipynb` in Google Colab, upload `data_enriched.csv` when prompted, and run all cells

---

## 📅 Timeline

| Milestone | Date | Status |
|---|---|---|
| Repository created | March 17 | ✅ Done |
| Proposal submitted | March 31 | ✅ Done |
| EDA & hypothesis testing | April 14 | ✅ Done |
| ML methods | May 5 | ✅ Done |
| Final report | May 18 | 🔜 Upcoming |

---

## 🤖 AI Disclosure

This project used Claude (Anthropic) to assist with generating the Machine Learning section (Section 8) of the notebook, including code for kNN, Decision Tree, Logistic Regression, K-Means, and PCA. All code was reviewed, understood, and verified by the author before submission.

---

## 📎 Links

- **Dataset:** [Women's Clothing E-Commerce Reviews – Kaggle](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews)
