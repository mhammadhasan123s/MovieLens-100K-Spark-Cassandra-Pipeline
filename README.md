# MovieLens-100K-Spark-Cassandra-Pipeline
P166175
## Dataset
Download from:
[grouplens.org](https://grouplens.org/datasets/movielens/)
Files used:
- u.user
- u.data
- u.item
## Project Overview

This project builds a complete big data pipeline using Apache Spark and Apache Cassandra to analyze user behavior and movie ratings from the MovieLens 100K dataset.

The system processes raw data, performs distributed transformations, stores structured results in Cassandra, and generates analytical insights using Spark SQL.

## Objectives
Build an end-to-end big data pipeline
Process and clean raw MovieLens dataset using Spark
Store structured data in Cassandra for scalable querying
Perform analytical queries to understand user behavior and movie popularity
Visualize key insights using Zeppelin notebooks
## Key Insights
A small group of users contributes a large portion of all ratings (power-user effect)
Movie popularity does not always correlate with higher average rating
Genre preferences vary significantly across users
Younger users (<20) represent a smaller segment of the dataset
Scientists aged 30–40 show a concentrated demographic pattern
## Analytical Tasks
#### Average rating per movie
#### Top 10 highest-rated movies
#### Active users (≥ 50 ratings) and their preferences
#### Users younger than 20
#### Scientists aged 30–40 demographic analysis

## Architecture
HDFS → Spark (RDD/DataFrame) → Data Cleaning → Cassandra → Spark SQL → Visualization

## Technologies Used
Apache Spark (PySpark)
Apache Cassandra
HDFS (Hortonworks Sandbox)
Zeppelin Notebook
Python
## Workflow
Load MovieLens dataset into HDFS
Create RDDs and DataFrames using Spark
Clean and transform data
Store structured data in Cassandra
Query data using Spark SQL
Generate insights and visualizations
## Output Examples
Movie ranking based on average rating
User activity distribution
Genre preference analysis
Demographic segmentation
## Business Value

This pipeline demonstrates how large-scale user behavior data can be transformed into actionable insights for recommendation systems, audience segmentation, and content strategy optimization.

## Reproducibility

Ensure:

Cassandra keyspace and tables are created
MovieLens dataset is loaded into HDFS
Spark-Cassandra connector is correctly configured
Zeppelin interpreter is properly set up
