# 📊 Marketing Analytics Portfolio

💡 Key Finding: High-traffic channels like YouTube drive acquisition, but conversion inefficiency and attribution gaps lead to under-optimized marketing spend.

🔗 Live Project: https://github.com/rutsatpa/marketing-product-analytics-portfolio

🛠 Tools: SQL(BigQuery) | Power BI | Funnel Analysis | Attribution Modeling (FIrst Touch Vs Last Touch) | Marketing Analytics | 


# 📊 Marketing Analytics Case Study (End-to-End Funnel & Attribution Analysis)

🚀 This project analyzes marketing performance across the full funnel — from user acquisition to conversion — and applies attribution thinking to identify growth opportunities.


## 🎯 Problem Statment:

Analyze marketing performance across channels and devices to:
- Identify high-value traffic sources
- Detect funnel drop-offs
- Evaluate channel efficiency
- Understand attribution gaps
- Recommend data-driven business decisions


Dataset:

Source: Google Analytics Public Dataset (Bigquery)
Data includes:
  - User Session
  - Traffic Source (Source / medium)
  - Device category
  - Pageview
  - Transactions
  - Revenue


## 🧠 Analytical Approach:

The analysis is structured across 4 layers:
1. Traffic & Conversion Analysis  
   → Who brings users vs who converts
2. Device Performance  
   → Where users convert best
3. Funnel Analysis  
   → Where users drop off (Pageview → Conversion)
4. Attribution Analysis  
   → First Touch (acquisition) vs Last Touch (conversion driver)


## 🔍 Key Insights

- Direct channel drives highest conversions, acting as a closing channel
- YouTube and referral channels drive high traffic but low conversion → awareness role
- Significant drop-off occurs between engagement and conversion stage
- Desktop users convert significantly higher than mobile → UX gap
- Attribution gap observed: upper-funnel channels are undervalued in last-touch models
- Direct appearing as both first and last touch suggests tracking limitations and returning users


## 🎯 Why This Matters

- Prevents misallocation of marketing budget due to attribution bias  
- Identifies true growth levers across acquisition and conversion  
- Helps prioritize funnel optimization over traffic scaling  



## 📊 Dashboard Overview

### Device Performance
<img width="959" height="505" alt="image" src="https://github.com/user-attachments/assets/bbd553b1-68be-4f4a-9ec1-4b57feb3bd7f" />

### Revenue Contribution
<img width="655" height="509" alt="image" src="https://github.com/user-attachments/assets/3dc7db93-2bc6-47e0-8ec5-28737f65e46a" />

### Channel Segementation
<img width="967" height="523" alt="image" src="https://github.com/user-attachments/assets/1a1217fb-853b-4b4a-9cb6-f3d1400dc529" />

### Efficiency Table 
<img width="651" height="589" alt="image" src="https://github.com/user-attachments/assets/728e3345-2853-4119-893e-90691ff23ebb" />

### Business Impact & Recommendations
<img width="657" height="135" alt="image" src="https://github.com/user-attachments/assets/e6b56c64-e72e-444a-b24d-eb8f5270d3ef" />

### Funnel Analysis
<img width="771" height="617" alt="image" src="https://github.com/user-attachments/assets/291a4f5c-2ba0-4813-8870-11b8c4156905" />

<img width="1033" height="485" alt="image" src="https://github.com/user-attachments/assets/5e79cca2-8476-4450-b8c9-4f9e5ddb3e29" />

### Attribution Analysis
<img width="1126" height="635" alt="image" src="https://github.com/user-attachments/assets/8a1c56df-a001-491e-9fb3-3e08e8398615" />
⚠️ Note: Conversion rate is intentionally not calculated in attribution analysis, as first-touch users and last-touch conversions belong to different attribution frameworks and combining them would lead to misleading insights.


## ⚠️ Limitations

- Attribution is simulated due to lack of user-level journey data  
- First-touch and last-touch models are approximations  
- Direct traffic may include untracked upstream sources


## 🚀 Next Steps

- Implement multi-touch attribution model  
- Incorporate user-level journey data  
- Run Incrementality/ Controlled A/B tests to improve conversion funnel   



## 💡 Business Recommendations:

- Optimize mobile experience (UX, checkout flow, page speed)
- Improve conversion funnel (reduce friction post engagement)
- Scale high-intent channels (DFA, email sources)
- Maintain awareness channels (YouTube, referrals) for demand generation
- Avoid over-reliance on last-touch attribution
- Move toward multi-touch attribution for better budget allocation



## 🛠 Tools & Skills

- SQL (BigQuery)
- Power BI (Dashboarding)
- Funnel Analysis
- Attribution Modeling (First Touch vs Last Touch)
- Marketing Analytics


## 🚀 Project Impact

This project demonstrates:
- End-to-end marketing analytics thinking
- Ability to identify funnel inefficiencies
- Understanding of attribution bias
- Data-driven decision-making for growth
