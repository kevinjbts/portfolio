# MovieCorrelations
Alex The Analyst Portfolio Project with Movie Correlations

# Background and Overview

Leveraging a sample project by Alex the Analyst, utilized the IMDB Movie database to explore correlation between various features within the dataset against movie performance. The initial hypothesis is that movie votes and gross profit have a positive correlation. Utilized Python to clean and analyze data using key visualizations including regression, heatmaps and correlation matrixes. 

# Data Structure Overview
The dataset contains 16 features and 7668 observations. The 8 features include string, integer and categorical data types. To clean the dataset, the following steps were taken: 

- Check for Null Values
- Adjust Date Types for Features
- Drop Duplicates

# Executive Summary 
As a Data Analyst & Strategist tasked with providng reccomendations to NEWCO's founder, the EDA on current e-commerce sales resulted in a relevant action plan that can be iterated in the future. From the analysis, the top 10 States by Sales Volume represented $30k in sales, while also having an evenly distributed number of customers (no outliers). Because of this, allocating higher advertising towards these regions should be tested for improved ROAS vs. underperforming states. 

In addition to adjusting advertising targeting, the Sales Analysis creates segmentation of the top 20% of purchasers for the company, representing a highly engaged audience for customized marketing campaigns and / or for sales reps. 

Lastly, the insights able to be generated are limited by the features and current dataset. Future customer surveys and / or data collection can be leveraged to offer new opportunities to analyze performance, while further guiding advertising targeting. 

# Insights Deep Dive

View the full Python EDA in Jupyter Notebook [here:](Movie_Correlation_Analysis.ipynb)

### Key Performance Indicators: 
* Mean purchase amount was $2,500
* Minimum purchase amount: $9
* Maximum purchase amount: $4,992
* 20th percentile: $1,082
* 80th percentile: $3,950
* Total Sales: $1,250,143

### Analyzing Sales Volume by Categories
Seasonality doesn't play a factor as sales volume is relatively even across seasons.

![Image](https://github.com/user-attachments/assets/97f117e8-4dab-4163-a8a4-53a0d7699b36)

Promotional activity also doesn't affect sales volume as it is evenly distributed: 

![Image](https://github.com/user-attachments/assets/f79263e4-7476-470e-b0bd-319db4cfdb92)

However, region affects sales performance, with 3 regions leading total sales volume: 


![Image](https://github.com/user-attachments/assets/0fae30d3-ce76-421b-ad9f-02b8af39c52f)

Given these factors, the Python file creates a list of customers above the 80th percentile, representing highest purchasers. 

![Image](https://github.com/user-attachments/assets/2bb825e2-4cb5-4253-b0a6-86f582787b6c)

Additionally, the top 10 states all have above 30k in sales revenue, while not having outliers in terms of total number of customers, representing best advertising targets for future tests. 

# Recommendations

To maximize return on advertising spend, Region & State are the best opportunities to focus future advertising spend on the best performers. 

The Top 10 States from this analysis each drove $30k in sales, and improved advertising in the states should be tested for higher ROI than other regions. 
* The current dataset does not include data on repeat customers, demographic data, or sales channel - all of which could be additional factors to investigate for additional marketing optimization. 
* Testing on our initial assumptions can be done in parallel with additional data collection. The recommendation to NEWCO would be to allocate a higher percentage of advertising spend towards the top 10 states, while also running promotional campaigns customer wide for surveys to collect additional data. This survey data can also be leveraged to guide brand marketing activities (outside of performance marketing). 
