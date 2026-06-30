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

## ⚠️ Challenges Faced

### 1. Accidental Loss of Terraform Workstation

**Challenge**

During the learning process, I accidentally terminated the EC2 instance that was being used as my Terraform workstation, resulting in the loss of the local Terraform configuration files.

**Resolution**

I recreated the project structure using my implementation notes and documentation. This reinforced the importance of storing Infrastructure as Code in version control systems such as GitHub instead of relying on a single workstation.

**Key Takeaway**

Infrastructure should always be reproducible from source code.

---

### 2. AWS Authentication Verification

**Challenge**

Before provisioning resources, I needed to ensure Terraform could authenticate successfully with AWS.

**Resolution**

Configured AWS CLI credentials using `aws configure` and verified the authentication before running Terraform commands.

**Key Takeaway**

Always verify authentication before provisioning infrastructure.

---

### 3. Understanding the Infrastructure Lifecycle

**Challenge**

Initially, my focus was only on creating AWS resources.

**Resolution**

While implementing Terraform, I learned that Infrastructure as Code also includes planning, state verification, resource inspection, and infrastructure cleanup using `terraform destroy`.

**Key Takeaway**

Provisioning infrastructure is only one part of the complete Terraform lifecycle.

---
