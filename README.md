# AWS Cloud Data Engineer Portfolio

This repository contains a series of end-to-end projects and study artifacts demonstrating my proficiency with AWS data services, infrastructure as code (Terraform), CI/CD automation, and monitoring. Over a 6-week sprint (June 1 – July 18, 2025), I built, documented, and validated the following four core projects:

- **Project 1: Serverless ETL → Redshift**  
  Ingest raw CSV files into S3, catalog them with AWS Glue, transform to Parquet via a Glue PySpark job, and load the results into Amazon Redshift Serverless. Includes Glue Crawler configuration, Glue ETL script, Redshift CTAS SQL, and screenshots of successful data validation in Athena and Redshift.

- **Project 2: Real-Time Streaming Pipeline**  
  Create a Kinesis Data Stream that receives JSON events, process and filter them using an AWS Lambda function, land the output as JSON/Parquet in S3, and query the results with Athena. A QuickSight dashboard visualizes streaming data in near-real time. Includes producer and processor scripts, Glue/Athena table configuration, and QuickSight chart snapshots.

- **Project 3: Infrastructure as Code (Terraform)**  
  Use Terraform modules to provision all AWS resources needed for Projects 1 & 2:  
  - S3 buckets for raw and processed data  
  - IAM roles and policies for Glue, Lambda, and Redshift  
  - Redshift Serverless namespace and workgroup  
  - Kinesis Data Stream  
  - AWS Lambda function for streaming processing  
  Documentation shows `terraform init`, `plan`, `apply`, and teardown steps, with screenshots of resources in the AWS Console.

- **Project 4: CI/CD & Monitoring**  
  Automate deployment of Terraform code and Python scripts via GitHub Actions. Build a local Airflow DAG (optional) to orchestrate the Glue → Athena workflow. Set up Grafana to visualize CloudWatch metrics for Glue job runtimes and Redshift CPU utilization. Includes GitHub Actions workflow YAML, Airflow DAG code, and Grafana dashboard screenshots.

Each project folder contains step-by-step instructions, source code, configuration files, and images/screenshots that document how services were configured and validated. By the end of July 2025, this portfolio also includes my passed **AWS Certified Data Engineer – Associate** badge.

---
