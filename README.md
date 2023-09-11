# Creating a Simple ETL Pipeline Using Airflow and Reddit API





# Overview

+ The goal of the project is  to create a simple ETL pipeline using Airflow and Reddit API. In this pipeline, I have extracted data from Reddit API, transformed it, and loaded it into an AWS S3 bucket using s3fs. 

+ I have used an  AWS EC2 instance to configure Airflow, and create a DAG with a task to schedule the ETL script to run. 

+ An IAM Role is assigned to the AWS EC2 instance with a policy to allow AWS S3 access. Finally the Airflow DAG is set to run on EC2 instance which initiates the ETL Pipeline. 


# Services used
+ Amazon S3: Amazon S3 is an object storage service that provides manufacturing scalability, data availability, security, and performance.
+ AWS IAM: This is nothing but identity and access management which enables us to manage access to AWS services and resources securely.
+ AWS EC2: Enables you to launch and manage virtual machines, known as instances.
+ Airflow : Airflow is an workflow orchestration tool, we can build schedule and monitor data pipelines.

# Files
+ reddit_etl.py: This file contains the Python ETL script for extracting, transforming, and loading data from Reddit API to AWS S3 using s3fs.
+ reddit_dag.py: This file contains the DAG and task definitions for Airflow.
