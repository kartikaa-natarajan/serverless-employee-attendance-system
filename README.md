# Serverless Employee Face Recognition & Attendance Management System

An AWS serverless team project developed during my AWS Cloud Internship at F13 Technologies.

## Project Overview

The project focuses on automating employee attendance using face recognition and AWS cloud services. It includes an administrator dashboard for employee registration and attendance monitoring, along with an employee interface for capturing attendance images.

This repository showcases the system architecture, AWS configurations, application screenshots, and workflow documented during the internship.

## Architecture

![AWS Serverless Architecture](architecture/aws-architecture.png)

The architecture combines serverless compute, cloud storage, authentication, face comparison, database management, and scheduled automation.

## Key Features

- Employee registration and reference image storage
- Administrator authentication
- Face comparison for attendance verification
- Automated attendance recording
- Attendance dashboard with employee status and records
- Scheduled attendance log archival
- Temporary image cleanup

## AWS Services Used

| Service | Purpose |
|---|---|
| Amazon Cognito | Administrator authentication |
| Amazon API Gateway | API endpoints |
| AWS Lambda | Backend processing and automation |
| Amazon Rekognition | Face comparison |
| Amazon DynamoDB | Employee and attendance records |
| Amazon S3 | Image storage, archives, and frontend hosting |
| Amazon EventBridge | Scheduled tasks |
| Amazon CloudWatch | Logs and monitoring |
| AWS IAM | Permissions and access control |

## Application Screenshots

### 1. Attendance Dashboard

![Attendance Dashboard](screenshots/admin-dashboard.png)

The dashboard displays employee attendance statistics, attendance status, and individual records.

### 2. Employee Registration

![Add Employee](screenshots/add-employee.png)

The administrator can register an employee and provide a reference image.

### 3. Authentication

![Amazon Cognito Login](screenshots/cognito-login.png)

Administrator sign-in is handled using Amazon Cognito.

## AWS Implementation

### API Gateway
![API Gateway](screenshots/api-gateway.png)

Provides endpoints for communication between the frontend applications and backend functions.

### AWS Lambda
![Lambda Functions](screenshots/lambda-functions.png)

The backend uses separate functions for registration, image processing, attendance recording, dashboard data, archival, and cleanup.

### Amazon S3
![S3 Storage](screenshots/s3-storage.png)

Stores reference images, temporary attendance images, archived logs, and frontend files.

### Amazon DynamoDB
![DynamoDB Tables](screenshots/dynamodb-tables.png)

Stores employee information and attendance records.

### Amazon EventBridge
![EventBridge Schedules](screenshots/eventbridge-schedules.png)

Schedules background tasks for attendance archival and temporary image cleanup.

### Amazon CloudWatch
![CloudWatch Logs](screenshots/cloudwatch-logs.png)

Provides logs for monitoring and troubleshooting Lambda execution.

## Attendance Workflow

1. The administrator signs in and registers employees.
2. Employee details and reference images are stored in AWS.
3. The employee captures an image through the web interface.
4. AWS Lambda invokes Amazon Rekognition to compare the images.
5. If the face comparison succeeds, attendance is recorded in DynamoDB.
6. The administrator views the updated attendance information on the dashboard.
7. Scheduled processes archive records and clean up temporary images.

## Technologies

- AWS
- Python
- HTML, CSS, and JavaScript
- Serverless architecture
- Event-driven processing

## My Internship Experience

Working on this collaborative project helped me understand how AWS services can be integrated to build a cloud-based application. It provided exposure to serverless architecture, storage, databases, authentication, AI services, and monitoring.

## Project Status

This repository is a documentation and implementation showcase of the internship team project. It contains selected screenshots and descriptions of the system. A live public demo is not currently available.

## Acknowledgement

Developed collaboratively with my teammates during my AWS Cloud Internship at F13 Technologies, with guidance from our industry mentor.
