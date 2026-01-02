# IMDB Movie Feature Correlation

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
* Highest Correlated features: votes vs. gross earnings: .63
* votes & budget, 0.44

### Analyzing Sales Volume by Categories
Based on a basic regression, there is a positive correlation between gross profit and total movie budget. 

![Image](https://github.com/user-attachments/assets/97f117e8-4dab-4163-a8a4-53a0d7699b36)

After developing a heatmap of features within the IMDB database, movie votes and gross profit seem to be correlated (.63) as well as gross profit and movie budget (0.74) which further supports the previous analysis. 

![Image](https://github.com/user-attachments/assets/f79263e4-7476-470e-b0bd-319db4cfdb92)

This is further expanded when all features are leveraged, and the same features rise to the surface as the top correlated features. 

![Image](https://github.com/user-attachments/assets/0fae30d3-ce76-421b-ad9f-02b8af39c52f)

When more specifically charting gross earnings vs. budget, we see the positive correlation. 

![Image](https://github.com/user-attachments/assets/2bb825e2-4cb5-4253-b0a6-86f582787b6c)

Based on a few various visualizations, it is clear that Gross Earnings and Budget are heavily correlated. 

# Recommendations

While at a larger level, gross earnings are highly correlated to budget, it would be interesting to also look into movies which over-indexed on gross earnings below a budget threshold. If we know that high budget movies tend to perform well, seeing any correlation between movies that had lower budgets but over-indexed on earnings might help to show how to create higher-earning movies without the expansive budgets necessary. Or for smaller producers looking at trends that can help them to over-perform with their films. 
