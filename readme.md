# Professional Summary
Kevin Bates is passionate about uncovering data-driven insights and leveraging them to create meaningful long-term growth for businesses. Kevin has helped launch new ventures, guided strategy for operations and marketing campaigns, and provided analytics and investor relations support. If you are looking for someone to bring a holistic perspective on business intelligence and strategy, let's connect and explore how to contribute to your organization's success. [Let's connect on LinkedIn!](www.linkedin.com/in/kevinjbts)

# Links to Projects 
* [Sales Dashboard Example](#sales-dashboard-example) 
* [Sales Data Example](#sales-data-example)
* [Covid Tableau Visualization](#covid-tableau-visualization)
* [AirBnB Tableau Visualization](#airbnb-tableau-visualization)

## Experience
* Innovation Program Manager, * *McKesson* *
* Business Intelligence Manager, * *Streamlytics* *
* Digital Strategist, * *Digital Niche Agency* *
* Engagement Manager, * *Growthink* *

## Education
* Bachelor's of Business Administration, Entrepreneurship **Loyola Marymount University**

## Certifications
* Google Data Analyst, Coursera (Key Courses Included: PowerBI, Tableau, Data Cleaning and Machine Learning)

# Projects
## [AirBnB Tableau Visualization](/projects/airbnb_tableau_visualization)
![](/AirBnbTableau.png)

Utilizing data from zeroAirBnB data from SeattleWashington, the visualization provides insight into potential opportunity for key metrics for a friend deciding whether or not to enter the AirBnB business. 
The full visualization native in Tableau can be found here: 

[Full Tableau Visualization Available Here](https://public.tableau.com/views/AirBnBDataSampleDashboard/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link)

Key insights include the following: 

## [Covid Tableau Visualization](/projects/covid_visualization.md)

![](/CovidDdata.png)

#### Summary

Utilized WHO data to clean, join, and visualize visualization of Covid Data, with props to Alex the Analyst for his walk-through tutorial. 
[Full version in Tableau Public] (https://public.tableau.com/views/CovidDataSampleDashboard/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link)

Key insights include the following: 

```
SELECT  * 
FROM still-primer-356101.coviddeaths.coviddeaths 
ORDER BY 3,4
```

Testing another section with a code block:

```
SELECT  * 
FROM still-primer-356101.coviddeaths.covidvaccinations 
ORDER BY 3,4
```

#####Select the Data we will be using for the project: 

```
SELECT  location, date, total_cases, new_cases, total_deaths, population
FROM still-primer-356101.coviddeaths.coviddeaths 
ORDER BY 1,2
```

Looking at Total Cases vs Total Deaths
Shows likelihood of dying if you contract covid in your country

```
SELECT  location, date, total_cases, total_deaths, (total_deaths/total_cases)*100 AS DeathPercentage
FROM still-primer-356101.coviddeaths.coviddeaths
WHERE location = 'United States'
ORDER BY 1,2
```

Looking at total cases vs. the population
Shows what percentage of population got Covid

```
SELECT  location, date, population, total_cases, (total_cases/population)*100 AS InfectionPercentagePopulution
FROM still-primer-356101.coviddeaths.coviddeaths
WHERE location = 'United States'
ORDER BY 1,2
```

Looking at countries with the highest infection rate paired to population

```
SELECT  location, population, MAX(total_cases) AS HighestInfectionCount, (MAX(total_cases/population))*100 AS InfectionPercentagePopulation
FROM still-primer-356101.coviddeaths.coviddeaths
WHERE location = 'United States'
GROUP BY location, population
ORDER BY InfectionPercentagePopulation DESC
```

Showing Countries with Highest Death Count per Population

```
SELECT  location, MAX(cast(total_deaths as int)) AS TotalDeathCount
FROM still-primer-356101.coviddeaths.coviddeaths
WHERE location = 'United States'
WHERE continent IS NOT NULL
GROUP BY location, population
ORDER BY TotalDeathCount DES
```

## Sales Data Example
![](/bikesales.png)

As part of the CFI BIDA certification, the data below provides sample data set of visualizing key metrics for sales metrics for a fictional company, CalWest.  
[Full Tableau Public Visual provided Here](https://public.tableau.com/views/Test1_16856628787760/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link)

...insights to be added
## Sales Dashboard Example
![](/CovidDdata.png)

Utilizing data from zeroAirBnB data from SeattleWashington, the visualization provides insight into potential opportunity for key metrics for a friend deciding whether or not to enter the AirBnB business. 
The full visualization native in Tableau can be found here: 

[https://public.tableau.com/views/AirBnBDataSampleDashboard/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link
](url)

...insights to be added


