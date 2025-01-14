#  Internet Sales Analysis

### Project Overview/ Business Demand Overview
This data analysis project aims to provide insights into the internet sales performance of a company since its inception in 2021. The business request requires analysing various aspects of the data, including customer demographics, make data- driven recommendation, and budgeting for the following year.

![Sales overview dashboard](https://github.com/user-attachments/assets/81675864-88d7-4747-8ad0-7dcbee0d791d)


### Data Sources
The SQL database used for this analysis contained dim_calender, dim_customer, dim_product and Fact_InternetSales among other tables. These tables were used for the purpose of this data analysis.

### Tools
- SQL Server - Data Cleaning and Analysis
- Power BI - Creating Reports

### Data Cleaning
In the initial data preparation phase, we performed the following tasks:

1. Data loading and inspection
2. Data cleaning and formatting
  
 ### Exploratory Data Analysis
 EDA involved exploring the sales data to answer key questions, such as:

- Which products are top sellers?
- Which customers buy the most?
- What us the trend of sales over the years against sales budget?
![customer details](https://github.com/user-attachments/assets/54f8135e-7168-4503-990c-02734e9f8907)

![Product details](https://github.com/user-attachments/assets/67fcea7c-0b61-4eb6-af0b-60bd76be0c37)




### Data Analysis
Here are some interesting code/features I worked with: 
``` sql
SELECT [ProductKey]
      ,[OrderDateKey]
      ,[DueDateKey]
      ,[ShipDateKey]
      ,[CustomerKey]
      ,[SalesOrderNumber]
      ,[SalesAmount]
  FROM [AdventureWorksDW2019].[dbo].[FactInternetSales]
  WHERE 
  LEFT ([OrderDateKey], 4) >= 2022
  ORDER BY
  OrderDateKey ASC
```

### Results/Findings
The analysis results are summarized as follows:
Mountain-200 bike is the best-performing product in terms of sales and revenue.
The top 10 customers where spread across North-America and Europe.
The sales exceeded the sales budget increasingly as the years progressed since 2022. 


### Recommendations
Based on the analysis, we recommend the following actions:
Sales in cities Within the Asia continent can be improved on by increasing marketing tactics there.
The top 10 customers can be encouraged to bring more customers by including comissions or vouchers. 

