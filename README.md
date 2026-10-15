![alt text](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/assets/banner.jpg)

# Do Women Spend More Than Men on Black Friday? Customer Spend Analysis
Hypothesis testing and CLT confidence intervals on Black Friday retail transactions: spend differences by gender, age, city, and marital status.

## About Business
Walmart is an American multinational retail corporation that operates a chain of supercenters, discount departmental stores, and grocery stores from the United States. Walmart has more than 100 million customers worldwide.

**North Start Metrics**
* Spend per customer: Total purchase per User_ID
* Revenue share by segment
* Customer count per segment
* Median spend per customer
* Probability of a high-value purchase

## Problem Statement
The Management team at Walmart Inc. wants to analyze the customer purchase behavior (specifically, purchase amount) against the customer’s gender and the various other factors to help the business make better decisions. They want to understand if the spending habits differ between male and female customers: Do women spend more on Black Friday than men? (Assume 50 million customers are male and 50 million are female).

## Data Schema (ERD)
* Tables: walmart_data
* Total Records: 550,068

![alt text](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/erd/erd.png)

## Executive Summary
This Black Friday sample confirms that male customers spend more per transaction than female customers, and the 95% confidence intervals do not overlap, so the difference is statistically meaningful. The largest value comes from the 26-35 and 36-45 age groups, while marital status and city category show smaller differences. Product categories are highly skewed, meaning some categories drive a disproportionate share of revenue.

## Insights
* P(Premium Spend | Male) is materially higher than P(Premium Spend | Female), so gender is a strong routing signal for premium offers.
* P(Premium Spend | Married) is almost the same as P(Premium Spend | Unmarried), so marital status should not be used as a targeting lever.
* High spend is concentrated in a few age brackets and city categories, giving Walmart clear segments to prioritize.

## Recommendations
* Prioritize male-led premium campaigns. Use the gender confidence interval gap to justify higher investment in male-targeted Black Friday and high-ticket product ads.
* Target the 26-50 age bracket. This group shows the highest AOV and revenue contribution; tailor creative and inventory to their preferences.
* Stop over-investing on marital status. It does not differentiate spend; redirect that budget to gender and age signals.
* Use the CLT intervals for budget sizing. The 95% CIs give a reliable range for expected average spend per segment; set ROI thresholds and daily spend caps around the lower bound of the interval to protect margin.
* Focus product mix on the top revenue categories. Move inventory and promotional visibility toward the categories that already produce the most revenue per transaction.
* Run a two-question qualifier at checkout/online: "Gender + Age group" can estimate expected spend and trigger personalized upsell recommendations.

## Limitations
The analysis is based on one Black Friday sample and assumes spend patterns are stable. Purchase amount is the only revenue proxy; margin and profitability are not included. Confidence intervals are sample-based and should be refreshed with new data.

## Visualisations

![Chart 1](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_1.jpg)
![Chart Age Counts](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_Age_counts.jpg)
![Chart City Category Counts](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_City_Category_counts.jpg)
![Chart Gender Counts](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_Gender_counts.jpg)
![Chart Marital Status Counts](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_Marital_Status_counts.jpg)
![Chart Aov](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_aov.jpg)
![Chart Heatmap](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_heatmap.jpg)
![Chart Purchase By Age](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_purchase_by_Age.jpg)
![Chart Purchase By City Category](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_purchase_by_City_Category.jpg)
![Chart Purchase By Gender](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_purchase_by_Gender.jpg)
![Chart Purchase By Marital Status](https://github.com/codehithesh/Black-Friday-Customer-Spend-Analysis/blob/main/charts/chart_purchase_by_Marital_Status.jpg)