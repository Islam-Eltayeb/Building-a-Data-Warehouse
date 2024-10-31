# Building-a-Data-Warehouse
Building an SQL data warehouse and integrating data from different sources to the warehouse with data pipelines. 



### Data Source:
- SQL Database
- CSV File:[FactSalesTable.csv](https://github.com/user-attachments/files/17593089/FactSalesTable.csv)


### Part 1: Implementing a SQL DATA Warehouse:
Aggregating and managing large volumes of customer data for analytical purposes.



#### Step 1: 
Investigate data in the database for accuracy and check if any data cleaning is required.
![image](https://github.com/user-attachments/assets/34f5f324-18dc-4fc9-8711-d0c4fec70715)


#### Step 2:
Make the necessary cleansing processes such as changing the data types of some columns to the correct data types and handling nulls.
![image](https://github.com/user-attachments/assets/ac8c0bb6-01f8-490f-8d8e-e8e6453a19cc)


#### Step 3: 
Studying the database structure and components after being cleaned to identify fact and dimension tables in the data warehouse.


#### Step 4:
Identify the columns to be put into fact and dimension tables.


#### Step 5:
Choose the suitable schema for the data. Star schema in our case.


#### Step 6:
Create a surrogate key in the Fact table named (SalesKey) to be the key of the fact table in the data warehouse.


#### Step 7: 
Identify Primary keys in dimension tables which foreign keys in fact table
![image](https://github.com/user-attachments/assets/98a8040f-3e39-4f68-910d-6a21615e3033)



#### Step 8:
Create the data warehouse(Customer_DW)
![image](https://github.com/user-attachments/assets/d03e5f4d-08fe-42ba-bb7d-2e66ae483b5e)



