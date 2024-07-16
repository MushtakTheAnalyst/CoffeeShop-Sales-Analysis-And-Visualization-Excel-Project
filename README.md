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
- [Dashboard Overview](#dashboard-overview)
- [Key Insights and Recommendations](#key-insights-and-recommendations)


## Project Description
The goal of this project is to analyze and visualize coffee shop's sales data from the year 2019 to 2022 using microsoft excel. This Excel-based dashboard provides stakeholders with critical insights, enabling them to drive smarter business decisions.


## Project Goal
The goal of this project is to analyze coffee order data to find trends in sales over time and by different coffee bean types, sales, by country, and we can gain some insights into who our top customers are.


## Project Requirement
The goal of this Excel project is to develop a sales analysis Dashboard from 2019 to 2022, delivering essential insights to clients using datasets with three different tables ie. customers, orders and products. The primary goal was to analyze retail sales data to gain insights that could help improve the coffee shop’s operations and sales strategies. The specific questions I aimed to answer included:

1. How do sales trend monthly, quarterly and yearly basis?
2. What is the total revenue for each month, quarters and year?
3. How do sales vary across different countries?
4. The top customers with/without loyalty cards
5. Which products are the best selling in terms of revenue and quantity?
6. How do sales vary by product type categories?


## Stakeholders List
- Manager
- Sales Lead
- Marketing Team


## Data Structure and Source
The dataset is in Excel (.xlsx) format with 3 different datasets customers, orders, and products table with unique keys like customer id. It contains customers and sales details with fields like coffee type, roast type, quantity, customers details and order details with sales from 2019 to 2022.

The data are from Kaggle and are available at: https://www.kaggle.com/datasets/mohammadkaiftahir/coffee-orders-data


## Data Cleaning and Transformation
I verified the dataset and found no empty cells, except in the email column. These gaps were addressed using the IF and XLOOKUP functions. Additionally, I reformatted the date column for better readability.


![Screenshot 2024-07-16 140806](https://github.com/user-attachments/assets/2e20ed90-afdd-4191-ae06-d37f4d91e2f6)



## Data Processing
To begin with, the dataset was comprised of three tables: one containing order details, another with customer information, and a third focused on product specifics. To enrich the orders table with customer details (name, email, and country),i utilized the XLOOKUP function. Following this, i also used the INDEX MATCH function to pull product-related data, including coffee type, roast type, size, and unit price.

To determine the total sales value, i calculated it by multiplying the quantity column with the unit price column. The coffee type and roast type information were initially abbreviated, so i created two additional columns to clearly display the full names of these categories. This was achieved using the IF function. Additionally, i reformatted the order date from its original format (e.g., 9/5/2019) to a more readable format (e.g., 5-Sep-2019).

For better clarity, we formatted the size and price columns by adding units—"kg" for size and "$" for price. Converting the dataset into a table format was a critical step, as it simplified data classification and filtering, and enhanced the functionality of pivot tables by allowing for automatic updates and the inclusion of new columns.

With the data now cleaned and prepared, can proceed to the analysis phase.


![Screenshot 2024-07-16 141104](https://github.com/user-attachments/assets/71b841a8-148d-4ac0-9a66-009e9893b244)



## Data Analysis

In Excel, pivot tables are incredibly useful for data analysis. We began by creating a pivot table to visualize total sales over time, using dates as rows, coffee types as columns, and sales as the values. This pivot table allowed us to generate a line chart displaying total sales over time. 

![Screenshot 2024-07-16 143822](https://github.com/user-attachments/assets/f30c7595-9216-4480-842b-a34e3834181c)

We followed a similar approach for the sales by country dashboard. First, we created a pivot table with countries as rows and total sales as values. From this table, we generated a bar chart to show sales by country. Next, we created a pivot table with customer names and the total amount they spent on products. We filtered this table to display only the top 5 customers, allowing us to create a bar chart showing these top customers and their total sales.

![Screenshot 2024-07-16 143921](https://github.com/user-attachments/assets/c1e74b6c-9a17-48e4-9c3b-2ec4a13575b9)


We then created a timeline to enable the selection of specific time periods for analysis. Additionally, we added three slicers: roast type, size, and loyalty card. These slicers act as data filters. For example, selecting “dark” roast type in the slicer displays data only for that specific roast type. The “loyalty card” information was originally in the "customers" database, so we used XLOOKUP to add this data to the "orders" database, which we used for the dashboard. Then we had created two KPIs to show the total sales and total quantity connecting to the other slicers and charts.

![Screenshot 2024-07-16 143954](https://github.com/user-attachments/assets/368028d2-f196-4618-b421-6f95f1001d89)


Initially, the timeline and slicers only affected the line chart showing sales over time. To provide a more comprehensive analysis, we connected these elements to the other charts, ensuring that all visualizations were synchronized and interactive.


## Dashboard Overview

This dashboard reveals several valuable insights about our coffee sales. 

- **Top Customers**: Allis, Brenn, Terri, Nealson, and Don are our highest spenders. Interestingly, the top four customers for dark roast coffee each spent $179 on this type.
- **Roast Preferences**: Customers generally spend the most on medium and light roast coffee.
- **Loyalty Cards**: Customers with loyalty cards tend to spend less, suggesting that our loyalty program may need reevaluation.
- **Popular Size**: The 2.5kg size is the most popular among our customers.
- **Geographical Insights**: The United States is a leading market, with significantly higher sales than other countries across all roast types and sizes. However, checking product availability in each country is necessary to validate this observation.
- **Trends Over Time**: Arabica was highly popular in 2020 and 2021, but its sales saw a significant decline in 2022. Conversely, Excelsa has consistently performed well, showing high peaks in sales throughout the analyzed period.

![Screenshot 2024-07-16 144100](https://github.com/user-attachments/assets/1507eb27-fe2c-455d-960d-078fcea12d96)


## Key Insights and Recommendations

- **Excelsa Leads the Way in Revenue Generation**
Excelsa coffee takes the top spot in revenue generation, showcasing its significant impact on the coffee industry.

- **"Light" Roast Coffee Emerges as Revenue Leader**
Among various roast types, "Light" roast coffee stands out as the leader in revenue generation.

### Coffee Sales by Country:
- **🇮🇪 Ireland**: Liberica coffee outperforms other types in revenue in Ireland.
- **🇺🇸 United States**: Arabica coffee secures the top spot for revenue generation in the United States.
- **🇬🇧 United Kingdom**: Excelsa coffee stands out as the revenue leader in the United Kingdom.

### Sales Soar in 2021 with a 13.6% Surge
While 2019 and 2020 saw nearly identical sales figures, 2021 witnessed a significant boost with a 13.6% increase compared to the previous year, reflecting a thriving coffee market.

These insights can help us make informed decisions about the product offerings, marketing strategies, and customer engagement initiatives.

