# Marketing Analytics & Sentiment Analysis – Sports Ecommerce Store

## Objective

This project involved an end-to-end data-driven analysis for an online sports retailer facing declining customer engagement and conversion rates. I analysed the dataset, including customer feedback, to identify key trends and insights. By combining marketing analytics with sentiment analysis, I provided actionable recommendations to optimise marketing strategies, enhance the customer experience, and improve overall business performance.

---

## Data Overview

- **Source:** SQL Server backup file (`.bak`) obtained from GitHub  
- **Content:** Comprehensive dataset comprising customer details, product information, user engagement metrics, product interaction records, and customer reviews 
- **Details:** Dataset includes customer demographics, product attributes, conversions, clicks, views, likes, engagement duration, drop-offs, conversions, and customer review texts intended for sentiment analysis  
- **Schema:** Galaxy schema architecture with multiple fact tables representing user engagement, product details, customer information, and review data  


---

## Methodology

### Data Preparation

- Restored the `.bak` file in **SQL Server**
- Performed data cleaning, joins, and formatting using SQL scripts

### Sentiment Analysis (Python)

- Used `TextBlob` to analyse customer reviews
- Generated:
  - Sentiment Categories: Positive, Negative, Neutral
  - Sentiment Scores (based on polarity)
- Exported results to `.xlsx` for Power BI integration

### Data Modelling & Visualisation (Power BI)

- Connected the .bak SQL Server backup file directly to Power BI via SQL Server connection and applied data cleaning within Power BI using SQL queries.
- Imported processed data into **Power BI**
- Performed hybrid cleaning using Power Query
- Created a **Calendar Table** for time-based analysis
- Defined KPIs with **DAX**:
  - Conversion Rate
  - Sentiment Score
  - Average Rating
  - Total Clicks, Views, Likes
- Designed an interactive dashboard with:
  - KPI overview
  - Monthly social engagement
  - Customer review sentiment
  - Product-wise conversion trends

---

## Key Insights

- **Conversion Rates** declined sharply in October (5.0%), then rebounded in December (10.2%)
- January had the **highest conversion rate** (18.5%), led by Ski Boots (150%)
- Social media views declined after July; CTR remained steady at **15.37%**
- Ratings averaged **3.7**; products below 3.5 need improvement
- Blog content had the **highest viewership**, particularly in April and July

---

## Outcome

- Delivered a dynamic Power BI dashboard with drilldowns and filters
- Identified product categories needing optimisation based on sentiment
- Proposed enhancements in marketing strategy and product quality

---

## Future Work

- Integrate social media sentiment alongside reviews
- Build ML models to forecast conversion trends
- Automate ETL for real-time Power BI updates

---

## Tech Stack

| Tool/Language   | Usage                              |
|----------------|-------------------------------------|
| SQL Server      | Restored .bak file, Data wrangling, joins |
| Python (TextBlob) | Sentiment analysis of reviews     |
| Power BI        | Data modelling, DAX, dashboarding   |
| Excel           | Data export/import                 |

---

## 📂 Project Structure

```
marketing-analytics-sentiment-sports-ecommerce/
├── data/
│   ├── raw/ (MarketingAnalytics.bak)
│   └── processed/ (sentiment_tb_results.xlsx)
├── sql/
│ ├── dim_customers.sql
│ ├── dim_products.sql
│ ├── fact_customer_journey.sql
│ ├── fact_customer_reviews.sql
│ └── fact_engagement_data.sql
├── python/
│   └── sentiment_textblob_customer_reviews.py
│   └── sentiment_textblob_customer_reviews.ipynb
├── powerbi/
│   └── dashboard.pbix
├── docs/
│   ├── interactive_dashboard_demo.mp4
│   └── marketing_analytics_presentation.pptx
│   └── screenshots/ — contains project-related screenshots
├── LICENSE
└── README.md

```

---

## Deliverables

- [`powerbi/dashboard.pbix`](powerbi/dashboard.pbix) – Open with [Power BI Desktop](https://powerbi.microsoft.com/desktop/)
- [`docs/interactive_dashboard_demo.mp4`](docs/interactive_dashboard_demo.mp4)
- [Presentation Slides (PPTX)](docs/marketing_analytics_presentation.pptx)

---


---

## 🌐 Connect with Me

- 🌍 Portfolio: [www.thusyanthan.dev](https://www.thusyanthan.dev)
- 💼 LinkedIn: [R Thusyanthan](https://www.linkedin.com/in/rthusy/)

---

> This project is part of my journey into data analytics and business intelligence. I’m continuously working on real-world projects—follow along to explore more!
=======
