# ATM-data-ETL-Pipeline-Sqoop-Pyspark-Redshift

# Purpose: 
Banks have to refill the ATMs when the money goes below a specific threshold limit. This depends on the activity and the area where a particular ATM is located as well as the weather, day of the week, etc. In our project, Spar Nord Bank is trying to observe the withdrawal behavior and the corresponding dependent factors to optimally manage the refill frequency. Apart from this, other insights also have to be drawn from the data. We have data from more than 100 ATMs across Denmark. Data is captured for every transaction including, card type, location, date, time, ATM type, etc.

# Skills: 
Apache Sqoop, Apache PySpark, Amazon S3 and Amazon RedShift

# Aim:
Build a batch ETL pipeline to read transactional data from RDS, transform and load it into target dimensions and facts on Redshift Data Mart(Schema, after which some analytical queries have to be performed on the loaded data. 

This includes the following tasks-
1. Extracting the transactional data from a given MySQL RDS server to HDFS(EC2) instance using Sqoop.
2. Transforming the transactional data according to the given target schema using PySpark. 
3. This transformed data is to be loaded to an S3 bucket.
4. Creating the Redshift tables according to the given schema.
5.Loading the data from Amazon S3 to Redshift tables.
6. Performing the analysis queries.

Coming to the analysis part, you will be tasked to carry out the calculations to perform the following analytical queries:
1. Top 10 ATMs where most transactions are in the ’inactive’ state
2. Number of ATM failures corresponding to the different weather conditions recorded at the time of the transactions
3. Top 10 ATMs with the most number of transactions throughout the year
4. Number of overall ATM transactions going inactive per month for each month
5. Top 10 ATMs with the highest total amount withdrawn throughout the year
6. Number of failed ATM transactions across various card types
7. Top 10 records with the number of transactions ordered by the ATM_number, ATM_manufacturer, location, weekend_flag and then total_transaction_count, on weekdays and on weekends throughout the year
8. Most active day in each ATMs from location "Vejgaard"


