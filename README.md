# ETL Project for Optimal ATM Management

## Objective:
Developed a batch ETL pipeline to analyze ATM transaction data for Spar Nord Bank, focusing on withdrawal behaviors and factors influencing ATM refills.

## Dataset:
- Danish ATM Transactions Dataset (2017)
- 2.5 million records from 113 ATMs
- Includes transaction details, weather data, and ATM statuses

## Tasks Performed:
### Data Ingestion:
  - Extracted data from MySQL RDS to HDFS using Apache Sqoop.

### Data Transformation:
  - Used PySpark to transform data into the target schema:
    - Created dimension tables (ATM, Location, Date, Card Type).
    - Created a transaction fact table.
  - Ensured data cleanliness, generated primary keys, and removed duplicates.
    
### Data Loading:
  - Loaded transformed data into Amazon S3.
  - Created and loaded data into Redshift tables.

### Data Analysis:
  - Performed analytical queries to derive insights:
    - Top 10 ATMs with most inactive transactions.
    - ATM failures by weather conditions.
    - Monthly inactive transaction trends.
    - Top 10 ATMs by total withdrawals.
    - Failed transactions by card type.
    - Most active days for specific locations.

### Skills and Technologies:
Apache Sqoop, Apache PySpark, Amazon S3, Amazon Redshift, MySQL,HDFS

### Impact:
Enhanced the bank’s ability to manage ATM refills efficiently, reducing downtime and improving customer satisfaction by leveraging big data tools for insightful analysis.
