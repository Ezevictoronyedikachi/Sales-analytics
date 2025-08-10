# Sales Analytics (Coffee sales data)


## Table of Contents

- [Project Overview](#Project-Overview)
- [Data Sources](#Data_Source)
- [Recommendation](#Recommendation)

### Project Overview

This data analytics project aims to provide insight into the sales performance of an E-commerce company over a period of time. By analyzing various aspects of the sales data, we seek to identify trends, make data driven recommendation, and gain a deeper understanding of the company's performance.

### Data Source:

Sales Data: The primary dataset used for this project analysis is the "coffeeOrdersData.xlsx" file, containing detailed information about each sales made by the company.

### Tools
- Excel( This is used for the cleaning, and creation of dashboard and report creation) [Download Here](Https://Microsoft.com/)

### Data Cleaning/Preparation

In the initial preparation phase, we performed the following tasks:
1. Data loading and inspection
2. Handling missing values
3. Data cleaning and formatting


### Exploratory Data Analysis

EDA involved exploring the sales data to answer key questions, such as;

- What is the overall sales trend?
- Which product are top sellers?
- What are the peak sales periods?

### Data Analysis
Used Xlookup to matchup a customer's name in a different sheet to another sheet
``` EXCEL
=XLOOKUP(C2,customers!$A$1:$A$1001,customers!$B$1:$B$1001,0)
```
Used Xlookup to matchup the customer's mail address to the next sheet
``` EXCEL
=IF(XLOOKUP(orders!$C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,0)=0," ",XLOOKUP(orders!$C2,customers!$A$1:$A$1001,customers!$C$1:$C$1001,0))
```

### Result/Findings

The analysis result are summarized as follows:
1. The company's sales has been increasing over the past year. with a noticable increase in 2020
2. United states in the Country category has the highest number of customers


### Recommendation
Based on the analysis, i recommend the following actions:
- I invest in marketing and promotion during peak sales seasons to maximize revenue
- I implement a customer segmentation strategy to target higher population effectively

### Limitations
I had to drop individual rows who do not have country address in order to have clean data. 
