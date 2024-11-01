# Building-a-Data-Warehouse


## Table of Contents
<ul>
<li><a href="#intro">Introduction</a></li>
<li><a href="#source">Data Sources</a></li>
<li><a href="#parta">Part 1: Implementing a SQL Data Warehouse</a></li>
<li><a href="#partb">Part 2: Loading Data From Various Sources Into Data Warehouse</a></li>
</ul>

<a id='intro'></a>
## Introduction
In this project, I designed a comprehensive data warehouse, establishing both fact and dimension tables. I utilized SQL for the creation of the warehouse and successfully integrated data from various sources, including an SQL database and CSV files. This integration was achieved through the SQL import/export tools as well as SSIS data pipelines, ensuring a seamless flow of information into the warehouse.

<a id='source'></a>
### Data Source:
- SQL Database
- CSV File:[FactSalesTable.csv](https://github.com/user-attachments/files/17593089/FactSalesTable.csv)





<a id='parta'></a>
## Part 1: Implementing a SQL Data Warehouse:
Aggregating and managing large volumes of customer data for analytical purposes.




### Step 1: Investigate data in the database for accuracy and check if any data cleaning is required.
![image](https://github.com/user-attachments/assets/34f5f324-18dc-4fc9-8711-d0c4fec70715)



### Step 2: Make the necessary cleansing processes such as changing the data types of some columns to the correct data types and handling nulls.
![image](https://github.com/user-attachments/assets/ac8c0bb6-01f8-490f-8d8e-e8e6453a19cc)



### Step 3: Study the database structure and components after cleaning to identify fact and dimension tables in the data warehouse.


### Step 4: Identify the columns to be put into fact and dimension tables.



### Step 5: Choose the suitable schema for the data. Star schema in our case.



### Step 6: Create a surrogate key in the Fact table named (SalesKey) to be the key of the fact table in the data warehouse.


### Step 7: Identify Primary keys in dimension tables which foreign keys in fact table
![image](https://github.com/user-attachments/assets/98a8040f-3e39-4f68-910d-6a21615e3033)



### Step 8: Create the data warehouse(Customer_DW)
![image](https://github.com/user-attachments/assets/d03e5f4d-08fe-42ba-bb7d-2e66ae483b5e)


### Step 9: Create fact and dimension tables of the data warehouse
![image](https://github.com/user-attachments/assets/9f9c1781-856b-41e7-a0de-1d720e88b332)
![image](https://github.com/user-attachments/assets/89b81a8f-83f7-4954-8d21-724f3f0daccd)






<a id='partb'></a>
## Part 2: Loading Data From Various Sources Into Data Warehouse:


### Step 10: Populate Customer and product Dimension Tables (Using the Import and Export Wizard Tool):
#### Choosing source and destination databases and tables, mapping columns, and finishing the import process.
![image](https://github.com/user-attachments/assets/8be65ba6-a593-4465-9b38-16d95d656354)
![image](https://github.com/user-attachments/assets/d025cc2d-1cca-4125-8121-9e460a075a63)
![image](https://github.com/user-attachments/assets/44b879d5-3143-4493-970c-61604cc09af8)


### Step 11: Populate Product Dimension Table (Using SSIS and Visual Studio):
#### Set the connection manager, Create a data flow, create the workflow in which we choose the source and destination and map the columns, and finally run the SSIS package to transfer the data into the warehouse.

![image](https://github.com/user-attachments/assets/5aa9113d-0114-4c5a-85df-478397d4c73a)
![image](https://github.com/user-attachments/assets/2cdbcaeb-668c-48d2-bac4-417dd9822091)
![image](https://github.com/user-attachments/assets/92fcb599-51fc-4dd6-9d00-63e1f425cb06)
![image](https://github.com/user-attachments/assets/42b69d9f-d126-4455-ae16-fa628a9a06b2)
![image](https://github.com/user-attachments/assets/ed163285-8fa4-452e-93a6-8fa7d15ef262)


### Step 12: Check the populated customer Dimension table on the warehouse
![image](https://github.com/user-attachments/assets/079d6caf-cc01-43b9-8f38-37a5922082ea)



### Step 13: Populate the Date Dimension table:
#### Using an SQL query populated the time dimension table with all its columns
![image](https://github.com/user-attachments/assets/0390ede9-5403-4087-9bca-7f0c93c58592)



### Step 14: Populating the fact table (from a CSV file using SSIS Tool in Visual Studio)
![image](https://github.com/user-attachments/assets/4ee7488d-3d59-4cf7-906b-cdb5b3a91983)
![image](https://github.com/user-attachments/assets/3e048396-2c2c-432a-b494-bd57a08bfeb3)
![image](https://github.com/user-attachments/assets/3c6b1680-8942-4051-af36-b44ec53a7794)
![image](https://github.com/user-attachments/assets/ea507ca6-6db8-456d-b0e5-b35e39f84c93)



### Step 15: Check the populated data of the Fact table in the data warehouse:
![image](https://github.com/user-attachments/assets/bb913299-f107-40c6-95fa-f689d8e0c463)


## Now the data warehouse is ready to conduct the required analytics!









