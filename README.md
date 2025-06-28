# Capstone Project: Mind the Gap: Exploring Gaps in Medicaid Coverage in the United States

## Overview
Using income and population data from the U.S. Census Bureau alongside County Enrollment Percentage data, this project explores Medicaid enrollment in the 
United State at the State and County Level.  Enrollment gap scores are calculated to estimate potential unutilized resources based on expected eligibility.  Insights are offered into the findings based on gap scores and revelations of current enrollment, as well as the indications of certain factors like gap score and enrollment percentage vs. total population related to population density and those who will be affected by changes to the Medicaid program.

## Datasets
- Primary Dataset: https://data.census.gov/
- Supplemental Dataset: https://data.medicaid.gov/datasets; https://ccf.georgetown.edu/2025/02/06/medicaid-coverage-by-county-2023/

## Key Questions
- Q1: Which States/Counties have the highest amount of Medicaid enrollees?
- Q2: Which regions have the highest number of eligible non-enrollees based on current Medicaid enrollment criteria?
- Q3: What factors contribute to gaps in enrollment, indicated by calculated gap scores?

## Tools Used
Python, Pandas, Matplotlib (visuals), Seaborn (visuals), Glob (data consolidation), Excel, Tableau

## Methodology
- Data Cleaning
	County data combined from 51 separate files into one csv for analysis.  Regions for which data was incomplete (Puerto Rico) were removed from 
analysis.  Census income and population data aggregated to form age groups to match Medicaid enrollment criteria (ex: residents 19 years and younger combined to form Child group; residents 65 years and older combined to form Senior group; remaining combined to form Adult group).  

- EDA
	Gap scores calculated by age group (population eligible - population enrolled); income-based Adult groupings calculated based on individual state income thresholds.  

- Visualizations
	Top 5 State enrollment gaps; Gap scores by enrollment population (Child, Adult, Senior); Top 5 county enrollment gaps; Regional population counts for Child, Adult, Senior population groups; Areas of highest enrollment; Areas with largest gap scores; Eligibility group breakdown for regions with largest gap scores; Regions of highest enrollment vs. total population; 

- Summary
	Regions with highest enrollment gaps based on raw population tend to encompass large urban centers.  Regions with the highest number of enrollees vs. total population were generally more rural.  Negative gap scores emerged from gap score calculations; Due to unavailabilty of data on Medicaid enrollment due to disability, this group was not represented during calculations, but was revealed in negative gap scores.  


## Visuals
https://public.tableau.com/app/profile/michael.shaffer5706/viz/Medicaid_Map_Capstone/MedcaidCountyDashboard?publish=yes

## Contact
Michael Shaffer • ekimshaf@gmail.com • https://www.linkedin.com/in/michael-j-shaffer/