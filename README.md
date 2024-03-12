# ETL-Transformations
Essential Transformations used in the ETL Pipeline

## Table of Contents

*   [Overview](#overview)
*   [Transaction Control Transformation](#transaction-control-transformation)
*   [Sequence Generator Transformation](#sequence-generator-transformation)
*   [Update Strategy Transformation](#update-strategy-transformation)
*   [Union Transformation](#union-transformation)
*   [Normaliser Transformation](#normaliser-transformation)
*   [Rank Transformation](#rank-transformation)
*   [Sorter Transformation](#sorter-transformation)
*   [Aggregator Transformation](#aggregator-transformation)
*   [Router Transformation](#router-transformation)
*   [Joiner Transformation](#joiner-transformation)
*   [Look up Transformation](#look-up-transformation)

## Overview

ETL Transformations is essential for unlocking Data Insights and crucial for Enhanced Analytics.\
Design, Develope and Data validation of several Transformations are performed, which are crucial for ETL Pipeline.\
Transformations are Designed and Developed with the Help of Informatica Powercenter.


## Transaction Control Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation\
•	Lookup Transformation is performed on a lookup table, to get the department names.\
•	TCT (Transaction control transformation) is used to get the File names extracted based upon the department name.\
• Separate target files need not be mapped. Based on the file name feature in the flat file. Files will be saved dynamically. TCT Commands helps to achieve this requirement.\
•	Transaction control Commands: (TC_Continue_Transaction, TC_Commit_Before, TC_Commit_After, TC_Rollback_Before, TC_ Rollback _After)


![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/bdd84867-eaf4-421c-ba41-2abb91e93fda)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target with necessary SQL Queries\
•	Check all the target files for data quality, completeness and correctness.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/df39f275-3340-4f2c-809b-91aef2cee518)

## Sequence Generator Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Sorter Transformation is used to get the distinct values in a column.\
•	Aggregator Transformation will also give unique values in a column\
•	Unconnected Lookup Transformation is used to get the Department_Name from Department_ID\
•	Sequence generator is used to generate a integer numbers to a row with incremental values

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/958e10e2-68c1-4686-af7f-845e23e31a4f)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target with necessary SQL Queries\
•	Check all the target files for data quality, completeness and correctness.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/0898763a-0f15-4a6e-ae24-2c52ee6083bb)

## Update Strategy Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Update Strategy is used to perform DML Operations. These commands are used (DD_Insert, DD_Update, DD_Delete, DD_Reject)\
•	Make use of necessary Commands as per the requirement.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/c91384bb-c09f-49df-afde-71ea935d851e)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target with necessary SQL Queries\
•	Check Target for data quality, completeness and correctness.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/3a4bb92a-9d8e-4695-90b5-ad008494fb22)


## Union Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Union Transformation is used to Merge the data from two different sources, it is necessary to have the same column fields Data types, Count and order.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/e6e40b5d-1966-499c-aff0-65c599eb0e15)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target \
•	Check all the target files for data quality, completeness and correctness.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/6226e994-61b0-4f14-8552-e9c2803fad2d)

## Normaliser Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Normaliser Transformation is used to UNPVOT the table data. GCID (Generated Column ID) and GK (Generated Key) helps to transform the data.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/cf69f701-dd34-4bb5-bc61-cedc6da02fa4)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target \
•	Check target for data quality, completeness and correctness.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/85f3ec03-ed5c-4419-b7ec-c1dac529bacd)

## Rank Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Rank transformation is used to get the records based on the rank defined at the port level in Informatica Designer\
•	Bottom or Top options can be selected to get Ascending or Descending values.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/bf7c028f-91e8-4ad8-b5de-67adf115bd81)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target \
•	Check target for data quality, completeness and correctness.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/fec0cba5-be27-49aa-a89a-898102a436b6)


## Sorter Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Expression transformation used to transform data in to the necessary format\
•	Sorter transformation is used to input the data of a column in ascending or Descending order.\
•	Select the keys of a column to sort in ascending or descending.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/0ed5d116-90e0-48da-9957-52bcf69af3e8)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target with necessary SQL Queries\
•	Check Weather the data is sorted in the Target Tables

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/bb46e84b-6215-4399-b6bf-b2bd5c331f8c)

## Aggregator Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Aggregator Transformation is used to Group data and perform aggregator functions on the data

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/f9825129-1d01-4e59-806b-ef86ea062867)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target with necessary SQL Queries\
•	Check all the target files for data quality, completeness and correctness.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/b4d17cee-68ec-436c-843f-09a4e6ebe191)

## Router Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Router Transformation is used to Route the data according to the groups formed based on the condition specified

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target with necessary SQL Queries\
•	Check all the target tables for data quality, completeness and correctness.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/2a073891-c183-405e-a447-591ca97ea6a2)

## Joiner Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Joiner Transformation is performed when data extracted from two different sources.\
•	Joining condition can be Normal join, Master outer/ Detail outer or Full outer join (inner, left, right, Full outer joins)\
•	Master Table – Less Records, Detail Table – More Records

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/a73aa9e6-c04a-4c74-92b5-e3abf012a78d)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target with necessary SQL Queries\
•	Check all the target tables for data quality, completeness and correctness.\
•	Use Minus queries to check for truncation of data

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/0b79e513-c210-433f-a5b6-29782eb218c0)

## Look up Transformation

### Design and Development

•	Import source and target details to the Designer\
•	Design Mapping from source to target with necessary transformation \
•	Lookup Transformation is performed on a lookup table, it can be connected or unconnected transformation.\
•	If Lookup is connected in the data flow, then it is connected. Or else it is unconnected. Connected LKP can return more than one column but unconnected Lookup returns only one column values\
•	Look up transformation by default provides Left outer join and it provides option with (<,>, =, =) operators while specifying joining condition

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/82896362-3610-4f9a-a496-6977d17d0b41)

### Data Validation

•	Check Run properties and session logs for the detailed report\
•	Validate source and target with necessary SQL Queries\
•	Check Lookup column values for null values\
•	Check all the target tables for data quality, completeness and correctness.

![image](https://github.com/varma-prasad/ETL-Transformations/assets/108605375/6695a74c-143e-4235-8b9c-599125cacfd1)

----

## 🛠 Tools used
![](https://img.shields.io/badge/Informatica_Powercenter-v10.2.0-orange)
![](https://img.shields.io/badge/Oracle_Database_21c-v21.1.0-blue)

## Authors

- [Varma Prasad S](https://github.com/varma-prasad)

## 🛠 Skills
SQL, ETL, Python, Power BI...

## 🔗 Links

[![linkedin](https://img.shields.io/badge/linkedin-0A66C2?style=for-the-badge&logo=linkedin&logoColor=white)](https://www.linkedin.com/in/varma-prasad-s/)



