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
<img width="1178" height="658" alt="image" src="https://github.com/user-attachments/assets/3779b1d1-c626-4818-b6b1-5b424b8311ce" />
These credentials were configured in AWS CLI using:<br>
aws configure<br>
<img width="1116" height="170" alt="image" src="https://github.com/user-attachments/assets/1bb95cf9-43e8-4d25-aea9-f340cba97cbd" />

## Step 4: Attached IAM Permissions
Attached a custom IAM policy in JSON format to allow Terraform to create IAM users.<br>
<img width="1273" height="587" alt="image" src="https://github.com/user-attachments/assets/2d263902-0196-4816-a996-c4d507ebf50c" />

## Step 5: Installed Terraform
Installed Terraform on the Linux server and verified installation using:<br>
terraform -version<br>
<img width="1908" height="337" alt="image" src="https://github.com/user-attachments/assets/4940216c-ca2b-4f00-8d90-2fee3da3fe8f" />

## Step 6: Created Terraform Configuration File
Created a file named:<br>
main.tf<br>
Terraform configuration:<br>
<img width="556" height="193" alt="image" src="https://github.com/user-attachments/assets/e9aaabc4-a73d-4dae-a5d3-0657422c501d" />

# Terraform Commands Used
## Initialize Terraform
terraform init<br>
<img width="1106" height="440" alt="image" src="https://github.com/user-attachments/assets/255b2cf1-f6b8-4cb6-8bfe-5b01f51705b4" />
Purpose:<br>
Downloads AWS provider plugins<br>
Initializes Terraform working directory
## Validate Terraform File
terraform validate<br>
<img width="794" height="88" alt="image" src="https://github.com/user-attachments/assets/bf438a0b-4e22-4628-9eda-4e95d1c811ff" />
Purpose:<br>
Checks Terraform syntax<br>
Ensures configuration is valid
## Generate Execution Plan
terraform plan<br>
<img width="1814" height="539" alt="image" src="https://github.com/user-attachments/assets/43a7f187-f46e-4d2d-b382-5a38fdb76db5" />
Purpose:<br>
Shows resources Terraform will create<br>
Displays infrastructure changes before deployment
## Apply Terraform Configuration
terraform apply<br>
<img width="1790" height="539" alt="image" src="https://github.com/user-attachments/assets/74e88de5-effb-41d2-8ae0-f746e78455c0" />
Purpose:<br>
Creates AWS resources defined in Terraform file

# Output
Successfully created an AWS IAM user using Terraform automation.<br>
<img width="1260" height="418" alt="image" src="https://github.com/user-attachments/assets/cade33fa-422b-405e-8c9e-1c9231eedef6" />




