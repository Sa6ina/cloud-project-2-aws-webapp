\# EC2 Setup – Cloud Project 2



\## Overview

This document describes the creation of an EC2 instance acting as a public web server.

The instance was launched using the AWS Management Console.



\## Instance Configuration

\- Name: cloud-project-2-web-server

\- AMI: Amazon Linux 2023

\- Instance Type: t2.micro

\- Region: eu-central-1



\## Network Configuration

\- VPC: cloud-project-2-vpc

\- Subnet: cloud-project-2-public-subnet

\- Public IP: Enabled



\## Security Group

\- Name: cloud-project-2-sg



\### Inbound Rules

\- SSH (22) → My IP

\- HTTP (80) → 0.0.0.0/0



\## Web Server Setup

Nginx was installed using EC2 user data at launch.



\### User Data Script

```bash

\#!/bin/bash

yum update -y

yum install -y nginx

systemctl start nginx

systemctl enable nginx



