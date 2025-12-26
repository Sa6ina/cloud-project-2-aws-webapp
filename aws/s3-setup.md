\# S3 Setup – Cloud Project 2



\## Overview

This document describes the creation of an Amazon S3 bucket to host static content.

The setup was done using the AWS Management Console.



\## Bucket Configuration

\- Bucket Name: cloud-project-2-static-assets-<your-name>

\- Region: eu-central-1

\- Public Access: Enabled via Bucket Policy



\## Uploaded Object

\- File: index.html

\- Path: /

\- Content-Type: text/html



\## Access Configuration

Public read access was granted using a bucket policy that allows the s3:GetObject action

for all objects inside the bucket.



\## Result

The static HTML file is publicly accessible via the S3 object URL and displays

a simple web page hosted on Amazon S3.



