# 📱 Amazon Phone Review — NLP Sentiment Analysis

> End-to-end Python project analyzing **67,986+ Amazon smartphone reviews** to uncover customer satisfaction patterns, brand performance insights, and product-level sentiment trends using EDA and NLP.

---

## 📌 Business Problem

Smartphone brands struggle to understand **what customers actually feel** about their products at scale. Manually reading thousands of reviews is impossible — so how do you identify:

- Which brands have the most satisfied customers?
- What drives negative reviews?
- Does price actually influence customer ratings?
- Are review trends seasonal?

This project answers all of the above using **data-driven NLP and exploratory analysis**.

---

## 🛠️ Tech Stack

| Tool | Usage |
|------|-------|
| Python | Core programming language |
| Pandas & NumPy | Data cleaning, merging, feature engineering |
| Matplotlib & Seaborn | Data visualizations |
| TextBlob | NLP sentiment analysis |
| Jupyter Notebook | Interactive development environment |

---

## 📂 Dataset Overview

- **Source:** [Amazon Cell Phones Reviews — Kaggle](https://www.kaggle.com/datasets/grikomsn/amazon-cell-phones-reviews)
- **Files:** `20191226-items.csv` (product data) + `20191226-reviews.csv` (review data)
- **Merged Records:** 67,986 reviews across multiple smartphone brands
- **Key Columns:** `brand`, `rating`, `price`, `totalReviews`, `helpfulVotes`, `date`, `review title`, `review body`

---

## ⚙️ Project Workflow

```
Raw Data (2 CSVs)
      ↓
Data Merging (ASIN key join)
      ↓
Data Cleaning (Missing values — brand filled with mode, helpfulVotes filled with 0)
      ↓
Feature Engineering (full_review = title + body)
      ↓
EDA & Visualizations (7 charts)
      ↓
NLP Sentiment Scoring (TextBlob polarity)
      ↓
Sentiment Classification (Positive / Negative / Neutral)
      ↓
Business Insights & Recommendations
```

---

## 📊 Analysis Performed

### Task 1 — Exploratory Data Analysis (EDA)
- Dataset shape, info, null value treatment
- Brand-wise average rating, total reviews, average price
- Missing value handling: ~20,000 brand nulls filled with mode

### Task 2 — Visualizations (7 Charts)
- **Rating Distribution** — histogram of all ratings
- **Price vs Rating** — scatter plot for price-rating relationship
- **Trend-wise Rating** — monthly average rating trend
- **Trend-wise Total Reviews** — monthly review volume trend
- **Brand-wise Average Rating** — horizontal bar chart
- **Brand-wise Total Reviews** — review volume by brand
- **Votes Rating-wise** — helpful votes by rating group

### Task 3 — NLP Sentiment Analysis
- Applied **TextBlob** polarity scoring on full review text
- Classified reviews: `Positive (>0.1)` | `Neutral (-0.1 to 0.1)` | `Negative (<-0.1)`
- Brand-wise sentiment distribution analysis

---

## 🔍 Key Insights

- 📦 Analyzed **67,986 smartphone reviews** across multiple brands and price ranges
- 📉 **~29.4% of reviews had missing brand data** — handled via mode imputation
- ⭐ Most customers rated products between **3.5 – 4 stars** — moderate overall satisfaction
- 📱 **Samsung** led in total review volume — highest market presence
- 💰 **Xiaomi** delivered the best value-for-money products based on rating vs price analysis
- 💡 **Price shows weak correlation with ratings** — customers rate based on experience, not cost
- 😠 **Negative reviews received the highest helpful votes** — dissatisfied customers engage more
- 📅 Review volume showed **seasonal trends** — certain months had significantly higher engagement
- 💬 **Positive sentiment dominated** overall — but negative reviews were more impactful per vote

---

## 💼 Business Recommendations

1. **Focus on mid-range smartphones** — price does not drive satisfaction; features and reliability do
2. **Investigate negative review drivers** — they receive the most helpful votes, meaning they influence other buyers heavily
3. **Use positive reviews in marketing** — leverage high-rated periods and brands in campaigns
4. **Launch promotions during high-engagement months** — seasonal trends show clear peaks
5. **Improve after-sales service** — negative sentiment is often service-related, not just product-related
6. **Brands with low review volume** should focus on encouraging verified purchaser reviews to improve visibility

---

## 📁 Repository Structure

```
CodeAlpha_Task/
│
├── Amazon Phone Review.ipynb     # Full analysis notebook (EDA + Visualizations + NLP)
├── 20191226-items.csv            # Product dataset
├── 20191226-reviews.csv          # Reviews dataset
└── README.md                     # Project documentation
```

---

## 🚀 How to Run

1. Clone the repository:
```bash
git clone https://github.com/Data897analysit/CodeAlpha_Task.git
```

2. Install dependencies:
```bash
pip install pandas numpy matplotlib seaborn textblob
```

3. Open the notebook:
```bash
jupyter notebook "Amazon Phone Review.ipynb"
```

4. Run all cells top to bottom ✅

---

## 🙋‍♀️ About Me

**Priyanshi Rajput** — Data Analyst with expertise in Python, SQL, Power BI, and Tableau.
Passionate about transforming raw data into actionable business decisions.

[![LinkedIn](https://img.shields.io/badge/LinkedIn-Connect-blue?logo=linkedin)](https://www.linkedin.com/in/priyanshi-rajput)
[![GitHub](https://img.shields.io/badge/GitHub-Portfolio-black?logo=github)](https://github.com/Data897analysit)
[![HackerRank](https://img.shields.io/badge/HackerRank-SQL%205★-brightgreen?logo=hackerrank)](https://www.hackerrank.com/profile/priyanshi1652001)
