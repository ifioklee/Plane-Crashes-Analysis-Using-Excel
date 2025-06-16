# <p align="center" style="margin-top: 0px;">  Plane-Crashes-Analysis-Using-Excel
# Project Overview
This repository contains a dashboard creating from analyzing 5,268 plane crash data from 1908 - 2009 using Microsoft Excel. It provides insigght into the number of aircraft crashes that has occured in 101 years, explores patterns relating to fatalities as a result of these incidents.

# Goal
Plane crashes have been happenening for over a hundred years since it invention by Wright brothers in 1903, on hearing the news of Air India crash involving a 12 year old Boeing 787 aircraft on Thurday 12th June 2025, I wanted to explore data aroud this occurance, provide insight into and analyse patterns relating to plane crashes. 
The main objective was to create a dashboard that will provide information about these insights and patterns by answering the following questions:

1. What are the total number of passengers who have been onboard planes that crashed from 1908 - 2009?

2. What are the number of passengers fatalities, that is number of passengers who died during plane craches in this time frame?

3. How many passengers survived plane crashes in this time frame?

4. What were the top 5 years with the highest plane crashes?

# Features
- Chart visulaizaations for showing parttern of total number of plane crashes, total number of fatalities and total number of survivors in the time frame under  investigation.
- A dashboard showing an overview of insights and pattern as a result of analytic process carried out on data.
- Pivot tables used in creating chart visulizations.
- Cleaned dataset that serve as basis for creating pivot tables, chart visulizations, mathematical calculations and dashboard.

# Data
This project uses data on plane crashes downloaded from open source platform [Kaggle](https://www.kaggle.com/datasets/imtkaggleteam/airplane-crashes) spanning from 1908-2009. Data includes date, time, location, operator, flight number, route, type, registration, number aboard, fatalities, summary of cause of plane crash.

# Project Structure
/Raw data/ [Raw dataset](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/blob/main/Raw%20Data%20for%20Airplane%20Crashes) and [Processed dataset](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/blob/main/Processed%20Dataset%20Airplane%20Crashes%20and%20Fatalities_Since_1908_w.xlsx)

/Visulizations/ [Chart visulization for different metrics](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/tree/main/Visualization)

/Dashboard/ [Dashboard created with Excel](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/tree/main/Dashboard)

README.md Project verview and instructions


# Technical Details
This project used Excel for both manipulation and dashbord visulizations. Key challengges included cleaning of inconsitent values for both number of passengers onboard and number of fatalities. In a bid to get filling missing data for number of passengers onboard and number of fatality, an external website, [planecrashinfo](http://planecrashinfo.com/) was used to find and replace missing data and where the data was not found such row was deleted from the dataset.

Another challenge encountered during this project was not been able to identify the causes of majority of these plane crashes. This is because the dataset contains a column called "summary" which gave in a sentence what the might have caused these aircraft to crash, it would have easier to create clusters for these responses if it were not a large dataset.

A new column was created within the dataset named "Survivors" which data input was the number of passengers that survivors each crash, it was computed by finding the difference between the number of passengers onboard and the number of fatalities.

Calculations to obatain the _Total number of passengers onboarded_, _Total number of passengers fatalities_ and _Total number of survivivors_ was computed using the mathematical sum fuction in Excel across all values in the _Onboard_, _Fatalities_, and _Survivor_ column respectively.

Pivot tables (PVT1, PVT2, and PVT3) as seen in the [Proccessed dataset](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/blob/main/Processed%20Dataset%20Airplane%20Crashes%20and%20Fatalities_Since_1908_w.xlsx) were used in creating chart visulizations.

- PVT1: This Pivot table was used to create the visulization for the [number of plane crash per year](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/blob/main/Visualization/Number%20of%20plane%20crash%20per%20year.jpg).
- PVT2: This Pivot table was used to create the visulization for the [years with highest number of plane crash](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/blob/main/Visualization/Years%20with%20highest%20number%20of%20plane%20crash.jpg)
- PV3: This Pivot table was used to create visulization for the [number of passengers onborded per year](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/blob/main/Visualization/Number%20of%20passengers%20onbosrd%20per%20year.jpg), [number of fatalities per year](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/blob/main/Visualization/Number%20of%20fatalities%20per%20year.jpg) and [number of survivors per year](https://github.com/ifioklee/Plane-Crashes-Analysis-Using-Excel/blob/main/Visualization/Number%20of%20survivors%20per%20year.jpg)

# Results and Insights 

- 144,624 passengers have boarded planes that have crashed from 1908 - 2009.

- 105,431 which represents 72.9% of passengers onboard these aircrafts in this time frame suffered casualties.

- 39,193 which is 27.1% of passengers onboard these aircrafts between 1908 - 2009 have survived.

- 1972, 1968, 1989, 1967, 1979, 1973 represents the years with highest number of plane crashes recorded.

# Future Work
#### Potential improvements 
- Find a way to work on the "summary" column to find causes of plane crashes from the dataset.

# References and Resources
- [Dataset for plane crash from 1908 - 2009 from Kaggle](https://www.kaggle.com/datasets/imtkaggleteam/airplane-crashes)
- [Plancrashinfo website](https://www.planecrashinfo.com/) for finding and replacing missing data.
