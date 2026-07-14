# Terraform AWS Infrastructure

This repository contains Terraform configurations to provision basic AWS infrastructure, including an EC2 instance and an S3 bucket.

## Features

- AWS Provider configuration
- EC2 Instance creation
- S3 Bucket creation
- Terraform Outputs
- Modular and easy-to-understand structure

## Project Structure

```
.
├── provider.tf      # AWS provider configuration
├── ec2.tf           # EC2 instance resource
├── s3.tf            # S3 bucket resource
├── outputs.tf       # Output values
├── variables.tf     # Input variables (optional)
├── terraform.tfvars # Variable values (optional)
└── README.md
```

## Prerequisites

- Terraform >= 1.0
- AWS CLI installed
- AWS account
- Configured AWS credentials

Configure credentials:

```bash
aws configure
```

## Usage

### 1. Clone the repository

```bash
git clone https://github.com/<your-username>/terraform-aws-infrastructure.git
cd terraform-aws-infrastructure
```

### 2. Initialize Terraform

```bash
terraform init
```

### 3. Validate configuration

```bash
terraform validate
```

### 4. Preview the execution plan

```bash
terraform plan
```

### 5. Deploy infrastructure

```bash
terraform apply
```

Type:

```
yes
```

when prompted.

## Outputs

After successful deployment, Terraform displays the configured outputs, such as:

- EC2 Instance ID
- EC2 Public IP
- S3 Bucket Name

You can also view outputs using:

```bash
terraform output
```

## Destroy Resources

To remove all provisioned resources:

```bash
terraform destroy
```

## Technologies Used

- Terraform
- AWS EC2
- AWS S3

## Author

Emaan Chaudhary
