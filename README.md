# ETL-Transformations
Essential Transformations used in the ETL Pipeline

## Table of Contents

* [Overview](#overview)
* [Transaction Control Transformation](#transaction-control-transformation)
* [Sequence Generator Transformation](#sequence-generator-transformation)
* [Update Strategy Transformation](#update-strategy-transformation)
* [Union Transformation](#union-transformation)
* [Normaliser Transformation](#Normaliser-transformation)


## Overview

ETL Transformations is essential for unlocking Data Insights and crucial for Enhanced Analytics.\
Designe, Develope and Data validation of several Transformations, which are crucial for ETL Pipeline.


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



