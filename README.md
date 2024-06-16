# Kevin-s-Cookie-Company-Yearly-Sales-Analysis

## Table Of Contents 
 - [Project Overview](#project-overview)
 - [Data Sources](#data-sources)
 - [Tools](#tools)
 - [Data Cleaning and Preparations](#data-cleaning-and-preparation)
    1. [MS EXCEL DATA CLEANING](#ms-excel-data-cleaning)
       - [Power query identification on dataset](#power-query-identification-on-dataset)
    2. [SQL DATA CLEANING](#sql-data-cleaning)
  - [Exploratory Data Analysis (EDA)](#exploratory-data-analysis-(EDA))
  - [Data Analysis](#data-analysis)
  - [Results and Findings](#results-and-findings)
  - [Recommendations](#recommendations)
  - [Limitations](#limitations)
  - [References](#references)
---

## Project Overview 

**This is a data analysis personal project that aims to provide insights into the cookie sales at Kevin's Cookie Company for the years *(2017, 2018, 2019, 2020)*, by sourcing/extracting the dataset, aggregating/cleaning the dataset by automating redundant processes in power query macros then afterwards analysing various aspects of the yearly cookie sales. The data cleaning automation processes ensured that any new dataset that is incorporated into the existing dataset will go through the redundant cleaning automation processes. The project aims to present informed solutions to answer critically posed business questions from the stakeholders and management. This will be done through a keen identification of trends, make data driven recommendations and give a deeper understanding of the company's performance**

## Data Sources 

The primary dataset used for this analysis is the *(2017 Order Data.xlsx, 2018 Order Data.xlsx, 2019 Order Data.xlsx, 2020 Order Data.xlsx, All years combined.xlxs)* containing detailed information about cookie sales made per year by the cookie company. 

 - To download the dataset [click here](https://1drv.ms/u/s!AmxrofZZlZ-whKZQTEiA4iLu-WPiaQ?e=AkAtOi)

 ## Tools 
  - Excel - Used to Extract, Transform and Load data. It was also used to create a report through the generation of interactive dashboards.
  - SQL - Used for Exploratory data analysis and Data Wrangling.
  - Tableau - Creating reports from wrangled data in SQL

---

## Data Cleaning and Preparation 

In the initial data preparation phase, the following tasks were performed: 

### MS EXCEl DATA CLEANING 
 - Creation of a power query for automating the data cleaning processes. To learn how to create, load or edit a query in Excel (power query) in details [click here](https://support.microsoft.com/en-au/office/create-load-or-edit-a-query-in-excel-power-query-ca69e0f0-3db1-4493-900c-6279bef08df4)
 - Filtering out the data and removing unwanted rows, columns and data valuea in order to enhance the amalysis.
 - Addition of new columns such as the *profits* and *shipping number of days* which were going to be used in answering critical business operational queations.
 - Automated redundant processes using power query macros with main idea of not have to go through the same procedures while sourcing new data values into the dataset.
 - Conditional formating of the dataset to review KPIs
 - Creation of pivot tables that would allow for creation of pivot charts for report creation.

## Power query identification on dataset 

Excel 2019 Excel 2016
Power Query offers several ways to create and load Power queries into your workbook. You can also set default query load settings in the Query Options window.   

Tip:
😉 **To tell if data in a worksheet is shaped by Power Query, select a cell of data, and if the Query context ribbon tab appears, then the data was loaded from Power Query.**

## SQL DATA CLEANING 

 - Extract the dataset from the excel files.
 - Creation of tables to fit the dataset into.
 - Removal of data outliers by dropping/deleting unwanted values/columns and columns, thereafter format and updating tables.
 - Prepared the data for EDA processea and visualization in Tableau.

## Exploratory Data Analysis (EDA)

EDA involved exploring the dataset in order to answer the following questions:

 - *What is the overall cookie sales trend?*
 - *Which year had the most profits and what let to this?*
 - *What factors affect the steady downslope of cookie sales and the measures that can be implemented to curb this?*
 - *What measures could be taken to ensure maximum customer satisfaction?*
 - *What was the peak sales and what was the predicted future profits incase new measures were implemented?*
 - *Which cookie type/category contributed to yielding maximum profits?*

## Data Analysis 

The Analysis of the dataset involved the use sql code such as the one sampled below:
```sql
    SELECT * FROM 2017_DATASET WHERE Shipping = 2;
```
**The SQL code above assisted in the analysis of profits obtained for cookie sales delivered to customers within 2 days. It helped realise that a two day (or less) cookie delivery policy for a maximum of 1000 cookie shipped yields profits that had an upward trajectory**

## Results and Findings 

The Analysis results can be summarized as follows:
 - The company's sales on cookies has been increasing over the past years, with a noticeable peak during the year 2020

## Recommendations 
Based on the analysis, the following measures were recommended:
 - Invest in marketing and promotions during peak sales to maximize revenue.
 - Focus on expanding and promoting products in category
 - Implement a customer segmentation strategy to target high_liv customers effectively

## Limitations 

- We made some adjustments to the dataset while cleaning it through removing all free cookie sample datasets from the sales and budgets columns because they would have affected the accuracy of mu conclusions from the analysis.
- There are still a few outliers even after the commission but even then we can still see that there is a positive correlation between both budget and number of votes with revenue.

## References 

1. SQL for business analytics by
2. [stack overflow](https://stackoverflow.com)
