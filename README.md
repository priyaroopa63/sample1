
# Diabos

Propelor is both the hardware that drives goods through seas and skies, but equally the desire that inspires us to propel businesses forward with an unstoppable sense of progress.


## Documentation

(https://minfytech-my.sharepoint.com/:w:/p/sreeram_daasetti/EffvlNNllo5KmUuPANJZ8EkB_p2s7zeqW_ZaPYBF_lnLCA?e=52qfaj)

## Tools used

| Phase | Tools & Technologies |
| :-------- | :------- |
|  Infrastructure Provisioning      | Terraform, Cloud Provider (AWS) |
| Deployment and Orchestration      | AWS Code Pipeline, EKS |


# Terraform Provisioning Project

This project uses Terraform to provision and manage infrastructure resources on AWS. It automates the deployment of infrastructure.

## Table of Contents

- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Configuration](#configuration)
- [Usage](#usage)
- [Terraform Modules](#terraform-modules)
- [Folder Structure](#folder-structure)
- [Variables](#variables)
- [Outputs](#outputs)


## Getting Started

### Prerequisites

Before you begin, ensure you have met the following requirements:

- [Terraform](https://www.terraform.io/) installed (version X.X.X)
- [Provider CLI](https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2.html) install and configure with your credentials

### Installation

1. Clone this repository:

   git clone https://github.com/viswanath2222/Modern-DevSecOps.git   
   cd terraform-provisioning

2. Initialize Terraform:
   
   terraform init

### Configuration

The Terraform configuration files are structured as follows:

main.tf: Defines the EC2 instance, VPC, subnet, security group, and key pair resources.

variables.tf: Declares the variables used in the Terraform configuration.

terraform.tfvars.example: Example variable values for your terraform.tfvars file.

outputs.tf: Defines the output values that Terraform will display after applying.

### Usage

To provision the infrastructure, follow these steps:

Review the variables.tf file and adjust any default values or settings as needed.

Run the following commands:

terraform init

terraform plan

terraform apply

Confirm the changes and apply the plan.


### Terraform Modules

This project uses the following Terraform modules:

Module Name: [ECS, RDS, VPC]


### Variables

Customize the terraform.tfvars file to set the following variables:

aws_access_key: Your AWS access key.

aws_secret_key: Your AWS secret key.

instance_type: EC2 instance type (e.g., "t2.micro").

ami_id: ID of the Amazon Machine Image (AMI) to use.

subnet_cidr_block: CIDR block for the subnet.

security_group_name: Name for the security group.

key_pair_name: Name for the EC2 key pair.


### Outputs

After applying the Terraform configuration, the outputs will be displayed.


