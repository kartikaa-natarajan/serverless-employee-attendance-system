# Serverless Employee Face Recognition & Attendance Management System

## Project Overview

This project demonstrates a serverless employee attendance management system developed collaboratively as part of an AWS Cloud Internship at F13 Technologies. It uses facial recognition to help identify registered employees and record attendance.

This repository contains the project architecture, AWS implementation screenshots, and project documentation. A live public demo is not currently available.

## Objectives

- Automate employee attendance using facial recognition.
- Provide an administrator interface for employee registration and attendance tracking.
- Store employee details and attendance records using AWS services.
- Use serverless components to reduce infrastructure management.

## AWS Services Used

- **Amazon Rekognition:** Face comparison for employee identification.
- **AWS Lambda:** Backend processing and automation.
- **Amazon API Gateway:** API endpoints for application requests.
- **Amazon DynamoDB:** Employee details and attendance records.
- **Amazon S3:** Image storage and related assets.
- **Amazon Cognito:** Administrator authentication.
- **Amazon EventBridge:** Scheduled tasks.
- **Amazon CloudWatch:** Logs and monitoring.
- **AWS IAM:** Access permissions and security.

## System Workflow

1. The administrator signs in and registers an employee.
2. Employee information and reference images are stored using AWS services.
3. The employee's face is captured for verification.
4. AWS Lambda processes the request and uses Amazon Rekognition to compare the face with the registered reference.
5. When a match is successful, attendance information is recorded in DynamoDB.
6. The administrator can view employee and attendance information through the dashboard.
7. Scheduled tasks support configured archival or cleanup activities.

## Architecture

![AWS Architecture Diagram](architecture/aws-architecture.png)

## Implementation Screenshots

### 1. Administrator Dashboard
![Admin Dashboard](screenshots/01-admin-dashboard.png)

### 2. Add Employee
![Add Employee](screenshots/02-add-employee.png)

### 3. Attendance Result
![Attendance Result](screenshots/03-updated-admin-dashboard.png)

### 4. Administrator Login
![Cognito Login](screenshots/04-cognito-login.png)

### 5. API Gateway
![API Gateway](screenshots/04-api-gateway.png)

### 6. CloudWatch Logs
![CloudWatch Logs](screenshots/06-cloudwatch-logs.png)

### 7. DynamoDB Tables
![DynamoDB Tables](screenshots/07-dynamodb-tables.png)

### 8. EventBridge Schedules
![EventBridge Schedules](screenshots/08-event-bridge-schedules.png)

### 9. Lambda Functions
![Lambda Functions](screenshots/09-lambda-functions.png)

### 10. S3 Storage
![S3 Storage](screenshots/10-s3-storage.png)

### 11. Employee Face Capture
![Employee Face Capture](screenshots/11-employee-face-capture-screen.png)

### 12. Employee Face Captured Screen
![Employee Face Captured Screen](screenshots/12-employee-captured-image.png)

## Repository Structure

- `architecture/` — AWS architecture diagram.
- `screenshots/` — Application interface and AWS configuration screenshots.
- `docs/` — Project report and supporting documentation.

## Project Status

This repository is a documentation and implementation showcase. It does not currently provide a working public demo.

## Acknowledgement

Developed collaboratively with team members as part of the AWS Cloud Internship at F13 Technologies.
