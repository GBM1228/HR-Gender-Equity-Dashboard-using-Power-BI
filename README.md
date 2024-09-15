# PwC Switzerland Power BI Job Simulation on Forage-Diversity and Inclusion Analysis

<img width="686" alt="2024-09-08 (31)" src="https://github.com/user-attachments/assets/dd570077-b1be-405c-b3f3-dd47fc1d346f">


## About This Project

As part of my 4th and final task for the Virtual Internship on Power BI from PwC, offered by Forage, I have developed a dashboard focused on Diversity & Inclusion. As a Data Analyst, my role was to define relevant KPIs in areas such as hiring, promotion, performance, and turnover,create visualizations to effectively communicate these insights and Write what i think some root causes of their slow progress might be.

## Table Of Contents

[Problem Statement](#ProblemStatement)

[Data Sourcing](#DataSourcing)

[Data Preparation](#DataPreparation)

[Data Preparation](#DataPreparation)

[Data Visualization](#DataVisualization)

[Data Analysis](#DataAnalysis)

[Insights](#Insights)

[Recommendation](#Recommendation)


## Problem Statement

The purpose of this analysis is to:

1.Define relevant KPIs in hiring, promotion, performance and turnover, and create a visualisation

2.Write what you think some root causes of their slow progress might be

## Data Sourcing

The Dataset used for this analysis was given by [Pwc switzerland](https://www.pwc.ch/en/careers-with-pwc/students/virtual-case-experience.html)

[Dataset](https://github.com/GBM1228/HR-Gender-Equity-Dashboard-using-Power-BI/blob/main/03%20Diversity-Inclusion-Dataset.xlsx)

## Data Preparation
Data transformation was performed using Power Query, followed by loading the refined dataset into Microsoft Power BI Desktop for in-depth analysis and reporting.

The dataset for diversity and inclusion has 32 columns and 500 rows.

The tabulation below shows the dataset table with its column names and their description:

|Column Name|Description|
|---|---|
|Employee ID	|The unique indentity number of the employee in the dataset|
|Gender|The gender of the employee|
|Job Level after FY20 promotions|	Describes the job level of the employee after being promoted in FY20|
|New hire FY20?|	Describes if the employee is a new hire in FY20|
|FY20 Performance Rating|	Represents the performance rating of the employee in FY20|
|Promotion in FY21?|	Describes if the employee is being promoted in FY21|
|In base group for Promotion FY21|	Describes if the employee is being selected for promoted in FY21|
|Target hire balance|	Describes the target hire balance of the employee|
|FY20 leaver?|	Describes if the employee is a leaver in FY20|
|In base group for turnover FY20|	Describes if the employee is in a group for turnover in FY20|
|Department @01.07.2020|	Describes the department each employee belongs to as at January 7, 2020|
|Leaver FY|	Describes if the employee is a leaver in a FY|
|Job Level after FY21 promotions|	Describes the job level of the employee after being promoted in FY21|
|Last Department in FY20|	Describes the last department each employee belongs in FY20|
|FTE group|	Describes if the employee belongs to a FTE group|
|Time type|	Describes the contract type employee|
|Department & JL group PRA status|	Describes the department and JL group PRA status of the employee|
|Department & JL group for PRA|	Describes the department and JL group PRA of the employee|
|Job Level group PRA status|	Describes the job level group PRA status of the employee|
|Job Level group for PRA|	Describes the job level group PRA of the employee|
|Time in Job Level @01.07.2020|	Describes the time in job level of the employee|
|Job Level before FY20 promotions|	Describes the job level employee before being promoted in FY20|
|Promotion in FY20?|	Describes if the employee is being promoted in FY20|
|FY19 Performance Rating|	Describes the performance rating of the employee in FY19|
|Age group|	Describes the age group of the employee|
|Age @01.07.2020|	Represents the age of the employee as at January 07, 2020|
|Nationality 1|	Describes the nationality of the employee in state level|
|Region group: nationality 1|	Describes the nationality of the employee in country level|
|Broad region group: nationality 1|	Describes the nationality of the employee in regional level|
|Last hire date|	Describes the last hire date of the employee|
|Years since last hire|	Represents the number of years since last hire of the employee|
|Rand|	Generates random number for each entry in the dataset|
