# YouTube Data Engineering and Analytics Project
## Overview
This project is designed to securely manage, process, and analyze both structured and semi-structured YouTube video data. By leveraging cloud-based services, the project focuses on categorizing videos and identifying trends through key performance metrics such as views, likes, and engagement. The solution emphasizes scalability, automation, and efficient data handling to support data-driven insights.

## Project Objectives
The primary objectives of this project are as follows:

### Data Ingestion:
Implement a mechanism to ingest data from various sources, including APIs and external datasets, ensuring secure and efficient data collection.

### ETL System:
Transform raw data into a structured format by applying cleaning, standardization, and schema alignment to prepare it for storage and analysis.

### Data Lake:
Utilize a centralized repository to store data from multiple sources, making it accessible for analytics and scalable as data volume increases.

### Scalability:
Design a system that can handle increasing data volume without compromising performance by leveraging cloud services.

### Cloud Processing:
Process and store large datasets in a cloud environment to take advantage of scalable computing power and storage solutions. AWS is used for cloud infrastructure in this project.

### Reporting & Insights:
Build interactive dashboards to visualize trends and answer key business questions, providing actionable insights based on video performance metrics.

## Services & Tools Used
The project employs the following cloud services and technologies to implement the data pipeline:

### Amazon S3:
Object storage service for scalable, secure, and high-performance data storage.

### AWS IAM (Identity and Access Management):
Service to securely control access to AWS services and resources through role-based permissions.

### Amazon QuickSight:
A cloud-native business intelligence (BI) tool used to create interactive dashboards and data visualizations.

### AWS Glue:
Serverless data integration service for discovering, preparing, and transforming data at scale.

### AWS Lambda:
A serverless compute service to execute code in response to data events, enabling automation of data ingestion and processing tasks.

### Amazon Athena:
Interactive query service that allows SQL queries on data stored in S3 without the need to load it into a separate database.

## Dataset Description
The dataset used for this project is sourced from Kaggle and contains daily statistics on trending YouTube videos across multiple countries. Each dataset file represents data from a specific region and includes information such as:

Video title, channel name, publication date, and tags
Performance metrics: views, likes, dislikes, and comment count
Video description and a category identifier (unique to each region)
You can find the dataset here: YouTube Trending Videos Dataset on Kaggle

## Architecture Overview
The solution architecture follows a typical data engineering workflow designed for cloud-based scalability and automation. The main components include:

### Data Source:
YouTube API and Kaggle dataset provide the raw data for ingestion.
https://www.kaggle.com/datasets/datasnaek/youtube-new

### Data Ingestion:
Data is ingested using Lambda functions and AWS Glue jobs, then stored in S3.

### Data Transformation:
AWS Glue performs ETL operations, transforming raw JSON/CSV data into a standardized format suitable for querying and analysis.

### Data Storage:
Cleaned and processed data is stored in S3 as part of a data lake architecture.

### Data Querying & Analysis:
Amazon Athena enables interactive SQL querying of the data stored in S3 without requiring additional data loading steps.

### Visualization:
Amazon QuickSight provides a dashboard to visualize trends and insights based on video performance metrics.

![ArchitectureDiagram](https://github.com/user-attachments/assets/0751d81d-1be2-4a5d-b0f6-1e2f6b4d5abe)
