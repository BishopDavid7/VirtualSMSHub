# VirtualSMSHub 📱📡

VirtualSMSHub is a cloud-based E-commerce SMS Gateway platform built entirely on **AWS Free Tier**. It allows businesses to rent virtual phone numbers, send and receive international SMS, and access REST APIs for automation.

---

## 🚀 Features

- 🌍 Rent virtual numbers (no physical SIMs)
- ✉️ Send international SMS (e.g., to UK)
- 📥 Receive confirmation replies via SMS
- 🔐 Secure login with Amazon Cognito
- 🧾 Billing per virtual number usage/day
- 🔧 REST API for programmatic SMS operations
- 📊 Admin dashboard with usage stats

---

## 🧱 Tech Stack

| Component             | Service Used                |
|----------------------|-----------------------------|
| Frontend Hosting     | AWS Amplify                 |
| Backend API          | AWS API Gateway + AWS Lambda|
| Authentication       | Amazon Cognito              |
| SMS Processing       | Amazon SNS / Twilio (via Lambda) |
| Database             | Amazon DynamoDB             |
| File Storage         | Amazon S3                   |
| Monitoring           | Amazon CloudWatch           |
| Containerization     | AWS Fargate (optional)      |

---

## 📁 Project Structure

```plaintext
VirtualSMSHub/
├── backend/
│   ├── lambda/
│   │   └── sendSMS.js
│   │   └── receiveSMS.js
│   └── api-gateway-definition.yml
├── frontend/
│   ├── src/
│   │   └── App.js
│   │   └── SMSDashboard.jsx
├── database/
│   └── dynamodb-schema.json
├── infrastructure/
│   └── amplify.yml
│   └── cognito-setup.md
├── README.md
└── architecture.md
