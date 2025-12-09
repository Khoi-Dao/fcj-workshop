---
title: "Week 7 Worklog"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.7. </b> "
---


### Week 7 Objectives:

* Understand Amazon DynamoDB as a fully managed NoSQL database service: key-value and document data models, partition keys, sort keys, global secondary indexes (GSI), and on-demand vs provisioned capacity modes.
* Learn how to build and manage Data Lakes on AWS using services like Amazon S3, AWS Glue, Amazon Athena, and Amazon QuickSight for analytics workloads.
* Explore AWS Analytics services: Amazon Athena for serverless SQL queries on S3, AWS Glue for ETL operations, and Amazon QuickSight for business intelligence and visualization.
* Practice data ingestion, transformation, and analysis workflows in the AWS cloud environment.
* Understand cost optimization and performance tuning strategies for analytics workloads on AWS.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - **Practice:** Data Lake on AWS.  <br>&emsp; + Understand data lake architecture on AWS using S3 as the data lake storage layer. <br>&emsp; + Learn about data ingestion, cataloging, and querying patterns. <br>&emsp; +  Explore integration between S3, Glue, and Athena for analytics.                                                                                                 | 10/20/2025 | 10/20/2025      | [Data Lake on AWS](https://000035.awsstudygroup.com/) |
| 3   | -   **Practice:** Amazon DynamoDB Immersion Day.  <br>&emsp; + Deep dive into DynamoDB core concepts: tables, items, attributes, primary keys, and indexes. <br>&emsp; + Practice creating tables, inserting data, and querying with partition keys and sort keys. <br>&emsp; +  Understand DynamoDB capacity modes (on-demand vs provisioned) and pricing models.                                            | 10/21/2025 | 10/21/2025      |  [Amazon DynamoDB Immersion Day](https://000039.awsstudygroup.com/)  |
| 4   | **Practice:** Cost and performance analysis with AWS Glue and Amazon Athena.  <br>&emsp; + Use AWS Glue to catalog data stored in S3 and create data catalogs. <br>&emsp; + Run SQL queries on S3 data using Amazon Athena. <br>&emsp; +  Analyze cost implications and optimize query performance. <br>&emsp; + Understand partitioning strategies for cost-effective analytics. <br>   **Practice:** Work with Amazon DynamoDB. <br>&emsp; + Create DynamoDB tables with appropriate key schemas. <br>&emsp; + Perform CRUD operations (Create, Read, Update, Delete) on DynamoDB items. <br>&emsp; + Work with Global Secondary Indexes (GSI) and Local Secondary Indexes (LSI). <br>&emsp; + Practice querying and scanning operations, understanding the differences.   | 10/22/2025 | 10/22/2025      |[Cost and performance analysis with AWS Glue and Amazon Athena ](https://000040.awsstudygroup.com/) <br> [Work with Amazon DynamoDB](https://000060.awsstudygroup.com/) |
| 5   | - **Practice:** Building a Datalake with Your Data.  <br>&emsp; + Build a complete data lake solution using AWS services. <br>&emsp; + Implement data ingestion pipelines. <br>&emsp; + Set up data transformation workflows with AWS Glue.  <br>&emsp; +  Create analytics-ready datasets for downstream consumption. <br> - **Practice:** Analytics on AWS workshop.  <br>&emsp; + Comprehensive workshop covering the full analytics stack on AWS.  <br>&emsp; + Integrate multiple services: S3, Glue, Athena, and visualization tools.  <br>&emsp; +  Build end-to-end analytics solutions from raw data to insights.                          | 10/23/2025 | 10/23/2025      | [Building a Datalake with Your Data ](https://000070.awsstudygroup.com/) <br> [Analytics on AWS workshop](https://000072.awsstudygroup.com/) |
| 6   | - **Practice:** Get started with QuickSight. <br>&emsp; + Create visualizations and dashboards using Amazon QuickSight. <br>&emsp; + Connect QuickSight to various data sources (S3, Athena, RDS, etc.). <br>&emsp; + Use AWS Database Migration Service (DMS) to migrate data .  <br>&emsp; + Build interactive reports and share insights with stakeholders.                                                                        | 10/24/2025 | 10/24/2025      | [Get started with Quick Sight ](https://000073.awsstudygroup.com/) |


### Week 7 Achievements:

* Gained comprehensive understanding of Amazon DynamoDB:

  * DynamoDB as a fully managed, serverless NoSQL database service with single-digit millisecond latency.
  * Key concepts: tables, items, attributes, primary keys (partition key + optional sort key), and data modeling best practices.
  * Global Secondary Indexes (GSI) and Local Secondary Indexes (LSI) for flexible query patterns.
  * Capacity modes: on-demand (pay-per-request) vs provisioned (reserved capacity) and when to use each.
  * DynamoDB Streams for real-time data processing and change data capture.
* Got more experience on Data Lake architecture on AWS:

  * Amazon S3 as the foundation for data lake storage with lifecycle policies, versioning, and encryption.
  * Data lake architecture patterns: raw zone, processed zone, and curated zone.
  * Data ingestion strategies: batch uploads, streaming data, and integration with various data sources.
  * Best practices for organizing data in S3: partitioning, naming conventions, and folder structures.
* Understood more about AWS Analytics services:

  * AWS Glue: Serverless ETL service for discovering, cataloging, and transforming data.
      * Glue Data Catalog as a centralized metadata repository.
      * Glue ETL jobs for data transformation using Apache Spark.
      * Glue Crawlers for automatic schema discovery.
  * Amazon Athena: Serverless interactive SQL query service for analyzing data in S3.
      * Pay-per-query pricing model and cost optimization strategies.
      * Integration with Glue Data Catalog for schema-on-read queries.
      * Query performance optimization through partitioning and columnar formats (Parquet, ORC).
  * Amazon QuickSight: Cloud-native business intelligence and visualization service.
      * Creating dashboards, visualizations, and reports.
      * Connecting to various data sources (S3, Athena, RDS, Redshift, etc.).
      * Sharing insights with teams and embedding analytics in applications.

