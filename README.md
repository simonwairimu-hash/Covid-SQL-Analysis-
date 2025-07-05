# 🦠 COVID-19 Data Exploration & Tableau Visualization
This project showcases my ability to clean, analyze, and extract insights from global COVID-19 data using SQL, and to visualize the results using Tableau dashboards. The analysis focuses on understanding infection rates, mortality rates, vaccination progress, and the overall global impact of the pandemic.

# 📊 Project Overview
Objective:
To explore COVID-19 data using SQL and create meaningful, interactive visualizations in Tableau to support data-driven decision-making.

# Key Tasks:

✅ Cleaning and transforming raw COVID-19 datasets

✅ Performing exploratory SQL analysis to answer critical questions

✅ Calculating death rates, infection percentages, and vaccination rates

✅ Identifying countries/regions most affected by the pandemic

✅ Preparing datasets for Tableau dashboard development

## 📁 Data Sources
COVID-19 Deaths Dataset: Global daily reported cases, deaths, and population by location

COVID-19 Vaccinations Dataset: Global vaccination progress by location

Note: Data originally obtained from publicly available sources (e.g., Our World in Data).

## 🛠️ Tools & Technologies
SQL Server Management Studio (SSMS) — Data exploration and analysis

SQL Window Functions & CTEs — For cumulative calculations

Tableau — For interactive dashboards and data storytelling

Data Cleaning & Casting — To ensure data types are consistent for calculations

## 🧩 SQL Queries Summary
The project includes well-structured SQL scripts to:

✔ Calculate global totals for cases, deaths, and death percentages

✔ Identify locations with the highest death counts excluding global aggregates

✔ Analyze infection rates as a percentage of population by location

✔ Track daily vaccination progress using window functions

✔ Prepare datasets optimized for Tableau visualizations

Example SQL Techniques Used:

# sql
**SELECT Location, Population, 
    MAX(total_cases) AS HighestInfectionCount,  
    MAX(total_cases/population) * 100 AS PercentPopulationInfected
FROM PORTFOLIOPROJECT..CovidDeaths$
GROUP BY Location, Population
ORDER BY PercentPopulationInfected DESC;*
## 📊 Tableau Dashboard Insights
Tableau Visualizations Include:

Global COVID-19 Infection and Death Rates

Top locations by death count and infection percentage

Vaccination progress trends over time

Interactive filters for exploring data by continent or country

Percent of population vaccinated visualizations

## 💡 Key Insights
Certain regions experienced disproportionately high infection or death rates relative to their population

Vaccination progress varied significantly by location

Data storytelling in Tableau enables stakeholders to explore global trends quickly and effectively
<a href="https://public.tableau.com/shared/3X4CDKJ49?:display_count=n&:origin=viz_share_link">Tableau Link</a>
