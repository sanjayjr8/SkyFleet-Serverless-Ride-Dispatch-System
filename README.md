# 🚖 SkyFleet – Serverless Ride Dispatch System

A fully serverless ride-booking platform built using AWS services like Lambda, Cognito, API Gateway, and DynamoDB. Developed as part of a hands-on AWS cloud engineering course (SVS203-R1), this project explores building scalable backend systems with modern DevOps practices.

---

## 🧠 What I Built

This project simulates a unicorn ride-sharing platform with:

- 🌐 A hosted frontend deployed using **AWS Amplify**
- 👤 User authentication via **Amazon Cognito**
- ⚙️ Serverless backend logic with **AWS Lambda (Node.js)**
- 🛣 Secure API layer using **Amazon API Gateway**
- 💾 Persistent ride history stored in **Amazon DynamoDB**

---

## 🛠 Tech Stack

| Layer        | Tool / Service               |
|--------------|------------------------------|
| Frontend     | HTML, JavaScript, Amplify    |
| Authentication | Amazon Cognito             |
| API Layer    | Amazon API Gateway           |
| Logic        | AWS Lambda (Node.js 20.x)    |
| Database     | Amazon DynamoDB              |
| CI/CD        | GitHub → AWS Amplify         |

---

## 📸 Architecture Overview

```txt
Client (User)
   │
   ▼
AWS Amplify (Static Site Hosting)
   │
   ▼
Amazon Cognito (Authentication)
   │
   ▼
API Gateway ──► Lambda (Ride Handler)
                        │
                        ▼
                 DynamoDB (Ride Logs)



---

## 🚧 Challenges Faced

- JWT token decoding and integrating **API Gateway authorizers**
- Configuring **IAM roles and policies** to enable Lambda-DynamoDB access securely
- Understanding **event.requestContext** for authenticated request handling
- Navigating **Cognito user pool config and token scopes**

---

## 🚀 Key Learnings

- Gained hands-on experience with **event-driven serverless apps**
- Learned how to **secure APIs with Cognito & JWT**
- Understood AWS **service-to-service communication** (IAM, API Gateway, Lambda, DynamoDB)
- Learned to debug Lambda using CloudWatch logs and test events

