---
title: "Database vs Data Warehouse vs Data Lake"
excerpt: "Here I have listed down my understanding between Database, Data Warehouse and Data Lake"
permalink: /posts/blog1/
collection: posts
tags:
  - cool posts
  - category1
  - category2
---

**Database:** Generally refers to a structured collection of data (structured data) optimised for efficient transactional processing.(OLTP - online transaction processing)

**Data Warehouse:** A specialised database designed for the efficient querying and analysis of large volumes of historical data, often used for business intelligence/analysis (used for analytical processing). The moment we run complex queries with an intent to do some analysis, the day to day transactions become slow and users get impacted. So that's why we don't want to complicate the database with many analytical queries. That's why we take the data from the database and migrate the data to the data warehouse. We can get data from multiple data sources. 

Data Warehouse also deals with Structured Data. Storage Costs are high but lesser than Databases.

Data Warehouse(OLAP) - Online Analytical Processing follows ETL. So here the transformation is a complex process. So before even loading the data into the data warehouse we need to get the data in a desirable format by making transformations. So ETL approach reduces our flexibility as we do not know what transformations we can do on the data. This is where Data lake comes in handy.

Eg: Teradata

**Data Lake:** Data is present in raw format. (It can be structured and unstructured)  It follows ELT (where  before loading we don't think of any transformation ) A storage repository that can hold large amounts of raw data in its native format, providing flexibility for diverse data types and advanced analytics. The storage cost is so low(cost effective) Schema on Read.

First we put a file and then we create a structure to visualise data but in the previous database and data warehouse it follows schema on write. It gives so much flexibility in using all the raw data whenever required, any teams can make use of data and later make transformations as needed

Eg: Structured data (rows and columns) from relational databases, semi-structured data (CSV, logs, XML, JSON), unstructured data (emails, documents, PDFs), and binary data (pictures, audio, video) are some examples which data lake can include.
