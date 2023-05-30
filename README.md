# SQL-Data-Exploration
The provided code performs data exploration and analysis on Covid-19 data using various SQL techniques and functions. Here is a breakdown of the different parts of the code:

Selecting Covid-19 data:

The code retrieves data from the "CovidDeaths" table in the "Data Exploration" database.
It selects specific columns related to location, date, total cases, new cases, total deaths, and population.
The data is filtered to exclude records where the continent is null and is ordered by location and date.
Analyzing Covid-19 statistics:

The code calculates the death percentage based on total cases and total deaths for locations containing the word "states."
It also calculates the percentage of the population infected with Covid-19 based on total cases and population.
The results are ordered by location and date.
Identifying countries with the highest infection rate and death count:

The code identifies countries with the highest infection count compared to their population.
It also identifies countries with the highest death count per population.
The results are grouped by location or continent and ordered accordingly.
Examining global numbers:

The code provides global statistics by summing the new cases and new deaths.
It calculates the death percentage based on the total deaths and new cases.
The results are ordered by the total number of cases and deaths.
Analyzing population and vaccination data:

The code retrieves data from the "CovidDeaths" and "CovidVaccinations" tables.
It performs a join operation on location and date columns.
The code calculates the rolling number of people vaccinated and the percentage of the population vaccinated.
The results are ordered by location and date.
Using CTE and temporary table:

The code demonstrates two alternative approaches for calculating the percentage of the population vaccinated.
It uses a Common Table Expression (CTE) and a temporary table to store intermediate results.
The final query retrieves data from the CTE or temporary table and calculates the percentage of the population vaccinated.
Creating a view:

The code creates a view called "PercentPopulationVaccinated" to store the data for later visualizations.
The view incorporates the logic used in the previous queries.
Overall, the code combines different SQL techniques such as joins, CTEs, temp tables, window functions, aggregate functions, and creating views to explore and analyze Covid-19 data, focusing on various aspects such as cases, deaths, population, and vaccinations.
