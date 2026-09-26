# Customer Shopping Behavior Analysis

Analysis of 3,900 retail transactions to uncover the factors that drive customer spending, retention, and product performance — using SQL for analysis and Power BI for visualization.

## 📌 Business Question

> How can the company leverage consumer shopping data to identify trends, improve customer engagement, and optimize marketing and product strategies?

## 🗂️ Dataset

- **3,900 records**, 18 attributes: demographics (age, gender, location), purchase details (item, category, amount, season), engagement signals (review rating, subscription status, discount/promo usage), and behavior (previous purchases, purchase frequency, shipping type, payment method).

## 🛠️ Tools Used

- **Python (Pandas)** — data cleaning: missing review ratings imputed by category median, standardized column names, removed a redundant promo-code column
- **PostgreSQL / SQL** — 10 targeted business questions answered via aggregation, window functions, and CTEs
- **Power BI** — interactive dashboard for ongoing monitoring by category, age group, gender, and subscription status

## 🔍 Methodology

1. Loaded and cleaned the raw dataset in Python
2. Loaded cleaned data into PostgreSQL
3. Wrote SQL queries to answer 10 business questions (revenue drivers, discount behavior, top products, shipping impact, subscription value, customer segmentation, repeat-buyer patterns)
4. Built a Power BI dashboard to summarize and visualize the results

## 📊 Key Insights

| # | Question | Finding |
|---|----------|---------|
| 1 | Revenue by gender | Male customers drive ~68% of revenue, but spend **per customer** is nearly equal across genders — the gap is customer count, not behavior |
| 2 | Discount users vs. avg. spend | A meaningful share of discount users still spend above the dataset average |
| 3 | Top-rated products | Gloves, Sandals, Boots, Hat, Skirt (avg. rating 3.78–3.86) |
| 4 | Shipping type vs. spend | Express shipping orders average **$2 more** than Standard |
| 5 | Subscribers vs. non-subscribers | Avg. spend is nearly identical ($59.49 vs. $59.87) — subscription isn't driving bigger baskets |
| 6 | Most-discounted products | Hat, Sneakers, Coat, Sweater, Pants — discounted on ~47–50% of purchases |
| 7 | Customer segments | 80% Loyal, 18% Returning, only **2% New** |
| 8 | Best sellers by category | Jewelry, Blouse, Sandals, Jacket lead their categories |
| 9 | Repeat buyers vs. subscription | 72% of repeat buyers (>5 purchases) are **not** subscribed |
| 10 | Revenue by age group | Fairly even; Young Adults slightly ahead ($62.1K) |

## 📈 Dashboard

The dashboard consolidates customer count, average purchase amount, average review rating, and revenue/sales breakdowns by category, age group, and subscription status.

*(Add a screenshot here, e.g. `![Dashboard](images/dashboard.png)`)*

## 💡 Business Recommendations

1. **Grow the female customer base** — spend per customer is equal; the opportunity is acquisition, not behavior change
2. **Prioritize new customer acquisition** — retention is strong, but new-customer inflow (2%) is a growth risk
3. **Re-evaluate the subscription program** — redesign perks around basket size and convert the 2,518 non-subscribed repeat buyers
4. **Review markdown strategy** on high-discount items to protect margin
5. **Promote express shipping** at checkout to lift average order value
6. **Feature top-rated and best-selling products** in marketing and merchandising
7. **Sustain broad-based marketing** across age groups, with incremental focus on Young Adults

## 📁 Repo Structure

```
├── data/               # raw & cleaned dataset
├── sql/                # SQL scripts for the 10 business questions
├── notebooks/          # Python data cleaning notebook
├── dashboard/          # Power BI (.pbix) file
├── report/             # Full project report (PDF/DOCX)
└── README.md
```

## 👤 Author

*Add your name / contact / LinkedIn here.*
