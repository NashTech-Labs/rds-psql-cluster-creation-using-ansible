# AWS-rds-psql-cluster-creation-using-ansible

This Ansible role automates the setup of an AWS RDS Aurora PostgreSQL cluster, including tasks for creating a new VPC with two subnets and a subnet group.

## Table of Contents

- [Introduction](#introduction)
- [Requirements](#requirements)
- [Installation](#installation)

## Introduction

This role streamlines the process of creating an RDS PostgreSQL cluster with a single instance. Additionally, it includes tasks for establishing a new VPC with two subnets and a subnet group, providing a comprehensive solution for database deployment on AWS.

**Note:** Replace `master_username` and `master_user_password` inside `/roles/rds_role/vars/main.yml` file.

## Requirements

Ensure you have the following prerequisites before using this role:
- Ansible installed on your control machine.
- AWS credentials configured with appropriate permissions.

## Installation

To use this Ansible role, follow these steps:
1. **Install the `community.aws` collection**:
   ```bash
   ansible-galaxy collection install community.aws

2. **Clone the repository** to your local machine:

   ```bash
   git clone https://github.com/your_username/aws-rds-psql-cluster-creation-using-ansible.git
   ```bash
   cd aws-rds-psql-cluster-creation-using-ansible/
   ```bash
   ansible-playbook playbook.yaml
