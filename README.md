# Social Media Ads Targeting Strategy Analysis

## Executive Summary:
I analysed social media advertising data to understand how different age groups, genders, and interest segments respond to campaigns. The analysis revealed clear disparities between engagement and conversion performance across demographics. While some groups generated high impressions and clicks, they delivered poor conversions. By identifying high-value and low-value segments, the project outlines audience optimization opportunities to improve targeting efficiency and overall campaign ROI.

## Business Problem:
Marketing teams need to allocate advertising budget to audience groups that convert efficiently, rather than those that merely generate engagement. However, existing targeting often includes demographics that produce high impressions and clicks but fail to convert, resulting in wasted spend. The objective of this project was to analyse demographic performance across key metrics to determine:
- Which audience groups deliver the strongest conversion outcomes
- Where spend is inefficient due to low post-click performance
- How targeting strategy can be adjusted to improve ROI and campaign effectiveness

## Methodology:
1. Created a database, schema, and tables in PostgreSQL to store the campaign dataset.
2. Imported [dataset](https://www.kaggle.com/datasets/alperenmyung/social-media-advertisement-performance) from [kaggle](https://www.kaggle.com/) to PostgreSQL tables.
3. Inspected all tables for accuracy. The "users" table contains duplicate entries- this is a bit complicated as some users from different regions share the same user_id, and since foreign keys point to this user_id, updating it will disrupt the whole database setup. Additionally, seeing the duplicates consistitute only about 1.07% of the dataset, they can be dropped without affecting analysis results significantly.
4. Created a **View** "cleaned_users" to filter out duplicates in the "users" table.
5. Computed core marketing KPIs including CTR, Conversion Rate, and CPC.
6. Segmented audience performance by age, gender, market, and interest groups.
7. Compared engagement strength versus conversion efficiency to identify misleading high-engagement segments.

## Skills:
-  SQL: Data cleaning, segmentation, KPI calculations.
-  Python: Exploratory data analysis and demographic performance comparisons.
-  Marketing Analytics: CTR, CPC, CPA, Conversion Rate, funnel interpretation.
-  Audience Segmentation: Identifying high-value vs low-value demographic groups.
-  Insight Development: Targeting optimisation, spend efficiency analysis.

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

### 4. Critical Drop-off: High Lead Interest but Zero Conversions in 55–65 Years Segment Across Three Countries
<img src="https://raw.githubusercontent.com/jacobdbt2100/Social-Media-Ads-Targeting-Strategy-Analysis/main/4_Leads Conversion Drop-off.jpg" width="400">

> In Canada, France, and Japan, the 55–65 age group drives strong engagement and clicks but records zero conversions, indicating likely technical, eligibility, or funnel barriers.

> REFINE LATER: Going by the average conversion rate, an estimated loss of --- purchases was incurred due to the zero post-click conversion across these countries for age group 55-65.

- Audit conversion flows for this segment—check forms, device compatibility, age restrictions, and country-specific filters to unlock high-intent leads.

### 5. High-Conversion Markets Concentrated in Japan, Mexico, U.S., and Canada
<img src="https://raw.githubusercontent.com/jacobdbt2100/Social-Media-Ads-Targeting-Strategy-Analysis/main/5_Country Post-click Conversions.jpg" width="750">

> These four markets delivered the highest post-click conversion rates higher or closest to the overall average of 5.07%

- Prioritize spend and optimization in these high-performing markets.

### 6. Tech-Linked Interests Drive Highest Conversions; Lifestyle & Gaming Underperform

<img src="https://raw.githubusercontent.com/jacobdbt2100/Social-Media-Ads-Targeting-Strategy-Analysis/main/6_Interests Post-click Conversions.jpg" width="900">

> Interest combinations tied to technology consistently yield the strongest conversion rates, outperforming the lowest segments by more than 3–4 times. In contrast, lifestyle-, gaming-, and travel-oriented audiences show limited purchase intent, signaling weaker alignment with the campaign value proposition.

- Concentrate targeting on tech-adjacent interest clusters and scale back low-intent segments.

- update visual

___
 
