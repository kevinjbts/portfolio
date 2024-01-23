# Kevin Bates - Data & Strategy Professional

I'm a trusted advisor for any organization I'm apart of. With a decade of experience with a focus on launching new ventures, advising on operational and marketing campaigns, and developing sustainable strategy. I'm most engaged in working on impactful projects in uncovered oceans. Previous experiences include capital raising for early-stage companies, launching equity-crowdfunding campaigns in a brand new industry, and supporting a data team with BI & investor relations support. 

www.linkedin.com/in/kevinjbts

## My Experience
- Innovatio Program Manager @ McKesson
- [Dates]
- Supported Fortune 10 Corporate Strategy Team on piloting enterprise-wide growth pilots that leveraged AI & Data capabilities.

-Business Intelligence & Investor Relations Analyst @ Streamlytics
-Supported competitive intelligence and marketing strategy for a ethical data company leveraging millions of data points. 

-Account Executive / Digital Strategist @ Digital Niche Agency
-Worked with 125+ clients to prepare user and investor acquisition strategies acting as lead strategist. 

-Analyst & Engagement Manager @ Growthink
-Support Strategic Advisory and Investment Banking for forward looking entrepreneurs and executives. 

## Education
-Bachelor's of Business Administration (Entrepreneurship) | Loyola Marymount University

## Certifications
-Google Data Analyst | Coursera (Key Courses Included: PowerBI, Tableau, Data Cleaning, Machine Learning)

# Projects
## AirBnB Tableau Visualization
![](/AirBnbTableau.png)

Utilizing data from zeroAirBnB data from SeattleWashington, the visualization provides insight into potential opportunity for key metrics for a friend deciding whether or not to enter the AirBnB business. 
The full visualization native in Tableau can be found here: 

https://public.tableau.com/views/AirBnBDataSampleDashboard/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link

Key insights include the following: 

## Covid Tableau Visualization
![](/CovidDdata.png)

Utilized WHO data to clean, join, and visualize visualization of Covid Data, with props to Alex the Analyst for his walk-through tutorial. 
The full visualization native in tableau can be found here: 
https://public.tableau.com/views/CovidDataSampleDashboard/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link
Key insights include the following: 
--SELECT  * 

--FROM still-primer-356101.coviddeaths.coviddeaths 

--ORDER BY 3,4

--SELECT  * 

--FROM still-primer-356101.coviddeaths.covidvaccinations 

--ORDER BY 3,4

--Select the Data we will be using for the project: 

SELECT  location, date, total_cases, new_cases, total_deaths, population

FROM still-primer-356101.coviddeaths.coviddeaths 

ORDER BY 1,2

-- Looking at Total Cases vs Total Deaths

-- Shows likelihood of dying if you contract covid in your country

SELECT  location, date, total_cases, total_deaths, (total_deaths/total_cases)*100 AS DeathPercentage

FROM still-primer-356101.coviddeaths.coviddeaths

WHERE location = 'United States'

ORDER BY 1,2

--Looking at total cases vs. the population

--Shows what percentage of population got Covid

SELECT  location, date, population, total_cases, (total_cases/population)*100 AS InfectionPercentagePopulution

FROM still-primer-356101.coviddeaths.coviddeaths

--WHERE location = 'United States'

ORDER BY 1,2

--Looking at countries with the highest infection rate paired to population

SELECT  location, population, MAX(total_cases) AS HighestInfectionCount, (MAX(total_cases/population))*100 AS InfectionPercentagePopulation

FROM still-primer-356101.coviddeaths.coviddeaths

--WHERE location = 'United States'

GROUP BY location, population

ORDER BY InfectionPercentagePopulation DESC

-- Showing Countries with Highest Death Count per Population

SELECT  location, MAX(cast(total_deaths as int)) AS TotalDeathCount

FROM still-primer-356101.coviddeaths.coviddeaths

--WHERE location = 'United States'

WHERE continent IS NOT NULL

GROUP BY location, population

ORDER BY TotalDeathCount DES

## Sales Data Example
![](/bikesales.png)

As part of the CFI BIDA certification, the data below provides sample data set of visualizing key metrics for sales metrics for a fictional company, CalWest. 
The full visualization native in tableau can be found here: 
https://public.tableau.com/views/Test1_16856628787760/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link
Key insights include the following: 

## Sales Dashboard Example
![](/CovidDdata.png)

Utilizing data from zeroAirBnB data from SeattleWashington, the visualization provides insight into potential opportunity for key metrics for a friend deciding whether or not to enter the AirBnB business. 
The full visualization native in Tableau can be found here: 

https://public.tableau.com/views/AirBnBDataSampleDashboard/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link

Key insights include the following: 


