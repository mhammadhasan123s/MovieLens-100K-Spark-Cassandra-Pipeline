🎬 MovieLens-100K Spark–Cassandra Analytics Pipeline
P166175
🚀 Overview

This project implements an end-to-end big data analytics pipeline using Apache Spark and Apache Cassandra on the MovieLens 100K dataset.

It demonstrates how raw user behavior data can be processed, transformed, stored, and analyzed at scale to generate meaningful insights about movie ratings, user activity, and demographic patterns.

The pipeline follows a modern data engineering workflow:
HDFS → Spark Processing → Cassandra Storage → Spark SQL Analytics → Visualization

🎯 Objectives
Build a scalable big data pipeline using Spark and Cassandra
Process and clean raw MovieLens dataset
Perform distributed transformations using Spark RDDs and DataFrames
Store structured data in Apache Cassandra for efficient querying
Analyze user behavior, rating patterns, and demographics
Generate insights using Spark SQL and Zeppelin visualizations
📊 Key Insights
A small percentage of users contribute a large portion of all ratings (power-user effect)
Movie popularity does not always correlate with higher average ratings
User preferences vary significantly across movie genres
Users under 20 represent a relatively small segment of the platform
Scientists aged 30–40 show a concentrated and identifiable demographic pattern
📈 Analytical Tasks

The project includes the following analytical components:

🎬 Average rating per movie
🏆 Top 10 highest-rated movies
👥 Active users (≥ 50 ratings) and their behavior
👶 Users younger than 20 analysis
🧪 Scientists aged 30–40 demographic segmentation
🎭 User genre preference analysis (advanced extension)
🏗️ Architecture
Raw Data (MovieLens 100K)
        ↓
HDFS Storage
        ↓
Apache Spark (RDD + DataFrame Processing)
        ↓
Data Cleaning & Transformation
        ↓
Apache Cassandra (Structured Storage)
        ↓
Spark SQL Analytics
        ↓
Zeppelin Visualization & Insights
⚙️ Technologies Used
Apache Spark (PySpark)
Apache Cassandra
HDFS (Hortonworks Sandbox)
Zeppelin Notebook
Python
🔁 Workflow
Load MovieLens dataset into HDFS
Create Spark RDDs and DataFrames
Clean and transform raw data
Write structured data into Cassandra tables
Query data using Spark SQL
Generate insights and visualizations in Zeppelin
📊 Example Outputs
Top-rated movies ranked by average rating
Distribution of highly active users
Genre preference analysis per user
Demographic segmentation of users (age & occupation-based)
💼 Business Value

This pipeline demonstrates how large-scale behavioral data can be transformed into actionable insights for:

Recommendation systems
User segmentation
Content strategy optimization
Engagement analysis

It simulates a real-world data engineering + analytics workflow used in modern streaming and recommendation platforms.

🧠 Skills Demonstrated
Big Data Processing (Apache Spark)
Distributed Data Engineering
SQL Analytics at Scale
Data Modeling with Cassandra
ETL Pipeline Design
User Behavior Analysis
Data Visualization (Zeppelin)
🔧 How to Run

⚠️ Requires Spark + Cassandra + Zeppelin environment

1. Dataset Setup

Upload MovieLens dataset to HDFS:

/user/maria_dev/ml-100k/
2. Start Services
Apache Spark
Apache Cassandra
Zeppelin Notebook
3. Run Pipeline

Execute notebook cells in order:

Data loading
Transformation
Cassandra writing
SQL analytics
📌 Reproducibility Notes

Ensure:

Cassandra keyspace and tables are created before execution
Spark-Cassandra connector version matches Spark version
Dataset paths in HDFS are correctly configured
Zeppelin interpreter is properly set up
📷 (Optional Enhancements)

You can improve this repo further by adding:

Charts screenshots in /outputs
Architecture diagram image
Sample query results
Dashboard screenshots
🏁 Final Note

This project showcases a complete end-to-end big data analytics pipeline, combining distributed processing, scalable storage, and analytical querying to derive meaningful insights from real-world data.
