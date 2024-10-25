Metrics Analysis Project
Overview
This project involves the analysis of agent performance metrics using AWS services, specifically Amazon S3, AWS Glue, and Amazon Athena. The metrics include key performance indicators such as Average Handle Time (AHT), Absolute Resolve Rate (ARR), and more. The goal is to extract insights from CSV data files and visualize them in a dashboard.
Setup Instructions
1.	Create S3 Buckets
o	Create two S3 buckets: one for the source data and another for output from Athena queries.
o	Upload metrics_1.csv and metrics_2.csv to the source bucket.
2.	Set Up AWS Glue Crawler
o	Create a Glue Crawler to detect the schema of your CSV files.
o	Configure the crawler to point to your source S3 bucket and run it to create the necessary tables in the Glue Data Catalog.
3.	Create Athena Tables
o	Use the AWS Athena console to create external tables based on the Glue Crawler output.
4.	Run SQL Queries
o	Use the provided SQL scripts in the /scripts directory to perform data analysis.
o	For example, execute create_view.sql to create a combined view of the metrics.
5.	Visualize Data
o	Connect Amazon QuickSight (or your preferred BI tool) to Athena.
o	Create a dashboard using the results from your SQL queries.
