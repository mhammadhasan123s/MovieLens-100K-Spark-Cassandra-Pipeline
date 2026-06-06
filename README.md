# MovieLens-100K Spark–Cassandra Analytics Pipeline
P166175

---

## Overview

This project implements an end-to-end big data analytics pipeline using Apache Spark and Apache Cassandra on the MovieLens 100K dataset.

It demonstrates how raw user behavior data can be processed, transformed, stored, and analyzed at scale to generate meaningful insights about movie ratings, user activity, and demographic patterns.

The pipeline follows a modern data engineering workflow:

HDFS → Spark Processing → Cassandra Storage → Spark SQL Analytics → Visualization

---

## Objectives

- Build a scalable big data pipeline using Spark and Cassandra  
- Process and clean raw MovieLens dataset  
- Perform distributed transformations using Spark RDDs and DataFrames  
- Store structured data in Apache Cassandra for efficient querying  
- Analyze user behavior, rating patterns, and demographics  
- Generate insights using Spark SQL and Zeppelin visualizations  

---

## Key Insights

- A small percentage of users contribute a large portion of all ratings (power-user effect)  
- Movie popularity does not always correlate with higher average ratings  
- User preferences vary significantly across movie genres  
- Users under 20 represent a relatively small segment of the platform  
- Scientists aged 30–40 show a concentrated demographic pattern  

---

## Analytical Tasks

- Average rating per movie  
- Top 10 highest-rated movies  
- Active users (≥ 50 ratings) and their behavior  
- Users younger than 20 analysis  
- Scientists aged 30–40 demographic segmentation  
- User genre preference analysis (advanced extension)  

---

## Architecture

Raw Data (MovieLens 100K)  
→ HDFS Storage  
→ Apache Spark (RDD + DataFrame Processing)  
→ Data Cleaning & Transformation  
→ Apache Cassandra (Structured Storage)  
→ Spark SQL Analytics  
→ Zeppelin Visualization & Insights  

---

## Technologies Used

- Apache Spark (PySpark)  
- Apache Cassandra  
- HDFS (Hortonworks Sandbox)  
- Zeppelin Notebook  
- Python  

---

## Workflow

1. Load MovieLens dataset into HDFS  
2. Create Spark RDDs and DataFrames  
3. Clean and transform raw data  
4. Write structured data into Cassandra tables  
5. Query data using Spark SQL  
6. Generate insights and visualizations in Zeppelin  

---

## Example Outputs

- Top-rated movies ranked by average rating  
- Distribution of highly active users  
- Genre preference analysis per user  
- Demographic segmentation of users (age and occupation-based)  

---

## Business Value

This pipeline demonstrates how large-scale behavioral data can be transformed into actionable insights for:

- Recommendation systems  
- User segmentation  
- Content strategy optimization  
- Engagement analysis  

It simulates a real-world data engineering and analytics workflow used in modern streaming and recommendation platforms.

---

## Skills Demonstrated

- Big Data Processing (Apache Spark)  
- Distributed Data Engineering  
- SQL Analytics at Scale  
- Data Modeling with Cassandra  
- ETL Pipeline Design  
- User Behavior Analysis  
- Data Visualization (Zeppelin)  

---

## How to Run

### Requirements

This project requires:
- Apache Spark
- Apache Cassandra
- Zeppelin Notebook environment
- HDFS cluster

### Dataset Setup

Upload MovieLens dataset to HDFS:

/user/maria_dev/ml-100k/

### Execution Steps

1. Start Spark, Cassandra, and Zeppelin services  
2. Open Zeppelin notebook  
3. Run notebook cells in order:
   - Data loading  
   - Transformation  
   - Cassandra writing  
   - SQL analytics  
   - Visualization  

---

## Reproducibility Notes

Ensure the following before execution:

- Cassandra keyspace and tables are created  
- Spark-Cassandra connector version matches Spark version  
- Dataset paths in HDFS are correctly configured  
- Zeppelin interpreter is properly configured  

---

## Optional Enhancements

- Add charts/screenshots in an `/outputs` folder  
- Include architecture diagram image  
- Add sample query results  
- Add dashboard screenshots for presentation  

---

## Conclusion

This project demonstrates a complete end-to-end big data analytics pipeline, combining distributed processing, scalable storage, and analytical querying to derive meaningful insights from real-world data.
