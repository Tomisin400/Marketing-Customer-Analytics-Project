# Marketing and Customer Behavior Analysis
An Excel Project | Turning raw data to Business Insights

## Table of Contents

- [Project Overview](#project-overview)
- [Problem Statement](#problem-statement)
- [Data Sourcing](#data-sourcing)
- [Data Transformation & Cleaning](#data-transformation--cleaning)
- [Analysis & Measures](#analysis--measures)
- [Dashboard & Visuals](#dashboard--visuals)
- [Insights & Findings](#insights--findings)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)



## Project Overview
This project analyzes marketing performance and customer behavior for an E-commerce industry.  
The analysis helps the business understand which marketing channels and customer segments drive the most conversions and identify gaps in the conversion funnel.  
The insights from this analysis help this business:
- Optimize marketing spend
-	 Improve customer engagement
- Focus on high-value customer segments
-	Increase overall conversions and revenue.


## Problem Statement
The business needs help with:
- Deciding which marketing channels to invest in for better returns.  
- Understanding customer segments with the highest conversion potential.  
- Identifying bottlenecks in the conversion funnel.

Currently, the business does not know:
- Which campaigns deliver the most value  
- Why high engagement does not always lead to conversions  
- How customer segments perform by age, gender, and income


## Data Sourcing
- Data source: This project uses a dataset sourced from **Kaggle**, containing marketing performance and customer behavior data.
- Time period:  Jan 2026 
- Dataset Type: Marketing and customer behavior dataset
- Number of records: 318 rows each (excluding header)
- Key fields: Customer ID, Campaign Channel, Campaign Type, Ad Spend, CPA, Conversions, Conversion rate, Website visits, Age, Gender, Income, Email Opens, Email clicks, Time on Site, Loyalty Points
  
  Sample of dataset sheet
  <img width="953" height="473" alt="Sample of datasheet" src="https://github.com/user-attachments/assets/dddf7a54-4ac9-4358-9040-4fd6def48269" />


## Data Transformation & Cleaning
The dataset was prepared to ensure accuracy and consistency before analysis.
- Data Quality Check: Checked for duplicates and outliers, none were found.
- Missing values: Only one missing value was found and it was ignored as it did not impact the analysis.
- Feature Engineering: Calculated KPIs such as Total conversions and cost per acquisition (CPA)
- Added Income Group column in the customer analytics dataset using IF statements to categorize customers based on income levels (Low, Mid, High).
```Excel  
=IF([Income]<50000, "Low", IF([Income]<100000, "Mid", "High"))
```

### Analysis & Measures
The analysis focused on marketing performance and customer behavior. Key performance indicators (KPIs) were calculated to measure campaign effectiveness and customer engagement:
 Marketing KPIs Calculated:  
- Total Ad Spend: Sum of spend across all channels.
- Total Conversions: Sum of conversions for all marketing campaigns
- Average Conversion Rate: 10.5% 
- CPA: Total spend/Total conversions  5,150
- Total website visits: 8026
 Customer Analytics KPIs calculated:
- Total Customers: Number of unique customers in the dataset
- Average pages per visit :5
- Average time on site: 7.91
- Average loyalty points: 2442
- Total Conversions:295

### Dashboard & Visuals
The project includes two Excel dashboards
1.	Marketing Dashboard
The dashboards allow users to:
Filter by: Campaign Channel, Campaign Type
View KPIs: Total Spend, Total Conversions, Conversion Rate, CPA, Total website visits

<img width="950" height="462" alt="Marketing_dashboard" src="https://github.com/user-attachments/assets/90372082-2006-4745-9452-856d1ddca83c" />


2.	Customer Analytics Dashboard
Filter by: Income group, Gender
View KPIs: Total Customers, Total conversion, average pages per visit, Average time on site, Average loyalty points.

<img width="931" height="476" alt="Customer_dashboard" src="https://github.com/user-attachments/assets/c4bf26b8-65c7-4048-9ce6-5686163d23ba" />


### Insights & Findings
- Social media performs best but is underfunded
- High-value customers (ages 42–65) convert 95–100% but are not prioritized
-	Funnel shows major drop at email stage: only 33% of visitors engage
-	Engagement is strong (7–9 minutes, 5 pages per visit), but conversion is low (3.7%)

  
### Recommendations
-	Reallocate marketing spend to high-performing channels (e.g., Social media)
-	Target campaigns toward high-value customers (42–65)
-	Improve email engagement to reduce funnel drop-off
-	Continuously monitor KPIs and update dashboards

  
### Conclusion
The dashboards provide clear insights on marketing and customer performance which
helps the business increase conversions, reduce wasted spend, and prioritize high-value customers.

Next steps: continuous monitoring and personalization for high-potential segments.

