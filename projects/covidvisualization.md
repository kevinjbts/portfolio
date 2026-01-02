# Covid-Visualization
SQL &amp; Visualization

covid visualization data: 

---
title: SQL & Visualization Project with Covid Data
description: Using SQL to download then tableau to visualize key insights
---

![](/CovidDdata.png)

# Summary

Utilized WHO data to clean, join, and visualize visualization of Covid Data, with props to Alex the Analyst for his walk-through tutorial. 

# Link
[Full visualization available here](https://public.tableau.com/views/CovidDataSampleDashboard/Dashboard1?:language=en-US&:display_count=n&:origin=viz_share_link)

# Key Insights: 
1. Insight #1
2. Insight #2

# Full Code: 

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

