# Infrastructure as Code Project with Ansible and Terraform

This project aims to deploy an environment on AWS that supports a backend with Python using Infrastructure as Code (IaC) principles. It utilizes Ansible for configuration management and Terraform for provisioning infrastructure resources on AWS.

## Table of Contents

- [Overview](#Overview)
- [Prerequisites](#Prerequisites)
- [Directory Structure](#Directory-Structure)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

This project automates the deployment of infrastructure components required to support a Python backend application on AWS. It leverages Terraform to provision infrastructure resources such as EC2 instances, VPC, Subnets, Security Groups, etc., and Ansible for configuration management tasks such as installing dependencies, configuring services, and deploying applications.

## Prerequisites

Before you begin, ensure you have the following prerequisites installed:

- [Terraform](https://www.terraform.io/) (>= 0.12)
- [Ansible](https://www.ansible.com/) (>= 2.10)
- [AWS CLI](https://aws.amazon.com/cli/) configured with appropriate permissions
- Python 3.x

## Directory Structure

The directory structure of this project is organized as follows:

```
├── ansible/ # Ansible playbooks and configuration files
│ ├── roles/ # Ansible roles for configuring servers
│ └── playbook.yml # Main Ansible playbook for server configuration
├── terraform/ # Terraform configuration files
│ ├── main.tf # Main Terraform configuration file
│ ├── variables.tf # Terraform variables
│ └── outputs.tf # Terraform outputs
└── README.md # Project README file
```

## Usage

1. **Clone the repository:**

```bash
git clone https://github.com/your-username/your-repo.git
cd your-repo
```

2. **Set up AWS credentials:**
```
Ensure you have AWS credentials configured either via environment variables, AWS CLI, or AWS credentials file.
```
3. **Configure Terraform:**
```
Edit terraform/variables.tf file to customize the Terraform variables according to your requirements.
```
4. **Initialize Terraform:**

```bash
cd terraform
terraform init
```

5. **Plan and Apply Terraform changes:**
```bash
terraform plan
terraform apply
```
6. **Run Ansible playbook:**
```bash
cd ../ansible
ansible-playbook playbook.yml
```

# Contributing
Contributions are welcome! Feel free to open issues or pull requests for any improvements, bug fixes, or new features.

# License
This project is licensed under the MIT License.

```
You can copy and paste this code directly into your README.md file. Make sure to replace placeholders like `your-username` and `your-repo` with your actual GitHub username and repository name.
```
