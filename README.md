# 📊 Marketing Analytics Portfolio

🔗 Live Project: https://github.com/rutsatpa/marketing-product-analytics-portfolio

🛠 Tools: SQL | BigQuery | Marketing Analytics

Project 1: Marketing Decision Simulation 

Problem Statment:
Analyzing marketing performance across Channel, devices and traffic sources to identify growth opportunity and optimize business decisions.

Dataset:
Source: Google Analytics Public Dataset (Bigquery)
Data includes:
  - User Session
  - Traffic Source (Source / medium)
  - Device category
  - Pageview
  - Transactions
  - Revenue

Tootls Used:
  - BigQuery (SQL)
  - GitHub (documentation)

Analysis Approach
1. Data Preparation
-  Extracted relevant fields from raw GA dataset
-  Cleaned data using SQL (handled NULLs, formatted date, converted revenue)
-  Created analysis table: channel_performance_raw

2. Traffic Analysis
Identified user distribution across channels
👉 Insight:
-  Direct traffic contributes highest users
-  Indicates strong brand recall + attribution gaps

3. Conversion Analysis
Compared transactions vs users
👉 Insight:
-  High traffic ≠ high conversion
-  basecamp.com shows high conversion → high intent users
-  Direct traffic has lower conversion efficiency

4. Referral Ecosystem
Analyzed referral sources
👉 Insight:
-  Platforms like Facebook, Reddit, Quora drive traffic
-  Indicates content-driven + community-based discovery

5. Device Analysis
Compared performance across devices
👉 Insight:
-  Desktop: highest traffic + highest conversion
-  Mobile: high traffic but low conversion
-  Indicates mobile UX friction

💡 Business Recommendations
- Scale high-conversion sources (e.g., basecamp partnerships)
- Improve attribution tracking (reduce “direct” ambiguity)
- Optimize mobile experience (checkout, speed, UX)
- Focus on converting mobile traffic into revenue

📈 Key Learnings
- Data ≠ Insight → Interpretation is critical
- Conversion rate is more important than traffic
- User behavior differs significantly by device
- Marketing decisions must be backed by data

📌 Conclusion
- This project demonstrates end-to-end marketing analytics workflow:
- data extraction → transformation → analysis → business recommendations.


SQL Queries:
#To identify conversion rate
SELECT
  source,
  medium,
  COUNT(DISTINCT user_id) AS total_users,
  SUM(transactions) AS total_transactions,
  SAFE_DIVIDE(SUM(transactions), COUNT(DISTINCT user_id)) AS conversion_rate
FROM `marketing_data.channel_performance_raw`
GROUP BY source, medium
ORDER BY total_users DESC;


## 📸 Analysis Snapshots

### Traffic Analysis
👉 Direct traffic contributes the highest user volume, indicating strong brand recall and potential attribution gaps.
<img width="1415" height="686" alt="Project 1 - Query Result - Traffic Source" src="https://github.com/user-attachments/assets/f0243a30-0fe6-4ded-8fcb-482c305a7290" />

### Conversion Analysis
👉 High-traffic channels like Direct show lower conversion efficiency, while niche sources indicate high user intent.
<img width="932" height="733" alt="Project 1 - Query Result - Channel Converion Rate" src="https://github.com/user-attachments/assets/546a1cff-8a54-4375-a82c-ff89859e5f4d" />

### Device Analysis
👉 Desktop users show significantly higher conversion rates compared to mobile, indicating potential mobile UX friction.
<img width="748" height="203" alt="Project 1 - Query Result - Device Performance" src="https://github.com/user-attachments/assets/fc33c458-5f40-4d30-96ef-2ed5863b06df" />


## 🎯 Project Outcome

- Identified inefficiencies in high-traffic channels
- Highlighted high-intent sources for scaling
- Diagnosed mobile conversion drop-offs
- Proposed actionable business optimizations
