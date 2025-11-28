# Social Media Ads Targeting Strategy Analysis

## Executive Summary:
This project analyses social media advertisement performance to understand how different demographic groups respond to campaigns. The goal is to identify the audience segments that deliver the highest engagement and conversions relative to spend, and to highlight where targeting adjustments can improve efficiency.

## Business Problem:
Marketing teams want to optimise ad spend by focusing on the right audience. However, current targeting may include age groups or genders that show high impressions and clicks but low conversions. This results in wasted spend and poor campaign efficiency. The project aims to determine:
-  Which demographic groups convert best
-  Where spend is inefficient
-  How targeting can be refined to improve ROI

## Methodology:
1. Imported the dataset from Kaggle into SQL and Python.
2. Explored campaign performance across impressions, clicks, spend, and conversions.
3. Created key metrics (CTR, CPC, Conversion Rate, CPA) to compare audience groups.
4. Analysed how age, gender, and campaign interact with performance and cost.
5. Identified patterns indicating high-value vs low-value audience segments.

## Skills:
-  Data cleaning and SQL querying
-  Exploratory data analysis
-  KPI creation and interpretation
-  Audience segmentation
-  Marketing analytics concepts (CTR, CPA, conversion modelling)
-  Insight development for targeting strategy optimisation

## Insights & Recommendation:

### 1. Channel Performance Shift: Instagram Leads in Clicks, Facebook Wins in Conversions.
<img src="https://raw.githubusercontent.com/jacobdbt2100/Social-Media-Ads-Targeting-Strategy-Analysis/main/1_Ads Platforms Performance.jpg" width="800">

> **Instagram** drives marginally higher **clicks** (**11.86%**), but **Facebook converts** more efficiently (**5.21%**), indicating stronger lower-funnel performance on Facebook.

- Use **Instagram** for **reach and engagement**, and prioritize **Facebook** for **conversion-led** campaigns.

### 2. Older Audiences Drive the Strongest Lead (Intent) Activity Across Markets
<img src="https://raw.githubusercontent.com/jacobdbt2100/Social-Media-Ads-Targeting-Strategy-Analysis/main/2_Leads.jpg" width="800">

> The 55–65 age group consistently generates the highest lead activity across all countries.

- Prioritize the 55–65 segment for lead-focused (I think AWARENESS-FOCUSDE) campaigns, supported by younger groups for broader reach.

### 3. Engagement Leaders Are Not Conversion Drivers
<img src="https://raw.githubusercontent.com/jacobdbt2100/Social-Media-Ads-Targeting-Strategy-Analysis/main/3_Age-wise Engagements & Conversions.jpg" width="900">

> Top-engaging age groups differ from top-converting ones across all countries. In three markets, the 55–65 group shows the highest engagement but delivers zero conversions.

> With the exception of Mexico, all other nine countries showed sharp contrast between engagement and conversion rates.

- Use high-engagement segments for awareness only and target conversion-heavy age groups for sales campaigns.

### 4.
<img src="https://raw.githubusercontent.com/jacobdbt2100/Social-Media-Ads-Targeting-Strategy-Analysis/main/4_Leads Conversion Drop-off.jpg" width="400">

### 5. Zero Conversion Across Three Countries Despite Substantial Lead Activity
<img src="https://raw.githubusercontent.com/jacobdbt2100/Social-Media-Ads-Targeting-Strategy-Analysis/main/5_Country Post-click Conversions.jpg" width="750">

> Going by the average conversion rate, an estimated loss of --- purchases was incurred due to the zero post-click conversion across these countries for age group 55-65.

### 6.
- update visual
<img src="https://raw.githubusercontent.com/jacobdbt2100/Social-Media-Ads-Targeting-Strategy-Analysis/main/6_Interests Post-click Conversions.jpg" width="900">

___
 
[Data set](https://www.kaggle.com/datasets/alperenmyung/social-media-advertisement-performance)
