## System Architecture

The system uses a serverless, event-driven architecture built with AWS services. Amazon Cognito handles administrator authentication, API Gateway connects the web application to backend services, and Lambda functions process employee registration and attendance requests. Amazon Rekognition performs face comparison, DynamoDB stores employee and attendance records, and S3 stores reference images and attendance archives.

![AWS System Architecture](architecture/aws-architecture.png)
