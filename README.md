
# AWS Resource Listing Automation Script

# Overview

This project provides a Bash automation script (aws_resource_list.sh) to list various AWS resources in a specific region. Instead of running multiple AWS CLI commands manually, this script allows you to quickly retrieve information about services like EC2, S3, RDS, IAM, Lambda, etc.

It is useful for:

Cloud Engineers and DevOps Engineers managing AWS infrastructure

Students and beginners learning AWS CLI automation

Audit and monitoring of AWS resources

# Features

The script currently supports the following AWS services:

• EC2 Instances

• RDS Databases

• S3 Buckets

• CloudFront Distributions

• VPCs

• IAM Users

• Route53 Hosted Zones

• CloudWatch Alarms

• CloudFormation Stacks

• Lambda Functions

• SNS Topics

• SQS Queues

• DynamoDB Tables

• EBS Volumes

# Prerequisites

Before running this script, make sure you have:

-Linux / MacOS / WSL environment

-AWS CLI installed → Install Guide

-AWS CLI configured with your credentials:

-aws configure

# Usage
Clone the repository-->git clone https://github.com/<your-username>/aws-resource-listing.git
                      cd aws-resource-listing

Make the script executable-->chmod +x aws_resource_list.sh

Run the script-->./aws_resource_list.sh <aws_region> <aws_service>

Example
./aws_resource_list.sh us-east-1 ec2


This will list all EC2 instances in the us-east-1 region.

# Example Outputs

EC2

Listing EC2 Instances in us-east-1
{
    "Reservations": [
        {
            "Instances": [
                {
                    "InstanceId": "i-0abcd1234efgh5678",
                    "State": { "Name": "running" },
                    "InstanceType": "t2.micro"
                }
            ]
        }
    ]
}


S3

Listing S3 Buckets
{
    "Buckets": [
        {
            "Name": "my-first-bucket",
            "CreationDate": "2024-01-01T10:00:00.000Z"
        }
    ]
}

