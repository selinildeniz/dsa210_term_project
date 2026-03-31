# 👗 What Makes Customers Recommend a Clothing Product?

**DSA 210 – Introduction to Data Science | Term Project**
**Selin Ildeniz | 35847 | Spring 2026**

---

## 📌 Overview

This project digs into **23,000 real customer reviews** from a women's fashion e-commerce platform to uncover what drives a customer to recommend a product. By combining exploratory analysis, hypothesis testing, and machine learning, the goal is to understand the relationship between customer demographics, product attributes, and review sentiment — and to predict whether a customer will recommend an item.

---

## 📊 Dataset

The data comes from the [Women's E-Commerce Clothing Reviews](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews) dataset on Kaggle (~23,000 reviews).

Each record includes:

| Feature | Description |
|---|---|
| `Clothing ID` | Unique product identifier |
| `Age` | Reviewer's age |
| `Title` | Short review headline |
| `Review Text` | Full written review |
| `Rating` | 1–5 star score |
| `Recommended IND` | Binary — 1 if recommended, 0 if not |
| `Positive Feedback Count` | Number of users who found the review helpful |
| `Division / Department / Class Name` | Product category labels |

### Derived Features

To add analytical depth, the following features are engineered from the raw data:

- **Review Length** — word count of each review
- **Age Group** — binned categories (Under 30 · 30–45 · 45–60 · Over 60)
- **Sentiment Polarity** — lexicon-based sentiment score from the review text

---

## 🔬 Methodology

1. **Exploratory Data Analysis** — distributions, category breakdowns, and visual patterns
2. **Hypothesis Testing** — statistical tests (t-test, chi-squared) on factors like age and rating vs. recommendation
3. **Predictive Modeling** — logistic regression to predict the `Recommended IND` column, evaluated with accuracy and AUC-ROC

---

## 🚀 How to Reproduce

1. Clone this repository
2. Download the dataset from [Kaggle](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews) (free account required)
3. Place `Womens Clothing E-Commerce Reviews.csv` inside the `/data` folder
4. Install dependencies:
   ```bash
   pip install -r requirements.txt
   ```
5. Run the notebooks in order inside `/notebooks`

> The `/data` folder is excluded via `.gitignore` — the dataset is not uploaded to this repo.

---

## 📅 Timeline

| Milestone | Date | Status |
|---|---|---|
| Repository created | March 17  |
| Proposal submitted | March 31 |
| EDA & hypothesis testing | April 14  |
| ML methods | May 5 |
| Final report | May 18 |

---

## 📎 Links

- **Dataset:** [Kaggle – Women's E-Commerce Clothing Reviews](https://www.kaggle.com/datasets/nicapotato/womens-ecommerce-clothing-reviews)
