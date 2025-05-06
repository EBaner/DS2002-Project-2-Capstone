# DS2002 Project 2 Capstone

This notebook builds a data pipeline using the AdventureWorks database to turn raw sales data into clean, organized information for business analysis. It initially uses data from AdventureWorks to export data into MongoDB and into CSVs. It then takes the data from different sources, including a MySQL database (which is an OLTP system used for storing daily business transactions), MongoDB, and CSV/JSON files and inserts it into a lakehouse architecture. After this, the fact sales table is used to establish and encorperate the three layers: 

Bronze layer: stores raw data.

Silver layer: stores cleaned and structured data.

Gold layer: stores final tables ready for analysis.

The pipeline uses PySpark for large-scale data processing, and it includes both batch (scheduled) and streaming (real-time) data.

Dependencies Required
Make sure the following Python and Spark packages are installed:

pymysql – to connect to the MySQL database

pymongo – to connect to MongoDB

pandas – for data manipulation

numpy – for numerical operations

sqlalchemy – to help with database connections

certifi – for secure MongoDB connection

findspark – to initialize Spark in local environments

pyspark – for distributed data processing
