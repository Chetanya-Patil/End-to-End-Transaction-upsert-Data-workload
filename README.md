# End-to-End-Transaction-upsert-Data-workload
Here, This is end to end project which consist of multiple technology and it will be very similar to production usecase. We will also create it's blog content and video content soon.


First Session:
In a data environment, data is initiated at operational databases and data will be extracted-transformed-loaded (ETL) to the data warehouse to suit the analytical environment.

##What is Slowly changing dimension ?
-->A slowly changing dimension (SCD) is a dimension that is able to handle data attributes which change over time. 
For example:
A customer dimension may hold attributes such as name, address, and phone number.
Over time, a customer's details may change (e.g. move addresses, change phone number, etc).

A slowly changing dimension is able to accommodate these changes, with some SCD patterns having the added ability to preserve history. Deciding on which type of slowly changing dimension pattern to implement will vary based on your business requirements.

Slowly Changing Dimensions in Data Warehouse are used to perform different analyses. Here we will discuss to implement Different types of Slowly Changing Dimensions such as Type 1, Type 2, Type 3. Apart from these, there are also Hybrid SCDs that you might come across. A Hybrid SCD is nothing but a combination of multiple SCDs to serve your complex business requirements.



##Better Solution now a days
-->
Here is where the Delta Lake comes in. Using its many features such as support for ACID transactions (Atomicity, Consistency, Isolation and Durability) and schema enforcement we can create the same durable SCD’s. This may have required a series of complicated SQL statements in the past to achieve this.


Slowly changing dimension Type 1 
- Overwrite the former value without saving history

Example:
<Get content of it from Oracle Website with examples and implement it with clear scenario.>
Implement:


Slowly changing dimension Type 2
- Enables you to track history of updates

Example:
Consider there is a column LOCATION in the EMPLOYEE table and you wish to track the changes in the location on employees. Consider a record for Employee ID 1001 present in your EMPLOYEE dimension table. Steve was initially working in India and then shifted to USA. We are willing to maintain history on the LOCATION field.



Implement:


Slowly changing dimension Type 3
- Creates a new current value column in the existing record but retain the existing column as well.

Example:

Implement:

