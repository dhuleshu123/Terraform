# Terraform Configurations

A collection of Terraform configuration files, hands-on exercises, and mini-projects covering core Terraform concepts and AWS infrastructure provisioning.

## Repository Structure

### AWS Infrastructure & Services
* **`aws-IAM-management/`** – Managing AWS Identity and Access Management (IAM) users, roles, and policies.
* **`aws-ec2/`** – Provisioning and configuring Amazon EC2 instances.
* **`aws-s3/`** – Creating and managing Amazon S3 buckets and object configurations.
* **`aws-vpc/`** – Building custom Virtual Private Clouds (VPCs), subnets, route tables, and gateways.
* **`aws-vpc-ec2-nginx/`** – End-to-end setup deploying an EC2 instance inside a custom VPC running an Nginx web server.

### Core Terraform Concepts
* **`tf-variables/`** – Working with input variables, output values, and `.tfvars` files.
* **`tf-data-sources/`** – Querying and referencing existing cloud infrastructure using data blocks.
* **`tf-functions/`** – Examples using built-in Terraform functions for string, collection, and numeric manipulation.
* **`tf-operators-exps/`** – Using conditional expressions, `for` expressions, and logical/arithmetic operators.
* **`tf-multi-resources/`** – Scaling resources dynamically using `count` and `for_each` meta-arguments.
* **`tf-backend/`** – Configuring remote state storage and state locking (e.g., S3 + DynamoDB).
* **`tf-cli-workspace/`** – Managing multiple environments using Terraform CLI workspaces.
* **`tf-test/`** – Scratchpad and test configurations for experimenting with Terraform blocks.

### Modules & Projects
* **`tf-module-vpc/`** – Implementing VPC infrastructure using public/registry Terraform modules.
* **`tf-own-module-VPC/`** – Creating a reusable custom VPC module from scratch.
* **`testing-local-module/`** – Consuming and validating locally developed Terraform modules.
* **`proj-static-website/`** – Complete project setup for hosting a static website on AWS.

---

## Prerequisites

Before running any configurations in this repository, ensure you have:
1. **[Terraform](https://developer.hashicorp.com/terraform/install)** installed (`v1.0+` recommended).
2. **[AWS CLI](https://aws.amazon.com/cli/)** installed and configured with valid credentials (`aws configure`).
3. An active **AWS Account** with permissions to create IAM, EC2, S3, and VPC resources.

---

## Usage

1. **Clone the repository:**
   ```bash
   git clone https://github.com/dhuleshu123/mprashant-terraform-configs.git
   cd mprashant-terraform-configs
   ```

2. **Navigate to a specific topic or project directory:**
   ```bash
   cd aws-ec2
   ```

3. **Initialize Terraform:**
   ```bash
   terraform init
   ```

4. **Review the execution plan:**
   ```bash
   terraform plan
   ```

5. **Apply the configuration:**
   ```bash
   terraform apply
   ```

6. **Clean up resources when finished (to avoid AWS charges):**
   ```bash
   terraform destroy
   ```

---

## Disclaimer
> **Note:** Running these configurations will provision real resources in your AWS account, some of which may fall outside the AWS Free Tier. Always run `terraform destroy` after testing.

## Credits
Forked from [paulgitrepo/mprashant-terraform-configs](https://github.com/paulgitrepo/mprashant-terraform-configs).
