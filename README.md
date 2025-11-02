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

## Data Interpretation
It can be deduced from the data that Wandsworth county has a total population of 321,500 people
out of which 155,110 are Males (which is 48.25% of the population) and 166,390 are Female (which
is 51.75% of the population) in essence we have more female than male in Wandsworth. In addition,
the data shows that St. Mary’s Park is the Ward with the highest population of 18,069 in all the 20
Wards that are in Wandsworth.

However, the report indicated that the total number of deaths recorded for the year 2016 in
Wandsworth is 1,508 and most of it happen in the month of January with a total of 182 deaths
recorded in January 2016. In the entire year, about 765 female deaths were recorded and 743 male
deaths were recorded in same year. Which means there were more female deaths than the male
deaths with a percentage difference of 2.96%. Most of these female deaths involve more of the
people within the age range of 75 years old to 90 years old while most of the deaths outside the age
brackets were male.

The report indicated that the leading underlying cause of the death in female was unspecified
dementia which claims the life of 45 females and it was chronic ischaemic heart disease for the male
counterpart which also claims the life of 68 males in the year under review. St. Mary’s Park ward had
the highest number of deaths for both male and female population while Northcote ward had the
least number of deaths for both sex in the entire Wandsworth county.

## Dashboard
<img width="1343" height="757" alt="WWC Dashboard" src="https://github.com/user-attachments/assets/3f653733-564c-458a-a7d6-ac64ffeaf849" />

## Conclusion
This report highlights the importance of Wandsworth county to engage in various campaign and awareness on quality lifestyle, medical and social services available for people to access in order to reduce the risk of dementia and chronic ischaemic heart disease with special focus on St. Mary’s Park ward and people within the age range of 75 years old to 90 years old. 
This awareness should include areas like:
- Managing stress and mental health
- Ensuring quality sleep
- Attending regular medical check-ups
- Staying socially connected
- Exercising regularly
Etc.
