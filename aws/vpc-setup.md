\# VPC Setup – Cloud Project 2



\## Overview

This document describes the creation of a custom VPC using the AWS Management Console.

The VPC is designed to host public-facing resources such as a web server.



\## VPC Configuration

\- Name: cloud-project-2-vpc

\- CIDR Block: 10.0.0.0/16

\- Region: eu-central-1



\## Public Subnet

\- Name: cloud-project-2-public-subnet

\- CIDR Block: 10.0.1.0/24

\- Availability Zone: eu-central-1a



\## Internet Gateway

\- Name: cloud-project-2-igw

\- Attached to: cloud-project-2-vpc



\## Route Table

\- Name: cloud-project-2-public-rt

\- Route: 0.0.0.0/0 → Internet Gateway

\- Associated Subnet: cloud-project-2-public-subnet



\## Result

The public subnet now has full internet access and is ready to host EC2 instances.



