#Project Overview
This notebook builds a data pipeline using the AdventureWorks database to turn raw sales data into clean, organized information for business analysis. It takes data from different sources, including a MySQL database (which is an OLTP system used for storing daily business transactions), MongoDB, and CSV/JSON files. The pipeline is designed to support OLAP (Online Analytical Processing), which means it helps you run reports and analyze trends, not just store data.

The project uses a layered approach to process the data in three steps:

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
