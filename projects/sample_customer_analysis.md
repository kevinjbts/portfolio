---
layout: default
title: Data Cleaning & Manipulation with Visualization in Tableau
description: Utilizing Tableau & Python
--- 
# Background and Overview

This project seeks to leverage Exploratory Data Analysis including visualization, feature analysis, and basic aggregations. As a small company, NEWCO is looking for where best to allocate future marketing dollars to see overindexed return on advertising spend. Analyzing the 12-month sales data (synthetic generated data) provides a solution for guiding future marketing tests towards this end. In addition to Python EDA, Tableau has been utilized to view location & customer data for Sales Representatives to contact, and/or create custom lists for promotion geared towards new sales.  

![Image](https://github.com/user-attachments/assets/c781838d-f43b-40be-bcb1-e1e704638183)

See the full Tableau visualization [here](https://public.tableau.com/app/profile/kevin.bates3947/viz/SampleCustomerAnalysis_17175511318920/Dashboard)

# Data Structure Overview
The dataset contains 8 features and 500 observations. The 8 features include string, integer and categorical data types. 

# Executive Summary 
As a Data Analyst & Strategist tasked with providng reccomendations to NEWCO's founder, the EDA on current e-commerce sales resulted in a relevant action plan that can be iterated in the future. From the analysis, the top 10 States by Sales Volume represented $30k in sales, while also having an evenly distributed number of customers (no outliers). Because of this, allocating higher advertising towards these regions should be tested for improved ROAS vs. underperforming states. 

In addition to adjusting advertising targeting, the Sales Analysis creates segmentation of the top 20% of purchasers for the company, representing a highly engaged audience for customized marketing campaigns and / or for sales reps. 

Lastly, the insights able to be generated are limited by the features and current dataset. Future customer surveys and / or data collection can be leveraged to offer new opportunities to analyze performance, while further guiding advertising targeting. 

# Insights Deep Dive

View the full Python EDA in Jupyter Notebook [here:](Sales_Analysis.ipynb)

### Key Performance Indicators: 
* Mean purchase amount was $2,500
* Minimum purchase amount: $9
* Maximum purchase amount: $4,992
* 20th percentile: $1,082
* 80th percentile: $3,950
* Total Sales: $1,250,143

### Analyzing Sales Volume by Categories
Seasonality doesn't play a factor as sales volume is relatively even across seasons.
![Image](https://github.com/user-attachments/assets/785b2363-f8cd-41d4-ab4b-3c08ac646232)

Promotional activity also doesn't affect sales volume as it is evenly distributed: 

![Image](https://github.com/user-attachments/assets/36572a4a-99f6-4cb5-968a-dfa50adc15b6)


However, region affects sales performance, with 3 regions leading total sales volume: 

![Image](https://github.com/user-attachments/assets/da5787f0-bf60-487f-b2c5-ca1e40679104)


Given these factors, the Python file creates a list of customers above the 80th percentile, representing highest purchasers. 

Additionally, the top 10 states all have above 30k in sales revenue, while not having outliers in terms of total number of customers, representing best advertising targets for future tests. 

![Image](https://github.com/user-attachments/assets/e42038f2-8e72-4a1a-8c99-7f4da6cde041)


# Recommendations

To maximize return on advertising spend, Region & State are the best opportunities to focus future advertising spend on the best performers. 

The Top 10 States from this analysis each drove $30k in sales, and improved advertising in the states should be tested for higher ROI than other regions. 
* The current dataset does not include data on repeat customers, demographic data, or sales channel - all of which could be additional factors to investigate for additional marketing optimization. 
* Testing on our initial assumptions can be done in parallel with additional data collection. The recommendation to NEWCO would be to allocate a higher percentage of advertising spend towards the top 10 states, while also running promotional campaigns customer wide for surveys to collect additional data. This survey data can also be leveraged to guide brand marketing activities (outside of performance marketing). 
