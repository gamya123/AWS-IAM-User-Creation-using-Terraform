# AWS-IAM-User-Creation-using-Terraform
This project demonstrates how to create and manage an AWS IAM user using Terraform. The project was created as a beginner-level Infrastructure as Code (IaC) implementation to understand Terraform workflow and AWS integration.

# Technologies Used
Terraform<br>
AWS IAM<br>
AWS CLI<br>
Git & GitHub<br>
Linux (Amazon Linux EC2)

# Project Workflow
## Step 1: Created Terraform Server
Launched an EC2 instance in AWS.<br>
Connected to the server using SSH.<br>
Used the server as a Terraform execution environment.<br>

## Step 2: Created IAM User
Created an IAM user named:devops-user.<br>
This IAM user is used by Terraform to authenticate with AWS services.
<img width="1488" height="372" alt="image" src="https://github.com/user-attachments/assets/e6576e1e-2f1f-4f51-9462-f9b10aec8354" />

## Step 3: Generated Access Keys
Generated:<br>
Access Key ID<br>
Secret Access Key<br>
These credentials were configured in AWS CLI using:<br>
aws configure
