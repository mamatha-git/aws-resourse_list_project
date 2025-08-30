# aws-resourse_list_project


# AWS Resource Listing Automation Script

This project is a Bash automation script that lists resources across multiple AWS services in a given region. The script helps cloud engineers and DevOps professionals quickly retrieve resource details without navigating through the AWS Management Console.

✅ Features

Supports 14 AWS services including EC2, RDS, S3, CloudFront, VPC, IAM, Route53, CloudWatch, CloudFormation, Lambda, SNS, SQS, DynamoDB, and EBS.

Accepts AWS region and service name as command-line arguments.

Validates AWS CLI installation and configuration before execution.

Provides simple, automated resource discovery for auditing and monitoring.

🚀 Usage
./aws_resource_list.sh <aws_region> <aws_service>


Example:

./aws_resource_list.sh us-east-1 ec2

📌 Key Benefits

Saves time by automating repetitive AWS resource listing tasks.

Ensures consistency in fetching details across services.

Useful for cloud audits, troubleshooting, and learning AWS CLI.
