# AWS Project 1 – Static Website Hosting
To host a static website in Amazon S3 and distribute it securely using Amazon CloudFront with HTTPS.
Services used
Amazon S3
Amazon CloudFront
CloudFront Origin Access Control
Configuration
S3 Bucket:
aws-project-antra-2026

Website file:
index.html

CloudFront:
Enabled

Default Root Object:
index.html

Viewer Protocol:
Redirect HTTP to HTTPS

Origin Access:
Origin Access Control

Result
The website was successfully uploaded to Amazon S3 and configured as the origin for an Amazon CloudFront distribution. The default root object was configured as index.html. HTTPS was enabled using the CloudFront viewer protocol policy. The website was successfully accessed through the CloudFront distribution URL.

# AWS Project 2 – EC2 Apache Web Server
## Objective
To deploy a web server using Amazon EC2 and Apache HTTP Server.

## AWS Services Used
- Amazon EC2
- Amazon Linux
- Apache HTTP Server
- EC2 Security Group

## Architecture
User
  ↓
Security Group
  ↓
EC2 Linux
  ↓
Apache Web Server
  ↓
HTML Webpage

## Configuration
Region: ap-south-1 (Mumbai)
HTTP: Port 80
HTTPS: Port 443
SSH: Port 22

## Testing
- Apache service checked
- curl localhost tested
- Website opened in browser
- Security Group checked

## Result
Apache was successfully configured on an Amazon EC2 Linux instance
and the custom webpage was successfully served.

# AWS Project 3 – Student Management System
## Objective
To create a cloud-based student management system using
Amazon EC2, Apache and Amazon DynamoDB.

## AWS Services Used
- Amazon EC2
- Apache HTTP Server
- Amazon DynamoDB
- AWS CloudShell
- EC2 Security Groups

## Architecture

User
  ↓
EC2 + Apache
  ↓
DynamoDB
  ↑
CloudShell / AWS CLI

## DynamoDB Table

Table Name: StudentManagement
Partition Key: StudentID

Attributes:
- StudentID
- Name
- Course
- Year
- Email

## Database Operations

- PutItem – Add student
- GetItem – Retrieve student
- Scan – Display records
- UpdateItem – Update student information

## Testing

S001 was retrieved successfully.
Multiple student records were displayed using Scan.
The Year value of S001 was updated to 4.

## Result

The StudentManagement DynamoDB table was successfully created
and student records were inserted, retrieved, scanned and updated.
