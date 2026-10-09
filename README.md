# Serverless Employee Face Recognition & Attendance Management System

## About the Project

This project was developed collaboratively with my teammates during my AWS Cloud Internship at **F13 Technologies**. The aim was to design and implement a serverless employee attendance management system using AWS services and face recognition.

The system allows administrators to register employees and view attendance records, while employees can capture their images through a web interface for identity verification. The project also includes automated attendance record storage, daily archival, and temporary image cleanup.

This repository showcases the project architecture, AWS service configurations, implementation screenshots, and application workflow documented during the internship.

## Key Features

- Employee registration with reference image upload
- Administrator authentication using Amazon Cognito
- Face comparison using Amazon Rekognition
- Automated attendance recording
- Attendance dashboard with employee status and records
- Daily attendance log archival
- Scheduled cleanup of temporary attendance images

## AWS Services Used

| AWS Service | Purpose |
|---|---|
| Amazon Cognito | Administrator authentication |
| Amazon API Gateway | Connects frontend applications to backend functions |
| AWS Lambda | Handles registration, image processing, attendance, and automation |
| Amazon Rekognition | Compares employee reference and captured images |
| Amazon DynamoDB | Stores employee details and attendance records |
| Amazon S3 | Stores images, archives attendance logs, and hosts frontend applications |
| Amazon EventBridge | Schedules archival and image cleanup tasks |
| Amazon CloudWatch | Monitors Lambda execution logs |
| AWS IAM | Manages permissions between AWS services |

## System Workflow

1. The administrator signs in and registers employees with their details and reference photographs.
2. Employee details are stored in DynamoDB, and reference images are stored in S3.
3. Employees capture and submit their images through the attendance interface.
4. An S3 event triggers a Lambda function, which uses Amazon Rekognition to compare the captured image with the reference image.
5. When a match is confirmed, the attendance record is saved in DynamoDB.
6. The administrator views attendance information through the dashboard.
7. EventBridge schedules Lambda functions to archive daily attendance records and remove temporary images.

## Project Screenshots

The repository includes screenshots documenting the following components:

- AWS serverless architecture
- API Gateway configuration
- Amazon Cognito authentication
- Lambda functions and triggers
- Amazon S3 buckets and stored objects
- DynamoDB employee and attendance tables
- EventBridge schedules
- CloudWatch logs
- Employee face-capture interface
- Attendance dashboard and employee registration

## Technologies

- Amazon Web Services (AWS)
- Python
- HTML, CSS, and JavaScript
- Serverless architecture
- Face recognition and image comparison
- Event-driven automation

## Learning Outcomes

Through this collaborative internship project, I gained exposure to AWS serverless architecture, cloud storage, database management, authentication, AI-based image comparison, event-driven workflows, and monitoring using AWS services.

## Project Status

This repository is a **documentation and implementation showcase** of the internship team project. It contains selected screenshots, architecture diagrams, and descriptions from the project report. A live public demo is not currently available.

## Acknowledgement

Developed as a collaborative team project during my AWS Cloud Internship at F13 Technologies, with guidance from the industry mentor and contributions from my teammates.
