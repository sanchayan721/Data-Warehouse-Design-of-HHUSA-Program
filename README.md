# Data-Warehouse-Design-of-HHUSA-Program

## Introduction

Hire Hero USA is a non-profit organization devoted towards connecting veterans and their spouses with organizations willing to hire. 
Not only that, they also provide volunteer services to willing participants by conducting mock interview sessions and other necessary 
arrangements while logging their data in transactional data bases. Such a data source is been analysed here in order to find 
relevant correlations in Employer Partnerships and Opportunities and Serving Spouses Program guided by the business questions in Teradata. 
The link to the data source and the business questions of interst is 
[here](https://academics.teradata.com/Community/Student-Competitions/2019/2019-Data-Challenge/Business-Questions). 


## The Flow of the Project

### Cleaning and Designing Reconsiled Schema
After downloading the dataset from the given link the first step is to clean and integrate the data to get a reconciled schema 
which is done using **Tableau Prep Builder**.

### Dimentional Fact Modelling
* Observations and assumptions are made in order to design the conceptual schema.
* **DFM** notation is used in order to design the conceptual schema.

### Conceptual Design
* Next step is to nievely design the *conceptual schema* from the DFM which is done using **Microsoft Visio**.
* Now we will explore different *views* considering different *aggregation patterns* related to the dimensions in the Fact Table.
* We need to calculate the *workload* in order to determine which view to *materialize*.
### Redesigning the Conceptual Schema
We will redesign our *conceptual schema* considering the cost of *materialized view* 
with respect to the business questions of our interest.
### ETL Design
* We will design the data Extraction and Transfor mation process using *Tableau Prep Builder*.
For reference please look for the *flow* inside Tableau Prep directory.
* The *Data Marts* corresponding to the *Data Warehouse* is built in **PostgreSQL** server. 
* The outputs of the *Extraction* and *Transformation* process is loaded into corresponding tables into PostgreSQL relational database.
### Analysis using OLAP queries
The analysis is primarily done by making *OLAP queries* on the data warehouse. Some of the concepts used are like *rollup*,*group by*, 
*window*, *window partioning*, *cube*, *group by grouping sets* and more. For more details please look for the documentation.
### Analysis and Visualization using Tableau Desktop
* Visualizations and in depth graphical analysis is done by using *Tableau Desktop* application.
* Connecting the PostgreSQL Database with Tableau Prep is a bit challenging and sometimes causes errors. Please look for the Tableau user 
manual for corresponding errors.
### Results
The results are primarily shown in the Tableau Desktop *Workbook* and some calculations are done directly on PostgreSQL.
Which could be found in the documentations and the presentation directory without recreating the entire process.
