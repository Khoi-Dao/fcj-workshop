---
title: "Week 6 Worklog"
date: 2025-09-10
weight: 1
chapter: false
pre: " <b> 1.6. </b> "
---



### Week 6 Objectives:

* Review fundamental Database Concepts: relational model, primary/foreign keys, ACID, normalization, OLTP vs OLAP.
* Understand Amazon RDS as a managed relational database service on AWS: engines, Multi-AZ, read replicas, backup, and scaling.
* Learn the benefits of Amazon Aurora compared to standard RDS engines: performance, high availability, automatic storage scaling, MySQL/PostgreSQL compatibility.
* Get familiar with Amazon Redshift as a petabyte-scale data warehouse for analytics, and distinguish it from RDS (OLTP workloads).
* Learn how Amazon ElastiCache (Redis / Memcached) provides an in-memory cache layer to reduce latency and offload backend databases.
* Practice Database Schema Conversion & Migration using AWS DMS and AWS Schema Conversion Tool (SCT) for moving databases to AWS.

### Tasks to be carried out this week:
| Day | Task                                                                                                                                                                                                   | Start Date | Completion Date | Reference Material                        |
| --- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------------ | ---------- | --------------- | ----------------------------------------- |
| 2   | - Review Database Concepts : relational model, ACID, transactions, indexing, normalization, OLTP vs OLAP. <br> - Map traditional on-premises database concepts to AWS cloud services.                                                                                                   | 10/13/2025 | 10/13/2025      | [AWS Study group Youtube Video](https://www.youtube.com/watch?v=OOD2RwWuLRw&list=PLahN4TLWtox2a3vElknwzU_urND8hLn1i&index=217) |
| 3   | - Study Amazon RDS & Amazon Aurora theory . <br> - Learn about supported engines, Multi-AZ, automated backups, snapshots, read replicas, and scaling. <br> - Compare RDS vs Aurora in terms of performance, availability, and cost.                                             | 10/14/2025 | 10/14/2025      |  [AWS AmazonRDS user guide](https://docs.aws.amazon.com/AmazonRDS/latest/UserGuide/Welcome.html) <br> [AWS AmazonRDS Aurora document](https://aws.amazon.com/rds/aurora/) |
| 4   | - Study Amazon Redshift & Amazon ElastiCache . <br> - Distinguish OLTP (RDS/Aurora) vs OLAP (Redshift) and in-memory cache layer (ElastiCache). <br> - Explore common use cases: data warehouse & BI, caching sessions, leaderboard, rate limiting, etc. | 10/15/2025 | 10/15/2025      |[Info about AWS Redshift ](https://aws.amazon.com/redshift/) <br> [Info about AWS Elasticache](https://aws.amazon.com/elasticache/) |
| 5   | - **Practice:** <br>&emsp; + Module 06-Lab 5 – Amazon Relational Database Service (Amazon RDS). <br>&emsp; + Create an RDS instance, configure security group, parameter group, backups. <br>&emsp; + Connect from a client, run queries, and test behavior                             | 10/16/2025 | 10/16/2025      | [Amazon Relational Database Service (Amazon RDS) ](https://000005.awsstudygroup.com/) |
| 6   | - **Practice:** <br>&emsp; + Module 06-Lab 43 – Database Schema Conversion & Migration. <br>&emsp; + Use AWS Schema Conversion Tool (SCT) to analyze and convert schema from source DB to RDS/Aurora/Redshift target. <br>&emsp; + Use AWS Database Migration Service (DMS) to migrate data .  <br>  -  Summarize and review all AWS Database Services .                                                                         | 10/17/2025 | 10/17/2025      | [Database Schema Conversion & Migration ](https://000043.awsstudygroup.com/) |


### Week 6 Achievements:

* Consolidated understanding of core database concepts:

  * Relational tables, primary/foreign keys, relational integrity, and basic indexing.
  * ACID properties of transactions and why they matter in OLTP workloads.
  * Clear distinction between OLTP vs OLAP and how this maps to AWS services.

* Gained hands-on familiarity with Amazon RDS:

  * Created and managed RDS instances via AWS Management Console.
  * Reviewed supported engines (MySQL, PostgreSQL, MariaDB, Oracle, SQL Server, Aurora) and their typical use cases.
  * Practiced configuring Multi-AZ, automated backups, snapshots, monitoring, and basic scaling options.
* Understood the strengths of Amazon Aurora:

  * Aurora as a cloud-native, MySQL/PostgreSQL-compatible database with significantly improved performance over standard engines.
  * Aurora DB cluster architecture, with a distributed storage layer across multiple AZs.
  * Reader and writer endpoints, automatic storage scaling, and high availability design.
* Understand the usage of Amazon Redshift & ElastiCache:

  * Redshift as a columnar, petabyte-scale data warehouse optimized for analytics and BI workloads.
  * How Redshift differs from RDS/Aurora: optimized for complex queries over large datasets rather than transactional workloads.
  * ElastiCache (Redis/Memcached) as a fully managed, low-latency in-memory cache layer to increase throughput and reduce load on backend databases.

