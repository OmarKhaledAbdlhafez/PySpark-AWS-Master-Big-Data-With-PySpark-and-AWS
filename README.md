# PySpark-AWS-Master-Big-Data-With-PySpark-and-AWS

# Change Data Capture / Replication Using PySpark and AWS

This repository contains a comprehensive implementation for Change Data Capture (CDC) and ongoing replication using PySpark and various AWS services. The project is designed to facilitate the movement and transformation of data between MySQL RDS and S3, ensuring that data is readily available for analytics and other applications.


## Introduction

This project demonstrates how to set up a data pipeline that captures ongoing changes in a MySQL RDS instance and replicates that data to an S3 bucket using AWS services such as DMS (Database Migration Service), Glue, and Lambda.

## Prerequisites

- AWS Account
- Basic knowledge of AWS services (RDS, S3, DMS, Glue, Lambda)
- Python 3.x installed
- PySpark installed

## Setup Instructions

### Creating RDS MySQL Instance

Create an RDS MySQL instance through the AWS Management Console or AWS CLI. Ensure to configure security groups and parameter groups according to your requirements.

### Creating S3 Bucket

Set up an S3 bucket where the data will be stored. This can be done via the AWS Management Console or CLI.

### Creating DMS Source Endpoint

Configure a DMS source endpoint pointing to your RDS MySQL instance.

### Creating DMS Destination Endpoint

Set up a DMS destination endpoint that points to your S3 bucket.

### Creating DMS Instance

Create a DMS replication instance to manage the data migration tasks.

### MySQL Workbench

Use MySQL Workbench to connect to your RDS instance and manage your database.

### Connecting with RDS and Dumping Data

Connect to the RDS instance using MySQL Workbench and dump the initial data as needed.

### Querying RDS

Run queries on the RDS instance to validate the data and structure.

### DMS Full Load

Perform a full load of data from RDS to S3 using DMS.

### DMS Replication Ongoing

Set up ongoing replication to capture changes in real-time.

### Stopping Instances

Learn how to stop DMS instances and manage costs.

### Glue Jobs

- **Full Load**: Create a Glue job for full load operations.
- **Change Capture**: Set up a Glue job for capturing changes.
- **CDC**: Implement a Glue job for Change Data Capture.

### Creating Lambda Function and Adding Trigger

Create a Lambda function to process data and add a trigger for automation.

### Checking Trigger

Verify that the trigger works correctly and processes events as expected.

### Getting S3 File Name in Lambda

Implement logic in your Lambda function to retrieve the file name from S3.

### Creating Glue Job

Set up additional Glue jobs to enhance data processing as needed.

### Adding Invoke for Glue Job

Configure your Lambda function to invoke Glue jobs when necessary.

### Testing Invoke

Test the invocation of Glue jobs using sample data.

### Writing Glue Shell Job

Develop Glue shell jobs to execute custom scripts.

## Pipelines

### Full Load Pipeline

Outline the steps and components involved in the full load pipeline from RDS to S3.

### Change Data Capture Pipeline

Detail the process for capturing ongoing changes and loading them into S3.

## License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
