![image alt]()

# AWS Transaction Reconciliation System

## Overview

This project demonstrates an event-driven serverless architecture on AWS for processing financial transaction files.

When a transaction CSV file is uploaded to Amazon S3, AWS Lambda validates the records and sends a reconciliation report through Amazon SNS. CloudWatch captures logs and provides monitoring.

## Architecture

Transaction File
→ S3 Bucket
→ Lambda Function
→ SNS Topic
→ Email Notification

CloudWatch Logs

## AWS Services Used

- Amazon S3
- AWS Lambda
- Amazon SNS
- Amazon CloudWatch
- AWS IAM

## Features

- Automatic file processing
- Transaction validation
- Reconciliation reporting
- Email notifications
- CloudWatch logging

## Sample Validation Rules

- Negative transaction amounts are invalid
- Malformed records are flagged
- Processing summary is generated

## Sample Output

Total Records: 100

Valid Records: 95

Invalid Records: 5

## Future Improvements

- DynamoDB for storing results
- Step Functions workflow
- CloudWatch alarms
- Terraform deployment
