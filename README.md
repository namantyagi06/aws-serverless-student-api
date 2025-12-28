
<img width="1175" height="475" alt="serverless2 2025-12-28 125716" src="https://github.com/user-attachments/assets/958a073d-0e7f-4388-9086-77b7660ff428" />

AWS Serverless Student Data API*******

A simple AWS Serverless web application that allows users to insert and retrieve student data using AWS Lambda, API Gateway, and DynamoDB, with a lightweight frontend built using HTML, CSS, and JavaScript.

This project demonstrates how to build, deploy, and integrate serverless backend services on AWS.

🚀 Project Overview********

The application follows a serverless architecture:

A user interacts with a web UI

Requests are sent to API Gateway

API Gateway triggers AWS Lambda functions

Lambda reads/writes data to DynamoDB

The response is sent back to the client

This approach eliminates server management and scales automatically.

🏗️ Architecture Diagram (Logical Flow)*********
Client (Browser)
     |
     |  HTTP Request
     v
API Gateway
     |
     v
AWS Lambda (Python)
     |
     v
DynamoDB

🛠️ Tech Stack**********

AWS Lambda – Backend compute (Python)

Amazon DynamoDB – NoSQL database

Amazon API Gateway – REST API endpoints

HTML / CSS / JavaScript – Frontend

Git & GitHub – Version control

📂 Project Structure***********

aws-serverless-student-api/
│
├── insertStudentData.py   # Lambda function to insert student data
├── getStudents.py         # Lambda function to fetch student data
├── index.html             # Frontend UI
├── scripts.js             # Frontend JavaScript logic
└── README.md              # Project documentation

🔑 Features**********

Add student details (ID, name, class, age)

Fetch all student records

Fully serverless backend

Scalable and cost-efficient architecture

Clean separation of frontend and backend

⚙️ Prerequisites************

Before deploying, ensure you have:

AWS Account

AWS CLI installed and configured

Python 3.x

IAM role with permissions for:

Lambda

DynamoDB

API Gateway

🧪 DynamoDB Table Configuration***************

Create a DynamoDB table:

Table Name: studentData

Partition Key: studentid (String)

🧩 Lambda Functions**************

1️⃣ Insert Student Data (insertStudentData.py)

Triggered via API Gateway (POST)

Inserts student data into DynamoDB

2️⃣ Get Student Data (getStudents.py)

Triggered via API Gateway (GET)

Fetches all student records from DynamoDB

🌐 API Endpoints (Example)
Method	Endpoint	Description
POST	/addStudent	Insert student data
GET	/getStudents	Retrieve student records

▶️ How to Deploy (High Level)**********************

Create DynamoDB table

Create Lambda functions and upload Python code

Configure API Gateway endpoints

Connect API Gateway to Lambda

Update API URLs in scripts.js

Open index.html in browser

🧠 Learning Outcomes

Hands-on experience with AWS serverless services

Understanding event-driven architecture

Real-world integration of frontend and backend

REST API design using API Gateway

📌 Future Enhancements

Input validation and error handling

Authentication using AWS Cognito

CI/CD using GitHub Actions

CloudFormation / Terraform for IaC

Pagination for DynamoDB scans

👤 Author

Naman Tyagi
Aspiring AWS / DevOps / Backend Engineer

GitHub: https://github.com/namantyagi06
