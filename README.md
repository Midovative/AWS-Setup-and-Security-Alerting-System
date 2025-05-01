# AWS-Setup-and-Security-Alerting-System
🔐 Automated AWS security alerting system using CloudTrail, EventBridge, and SNS to detect and notify on root user API activity. Built on AWS Free Tier for real-time monitoring and cloud security testing
This project demonstrates how to set up a real-time security alerting system in AWS to monitor critical root user activity. The system uses AWS CloudTrail to log API events, Amazon EventBridge to detect suspicious behavior, and Amazon SNS to send instant email notifications.

The main use case is tracking GetCallerIdentity API calls made by the root user, which can indicate unauthorized access attempts or credential misuse.

🔧 Technologies Used
AWS CloudTrail – Logs all AWS API activity.

Amazon SNS (Simple Notification Service) – Sends email alerts to subscribers.

Amazon EventBridge – Filters and routes events based on defined rules.

AWS CLI – Used for testing and simulating API calls.

Kali Linux – Environment for testing the setup.

📌 Key Features
Monitors root-level API calls in real time.

Sends immediate email alerts when suspicious activity is detected.

Fully serverless and uses only AWS Free Tier services.

Lightweight, scalable, and easily extendable to monitor additional actions or users.

✅ Setup Highlights
Configured CloudTrail with multi-region logging and S3 storage.

Created SNS topic and confirmed email subscription for alerting.

Defined EventBridge rule to detect GetCallerIdentity events from the root user.

Verified system using the AWS CLI in a Kali Linux environment.
