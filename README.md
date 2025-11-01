# Data Analysis of all deaths to Wandsworth residents registered in 2016 (Interactive Dashboard created using PowerBI)
## Project Objective
Wandsworth, a district in southwest of London, wants to analysis the death roll of its residents registered in the year 2016 in order to discover the impact across its wards and gender and to know the cause of the majority of the deaths.

## Dataset used 
- <a href="https://github.com/Obabtd/My_Project_Work/blob/main/Wandsworth%20county%20Data.xlsx">Dataset</a>

## Questions (KPIs) 
- What are the number of deaths per month
- What is the death rate (calculated per 100,000 population) per ward
- What are the leading underlying causes of death
- How does the death rates varied by age and sex
- Which month saw the most registered deaths and how many were there
- Which ward had the highest death rate and what was it?
- What is the leading underlying cause of death in males and what is the leading underlying cause of death in females?
- What percentage of deaths in females occurred in the 80+ age groups and how does this compare to males?

## Dashboard Interaction 
- <a href="https://github.com/Obabtd/My_Project_Work/blob/main/WWC%20Dashboard.png">View Dashboard</a>

## Process
- Verify data for any missing values and anomalies, and sort out the same.
  
After loading the Excel sheets into the PowerBI using Get data button, I used the power query to
clean and transform the data in the Excel sheets by clicking on the Transform data button.
I was able to clean and transform the data in the tables by promoting the first row into the header of the columns in the table using the Use First Row as Headers button under the Transform pane so that each column heading can uniquely standout in the table.

- Ensured data is consistent and clean with respect to data type, data format and values used

On DATA_2016 table, I then use the split columns by delimiter to extract the months in words from the month of death registration column into another column and renamed the new column as the month of death registration and deleted the former column in order to assign numbers to the month in a way that PowerBI will be able to identify and use the month data for analysis. 
On the POPULATION_2016 table, I used the unpivoted column in the Transform pane to create a new column that match the ward code to the ward name. Then, I used the split columns by delimiter to separate the ward codes and the ward names into two different columns then renamed the columns for easy analysis on PowerBI.

- Create Pivot tables according to the predetermined KPIs

On the POPULATION_2016 table, I used the conditional column to convert the age column into age group column just similar to the age group column in DATA_2016 table.
Using the Pivot table, I grouped the row data according to the table columns in order to generate the total population of people in Wandsworth.

- Build a dashboard for data visualisation and apply slicer to make dynamics
  
Using the data model view window in PowerBI, I was able to established the relationships between the tables and analyse the tables using DAX in PowerBI. 

## Answers to KPIs
- Q1. Which month saw the most registered deaths and how many were there?

The report shows that the month of January has the month with the most registered deaths and the
number of deaths registered was 182

- Q2. Which ward had the highest death rate and what was it?

The ward E05000622 referred to as St Mary’s Park has the highest death rate of 140

- Q3. What is the leading underlying cause of death in males and what is the leading underlying
cause of death in females?

As indicated in the report, the leading underlying cause of death in males is Chronic ischaemic heart
disease with a record of 68 cases while in female the leading underlying cause of death is
Unspecified dementia with a record of 45 cases.

- Q4. What percentage of deaths in females occurred in the 80+ age groups and how does this
compare to males?

The percentage of deaths in female that occurred in the 80+ age group is 459 which is about 60.08%
of the total death that occurred in this age group and it is about 50.5% increase to that of death in
male which is at total of 305. The total death that occurred in this age group is 764

