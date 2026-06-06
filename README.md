# MovieLens-100K-Spark-Cassandra-Pipeline
P166175
## Overview
This project implements a data pipeline using Apache Spark and Apache Cassandra on the MovieLens 100K dataset.
## Dataset
Download from:
[grouplens.org](https://grouplens.org/datasets/movielens/)
Files used:
- u.user
- u.data
- u.item
## Technologies
- Python 3.x
- Apache Spark
- Apache Cassandra
- Zeppelin Notebook / Jupyter Notebook
- HDFS
## Workflow
1. Load raw data into HDFS
2. Create RDDs from raw files
3. Convert RDDs into Spark DataFrames
4. Clean and preprocess data
5. Store DataFrames in Cassandra
6. Read Cassandra tables back into Spark
7. Execute analytical queries
8. Present outputs with tables and charts
## Analytical Tasks
- Average rating for each movie
- Top 10 highest-rated movies
- Users with at least 50 ratings and their favourite genre
- Users younger than 20
- Scientists aged 30 to 40
## Reproducibility
Ensure:
- Cassandra keyspace and tables are created
- MovieLens files are uploaded to HDFS
- Spark Cassandra connector version matches Spark/Scala version
- Zeppelin interpreter is configured with Cassandra connector
