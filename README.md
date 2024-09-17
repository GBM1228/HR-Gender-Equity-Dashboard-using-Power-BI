# PwC Switzerland Power BI Job Simulation on Forage-Diversity and Inclusion Analysis

<img width="675" alt="2024-09-08 (31)" src="https://github.com/user-attachments/assets/7d62e247-c7ee-4d74-aeaa-3476e6d9fbd2">

## About This Project

As  my 4th and final task for the Virtual Internship on Power BI from PwC, offered by Forage, I have developed a dashboard focused on Diversity & Inclusion. As a Data Analyst, my role was to define relevant KPIs in areas such as hiring, promotion, performance, and turnover,create visualizations to effectively communicate these insights and Write what some root causes of their slow progress might be.

#

## Table Of Contents

[Problem Statement](#ProblemStatement)

[Data Sourcing](#DataSourcing)

[Data Preparation](#DataPreparation)

[Data Visualization](#DataVisualization)

[Data Analysis](#DataAnalysis)

[Insights](#Insights)

[Recommendation](#Recommendation)

#


## Problem Statement

The purpose of this analysis is to:

1.Define relevant KPIs in hiring, promotion, performance and turnover, and create a visualisation

2.Write what you think some root causes of their slow progress might be

#

## Data Sourcing

The Dataset used for this analysis was given by [Pwc switzerland](https://www.pwc.ch/en/careers-with-pwc/students/virtual-case-experience.html)

[Dataset](https://github.com/GBM1228/HR-Gender-Equity-Dashboard-using-Power-BI/blob/main/03%20Diversity-Inclusion-Dataset.xlsx)

#

## Data Preparation
Data transformation was performed using Power Query, followed by loading the refined dataset into Microsoft Power BI Desktop for in-depth analysis and reporting.

The dataset for diversity and inclusion has 32 columns and 500 rows.

The dataset is organized into the following table, with the corresponding column names

|Column Name|
|---|
|Employee ID	|
|Gender|
|Job Level after FY20 promotions|
|New hire FY20?|
|FY20 Performance Rating|
|Promotion in FY21?|
|In base group for Promotion FY21|
|Target hire balance|
|FY20 leaver?|
|In base group for turnover FY20|
|Department @01.07.2020|
|Leaver FY|	
|Job Level after FY21 promotions|
|Last Department in FY20|
|FTE group|
|Employement Type|
|Department & JL group PRA status|
|Department & JL group for PRA|
|Job Level group PRA status|
|Job Level group for PRA|
|Time in Job Level @01.07.2020|
|Job Level before FY20 promotions|
|Promotion in FY20?|
|FY19 Performance Rating|
|Age group|
|Age @01.07.2020|
|Nationality 1|
|Region group: nationality 1|
|Broad region group: nationality 1|
|Last hire date|
|Years since last hire|
|Rand|

The following steps were taking for the data cleaning and transformation  :

* Promoting headers 

* Changing data types

* Replacing text values 

* Removing unnecessary columns

* Renaming Column name for clarity

  #

## Data Visualization

The Diversity and Inclusion dataset was tittled (HR Gender Equity Dashboard) and visualized in three phases using Microsoft Power BI Desktop, resulting in a comprehensive and interactive dashboard:

##### Page1 (Employment Diversity) visulaizes the :

* Total Employees
* Total New Hire
* Employees By Gender%
* New Hire By Gender%
* Total employees by Department and Gender
* Total Employees by Employment type and Gender
* Total Attrition by Gender
* Total Retention by Gender
* Total Employees by Job Level and Gender

<img width="675" alt="2024-09-08 (31)" src="https://github.com/user-attachments/assets/65e54a10-a2be-4622-b94c-d7aaf3722a93">

##### Page2 (Perfomance Diversity) visulaizes the:
* Average Performance rating
* Average performance Rating, Total attrition, Total Retention by Gender
* Average Performance Rating and New Hire by Gender
* Average Performance Rating by Employment Type and Gender
* Average Performance Rating by Department and Gender
* Average Performance Rating by Job level and Gender

<img width="685" alt="2024-09-08 (32)" src="https://github.com/user-attachments/assets/05b33ec0-836f-474a-ab6b-9daff769b971">


##### Page3 (Promotion Diversity) visulaizes the :
* Total Promoted
* Total Not-Promoted
* Total Promoted, Total Not-Promoted, Total Attrition, Total Retention by Gender
* Total Promoted by Service Year and Gender
* Total Promoted by Department and Gender
* Total Promoted by Job Level and Gender
* Total Not-Promoted by Department and Gender
* Total Not-Promoted by Job Level and Gender

<img width="676" alt="2024-09-08 (33)" src="https://github.com/user-attachments/assets/c58e8911-aa8a-44dd-8db2-81a7ab9370e4">

#

## Data Analysis

The following measures were developed to assess the effectiveness of our diversity and inclusion initiatives:
* Total Employees = COUNTA('Pharma Group AG'[Employee ID])+0
* Total male = COUNTX(FILTER('Pharma Group AG', 'Pharma Group AG'[Gender] = "male"), 'Pharma Group AG'[Employee ID])+0
* Total Female = COUNTX(FILTER('Pharma Group AG', 'Pharma Group AG'[Gender] = "Female"), 'Pharma Group AG'[Employee ID])+0
* Total Attrition = COUNTX(FILTER('Pharma Group AG', 'Pharma Group AG'[FY20 leaver?] = "Yes"), 'Pharma Group AG'[Employee ID])+0
* Total Retention = COUNTX(FILTER('Pharma Group AG', 'Pharma Group AG'[FY20 leaver?] = "No"), 'Pharma Group AG'[Employee ID])+0
* Promoted = COUNTX(FILTER('Pharma Group AG', 'Pharma Group AG'[Promotion in FY20?] = "Promoted"), 'Pharma Group AG'[Employee ID])+0
* Not Promoted = COUNTX(FILTER('Pharma Group AG', 'Pharma Group AG'[Promotion in FY20?] = "Not Promoted"), 'Pharma Group AG'[Employee ID])+0
* New Hire = COUNTX(FILTER('Pharma Group AG', 'Pharma Group AG'[New hire FY20?] = "Yes"), 'Pharma Group AG'[Employee ID])+0
* % Male = DIVIDE([Total male],[Total Employees])+0
* % Female = DIVIDE([Total Female],[Total Employees])+0
* % Attrition = DIVIDE( [Total Attrition], [Total Employees])+0

  #

## Insights

#### According to the analyzed data

 ##### Page1 (Employment Diversity):

1. Gender Distribution: Out of 500 employees, 41% are female and 59% are male.

2. New Hires: 66 new employees were hired, with females making up 51.52% and males 48.48%.

3. Departmental Gender Distribution:
    - Operations: 100 females, 103 males
    - Sales & Marketing: 59 females, 109 males
    - Internal Services: 24 females, 48 males
    - Strategy: 4 females, 12 males
    - Finance: 6 females, 12 males
    - HR: 12 females, 5 males

4. Employment Type by Gender:
    - Full-time: 172 females, 293 males
    - Part-time: 33 females, 2 males

5. Attrition by Gender: Total attrition is 47, with 26 males and 21 females.

6. Retention by Gender: Total retention is 453, with 269 males and 184 females.

7. Job Level by Gender:
    - Junior Officer: 109 females, 95 males
    - Senior Officer: 49 females, 56 males
    - Manager: 30 females, 52 males
    - Senior Manager: 10 females, 46 males
    - Director: 5 females, 32 males
    - Executive: 2 females, 14 males

 ##### PAge2 (Performance Diversity):

- Average employee performance is 1.99.
- Female employees' average performance is 1.89, while male employees' average performance is 2.06.
- No significant performance differences were found across departments, new hires, employment types, job levels, or genders.

 ##### Page3 (Promotion Diversity):

- 36 employees were promoted, with 8 females and 28 males.
- Male employees are being promoted significantly more than female employees, varying by service year, department, job level, and gender.

These insights highlight areas for improvement in gender equity, particularly in promotion opportunities and representation in leadership positions.

#

## Recommendation


#### Based on this analysis, I recommend:

1. Gender Balance Initiatives: Implement strategies to achieve a more balanced gender distribution, especially in leadership positions (e.g., Director, Executive).

2. Promotion Equity: Investigate and address the disparity in promotion opportunities for female employees, ensuring fair consideration regardless of gender.

3. Departmental Diversity: Focus on increasing female representation in departments like Operations, Sales & Marketing, and Finance, where they are underrepresented.

5. Performance Evaluation: Review performance evaluation processes to ensure fairness and equity, addressing any potential biases.

6. Mentorship and Development: Offer mentorship programs and training opportunities to support female employees' career growth and advancement.

7. Diversity and Inclusion Training: Provide regular training for all employees to foster a culture of inclusivity and respect.

8. Monitor Progress: Regularly track and analyze diversity metrics to ensure progress toward gender equity and adjust strategies accordingly.

By implementing these recommendations, the organization can work toward achieving greater gender diversity, equity, and inclusion.
