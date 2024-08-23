# AWS EKS Cluster Automation with Terraform

## Project Overview
This project automates the provisioning of an AWS Elastic Kubernetes Service (EKS) cluster using Terraform. The infrastructure includes a custom Virtual Private Cloud (VPC), IAM roles, worker nodes with auto-scaling, and state management using S3 and DynamoDB.

## Features
- **Infrastructure as Code (IaC):** Automates the deployment of AWS resources using Terraform.
- **VPC Configuration:** Creates a custom VPC with public and private subnets.
- **IAM Management:** Configures IAM roles and policies for secure access control.
- **Worker Nodes:** Deploys EKS worker nodes with auto-scaling capabilities.
- **State Management:** Utilizes S3 and DynamoDB for locking and maintaining the Terraform state.

## Prerequisites
- AWS Account
- Terraform (v1.x.x or higher)
- AWS CLI configured with appropriate access rights
- S3 bucket and DynamoDB table for state management

## Setup Instructions

1. **Clone the Repository:**
   ```bash
   git clone https://github.com/swatinath/AWS-EKS-Cluster-Automation.git
   cd AWS-EKS-Cluster-Automation
   ```

2. **Initialize Terraform:**
   ```bash
   terraform init
   ```

3. **Create an Execution Plan:**
   ```bash
   terraform plan
   ```

4. **Apply the Terraform Plan:**
   ```bash
   terraform apply
   ```

5. **Verify the Cluster:**
   After the deployment is complete, use `kubectl` to interact with your EKS cluster.

## File Structure
- **main.tf:** Core infrastructure definition.
- **variables.tf:** Input variables for customization.
- **outputs.tf:** Outputs of the Terraform execution.
- **provider.tf:** AWS provider configuration.

## Contributing
Feel free to submit issues or pull requests if you find a bug or want to add enhancements.

## License
This project is licensed under the MIT License.
