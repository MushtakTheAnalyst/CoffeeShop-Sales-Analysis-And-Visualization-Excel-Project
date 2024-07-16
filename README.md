# Coffee Shop Sales Analysis
Coffee shop sales analysis from 2019 to 2022 dashboard using microsoft excel


## Table of Contents
- [Project Description](#project-description)
- [Project Goal](#project-goal)
- [Project Requirement](#project-requirement)
- [Stakeholders List](#stakeholders-list)
- [Data Structure and Source](#data-structure-and-source)
- [Data Cleaning and Transformation](#data-cleaning-and-transformation)
- [Data Processing](#data-processing)
- [Data Analysis](#data-analysis)
- [Visualization and Dashboard Overview](#visualization-and-dashboard-overview)
- [Key Insights](#key-insights)
- [Recommendations](#recommendations)
- [Conclusion](#conclusion)


## Project Description
The goal of this project is to analyze and visualize coffee shop's sales data from the year 2019 to 2022 using microsoft excel. This Excel-based dashboard provides stakeholders with critical insights, enabling them to drive smarter business decisions.


## Project Goal
The goal of this project is to analyze coffee order data to find trends in sales over time and by different coffee bean types, sales, by country, and we can gain some insights into who our top customers are.


## Project Requirement
The goal of this Excel project is to develop a sales analysis Dashboard from 2019 to 2022, delivering essential insights to clients using datasets with three different tables ie. customers, orders and products. The primary goal was to analyze retail sales data to gain insights that could help improve the coffee shop’s operations and sales strategies. The specific questions I aimed to answer included:

1. How do sales vary monthly, quarterly and yearly basis?
2. What is the total revenue for each month, quarters and year?
3. How do sales vary across different countries?
4. The top 5 customers with/without loyalty cards
5. Which products are the best selling in terms of revenue?
6. How do sales vary by product category and roast type?


## Stakeholders List
- Business Development Manager
- Sales Team
- Marketing Manager


## Data Structure and Source
The dataset is in Excel (.xlsx) format with 3 different datasets customers, orders, and products table with unique keys like customer id. It contains customers and sales details with fields like coffee type, roast type, quantity, customers details and order details with sales from 2019 to 2022.

The raw dataset is attached in the project here.


## Data Cleaning and Transformation

1. The dataset underwent was analyzed in Microsoft Excel to enhance comprehension and identify areas requiring cleaning before analyzing. Notable issues included blank entries and spelling errors. Specifically, the ‘Accident_Severity’ and ‘Junction_Control’ columns included errors such as ‘Fetal’ instead of ‘Fatal’ and ‘Auto traffic sigl’ instead of ‘Auto traffic signal’.

2. The raw data was duplicated into a new sheet, and labeled ‘Data Worksheet.’ The subsequent cleaning procedures were executed on this dedicated sheet, comprising:
 - The Dataset columns were spaced to get a full view
 - Each column was checked for anomalies and any error
 - Blank cells in the columns 'Road_Surface_Conditions' and 'Road_Type' was grouped as "Others" instead of removing the black cells
 - All errors were corrected using the Find and Replace function in Excel
 - Made sure data is consistent and clean with respect to data type, data format and values used
 - Creating 2 new attributes 'Year' and 'Month' were added for logical and easy interpretation of dataset


**Preview of a section of cleaned data sheet -**
![Screenshot 2024-07-13 164434](https://github.com/user-attachments/assets/cf0d1965-bab9-48cb-9a83-4418a95f8f47)


## Data Processing

Part of the requested KPIs by the client is to showcase the dashboard in monthly and yearly insight, but from our data, we only have an Accident_Date column with the full date for each data entry. Therefore, there is a need to create month and year columns to get the requested insight. The process of doing this is as follows;

1. Create two blank columns, and name them ‘Month’ and ‘Year’ respectively

2. Use the Excel Text function to extract the month and year from the Accident_Date column.
 - =TEXT(B2, “mmm”) for the newly created ‘Month’ column
 - =TEXT(B2, “yyyy”) for the newly created ‘Year’ column


![Screenshot 2024-07-13 134108](https://github.com/user-attachments/assets/c52d4855-3f72-4bbf-8048-94861f2a9978)


## Data Analysis

#### Primary Key Performance Indicators (KPIs)

- The Excel-Pivot Table was utilized to determine the total number of casualties after the accident in 2021 and 2022.
- The Accident_Severity is of 3 types- Fatal, Serious and Slight. PivotTable was utilized to determine the total number of casualties for each Accident_Severity type, and the Excel function was used to calculate the percentage of total casualties for each Accident_Severity type.
- The same PivotTable was used to determine the Vehicle_Type with maximum casualties.

#### Secondary Key Performance Indicators (KPIs)

- Categorized total casualties based on vehicle types using Excel PivotTable, and casualties for agricultural vehicles, cars, buses, vans, bikes, and others were identified. This breakdown facilitates a detailed understanding of the impact across various vehicle categories.
- Utilized Excel Pivot Table to compare monthly casualties for the current and previous years. This analysis helps identify patterns, seasonality, and potential contributing factors to accidents with time.
- Identified and analyzed the road types associated with the highest casualties. Excel Pivot Table was instrumental in summarizing and visualizing this data.
- Utilized Pivot Table to break down casualties based on road surface conditions. This analysis provides insights into the impact of road conditions on accident severity.
- Excel PivotTable was employed to analyze the correlation between casualties' location and time of day. Understanding the relationship between these variables contributes to targeted safety measures, especially in specific areas.


## Visualization and Dashboard Overview

1. Visualization:

A dedicated ‘Data Analysis’ sheet was created for comprehensive data visualization. Excel’s ‘Insert Function’ feature was utilized to pick suitable charts for each table derived from PivotTable data analysis.

- Primary KPIs: Doughnut charts were employed to visualize and represent primary KPIs. The charts were formatted for clarity, ensuring a clean and easily interpretable presentation.
- Secondary KPIs: Different visualization tools, including Doughnut chart, Treemap, Line graph, and Bar chart, were utilized to convey insights from secondary KPIs.


![Screenshot 2024-07-13 164038](https://github.com/user-attachments/assets/e9957059-0808-49cb-9999-981d9c88da7c)


  
2. Dashboard:

An interactive dashboard with key features to enhance usability and understanding was developed.

- The timeline button was integrated to visualize road accidents in 2021 and 2022 separately or collectively. This enables a more detailed examination of trends and patterns over each year.
- Slicer functionality was incorporated into the dashboard, using Rural/Urban categorization as a filter. This allows users to view the dashboard based on specific KPIs and choose between Urban, Rural, or overall perspectives for a targeted analysis.
- The dashboard is intricately linked with the ‘Data Analysis’ sheet, and providing seamless navigation to internet resources. This integration ensures easy mobility and quick access to related information. This can be interacted with with the use of icons on the left-hand side of the dashboard.


**Final Dashboard:**
![Screenshot 2024-07-13 164705](https://github.com/user-attachments/assets/9de6a973-9571-4bac-b27f-bc6a4ab24be3)



## Key Insights

**Total Casualties Analysis:** The dashboard reveals an alarming 417,883 casualties occurred due to accidents over the two-year period.

**Peak Months:** Casualties were slightly higher in 2021 compared to 2022. The highest number of casualties occurred in October and November in both years, while the lowest casualties were in January and February.

**Casualties by Vehicle Type:** Car accidents accounted for the majority of casualties, contributing to 79.8% of the total. Casualties were minimal in accidents involving other vehicle types.

**Casualties by Accident Severity:** Slight severity accidents accounted for the majority of casualties (84.1%), while fatal severity casualties were only 1.7%.

**Road Type Analysis:** The highest number of casualties occurred on single carriageway roads (309.7K), and the lowest on slip roads (4.7K).

**Casualties Distribution by Road Surface:** The majority of casualties (66.9%) occurred on dry road surfaces.

**Casualties Relation by Area/Location:** Urban areas accounted for 61% of the casualties after accidents.

**Casualties Distribution by Light Condition:** 73% of casualties occurred during daylight conditions.


## Recommendations

1. **Focus on High-Risk Periods:** By comparing casualty trends between the current and previous years on a monthly basis, the dashboard identifies critical periods in October and November. Traffic police and other stakeholders should increase safety measures and monitoring during these high-risk months.

2. **Target Car Drivers:** Since car drivers account for the bulk of casualties, they should be the focus of awareness campaigns, strict monitoring, and periodic check-ups on safe driving.

3. **Improve Single Carriageway Roads:** Extra safety measures should be implemented on single carriageway roads, and wherever possible, these roads should be upgraded to double lanes.

4. **Enhance Road Surface Conditions:** Understanding casualty distribution based on different road surface conditions helps pinpoint areas where road maintenance and surface improvements are essential.

5. **Interventions in Urban Areas:** Urban areas should be targeted for specific interventions to improve road safety, particularly during daylight hours.
