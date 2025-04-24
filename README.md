# Terraform AWS Project

This repository contains Terraform configurations to set up and manage AWS resources like EC2, S3, VPC, and more. It demonstrates the power of Infrastructure as Code (IaC) for automating the provisioning and management of AWS resources using Terraform.

## Features

- **EC2 Instances**: Create, configure, and manage EC2 instances.
- **S3 Buckets**: Automate the creation and management of S3 buckets.
- **VPC**: Set up and manage Virtual Private Cloud (VPC) resources.
- **Security Groups**: Configure security groups to control access.
- **IAM**: Manage IAM roles, policies, and permissions.

## Prerequisites

- **AWS Account**: You need an AWS account with the necessary IAM permissions to create resources.
- **Terraform**: Install Terraform on your local machine.
- **AWS CLI**: Configure AWS CLI with proper credentials.

## Installation

1. Clone this repository:

```bash
git clone https://github.com/ToxicStarboy/terraform-aws-project.git
cd terraform-aws-project
```

2. Initialize Terraform:

```bash
terraform init
```

3. Configure AWS credentials (if not already done):

```bash
aws configure
```

4. Run Terraform to apply the configuration:

```bash
terraform apply
```

## Usage

This project sets up the following AWS resources:

- **EC2 Instances**: A specified number of EC2 instances in the desired region.
- **S3 Buckets**: Automatically created buckets for storage.
- **VPC and Subnets**: A VPC with public and private subnets.

## Cleanup

To destroy all the resources created by this project:

```bash
terraform destroy
```

> Be sure to confirm the destruction of resources when prompted.

## Notes

- Customize the Terraform variables as needed, especially for region, instance types, and AMI IDs.
- Ensure that you have the proper IAM permissions to create and manage AWS resources.
- This project is for demonstration purposes. Always check for best practices before using in production environments.
