# Terraform AWS EC2 Provisioning

## 📖 Project Overview

This project demonstrates how I provisioned and managed AWS infrastructure using Terraform by implementing Infrastructure as Code (IaC). The project covers the complete infrastructure lifecycle—from configuring Terraform and AWS authentication to provisioning an EC2 instance, verifying the infrastructure state, and cleaning up resources.

---

## 🎯 Project Goal

The objective of this project was to understand and implement Infrastructure as Code (IaC) by provisioning an AWS EC2 instance using Terraform instead of creating resources manually through the AWS Management Console.

---

## 🚀 Implementation Journey

### Step 1 - Set Up the Terraform Workstation

- Launched an Ubuntu EC2 instance to use as the Terraform workstation.
- Connected to the instance using SSH.
- Installed Terraform and verified the installation.

📷 *Screenshot: Terraform installation and version verification*

---

### Step 2 - Configure AWS Authentication

- Created an IAM user with the required permissions.
- Configured AWS CLI credentials using `aws configure`.
- Verified successful authentication before provisioning infrastructure.

📷 *Screenshot: AWS CLI configuration*

---

### Step 3 - Initialize the Terraform Project

- Created the Terraform configuration files.
- Initialized the working directory using `terraform init`.
- Downloaded the required AWS provider plugins.

📷 *Screenshot: terraform init*

---

### Step 4 - Validate and Plan the Infrastructure

- Validated the Terraform configuration.
- Reviewed the execution plan using `terraform plan`.
- Verified the resources before provisioning.

📷 *Screenshot: terraform plan*

---

### Step 5 - Provision the EC2 Instance

- Applied the Terraform configuration using `terraform apply`.
- Successfully provisioned an AWS EC2 instance.
- Verified the instance from the AWS Management Console.

📷 *Screenshot: EC2 instance running*

---

### Step 6 - Verify the Terraform State

- Inspected the Terraform state after provisioning.
- Verified the managed resources using Terraform state commands.
- Confirmed that the infrastructure matched the Terraform configuration.

📷 *Screenshot: terraform state*

---

### Step 7 - Destroy the Infrastructure

- Destroyed all created AWS resources using `terraform destroy`.
- Verified that the infrastructure was cleaned up successfully.

📷 *Screenshot: terraform destroy*

---
