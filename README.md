# 🚀 AWS EC2 Auto Scheduler (Cost Optimization Project)

This project automates the **start and stop scheduling of AWS EC2 instances** to reduce unnecessary cloud infrastructure costs during off-hours.

Many development and testing environments run 24/7 even when they are not actively used. This project solves that problem using **AWS Lambda and EventBridge scheduling**.

---

## 📌 Problem

Running EC2 instances continuously leads to **higher cloud costs**, especially for development environments that are only required during working hours.

---

## 💡 Solution

This project implements an automated scheduling system that:

• Starts EC2 instances at the beginning of working hours
• Stops EC2 instances after working hours
• Reduces unnecessary compute usage and cloud costs

---

## 🏗 Architecture

EventBridge triggers an AWS Lambda function at scheduled times.

The Lambda function then uses the **AWS SDK (Boto3)** to start or stop EC2 instances automatically.

Architecture Flow:

EventBridge → Lambda Function → EC2 Start/Stop API

---

## ⚙️ Technologies Used

* AWS EC2
* AWS Lambda
* Amazon EventBridge (CloudWatch Scheduler)
* IAM Roles & Policies
* Python (Boto3)

---

## 📷 Project Screenshots

### EC2 Instance

![image alt](https://github.com/okkyychetan/ec2-cost-optimization-automation/blob/df155b7ed5a525f8cb113e2e42d1c7ebe2b4aeb6/Screenshot%202026-03-05%20150552.png)


### EventBridge Scheduler

![image alt](https://github.com/okkyychetan/ec2-cost-optimization-automation/blob/df155b7ed5a525f8cb113e2e42d1c7ebe2b4aeb6/Screenshot%202026-03-05%20150655.png)

---

## 🔧 Setup Instructions

1. Create an EC2 instance in AWS.
2. Create a Lambda function using Python.
3. Attach IAM permissions to allow Lambda to manage EC2.
4. Write a Lambda function to start and stop instances using Boto3.
5. Create an EventBridge rule to schedule Lambda execution.
6. Test the automation.

---

## 📈 Key Learning Outcomes

• AWS automation
• Serverless architecture
• Cloud cost optimization
• Scheduling cloud resources
• IAM permissions management

---

## 🔗 Future Improvements

* Add support for multiple EC2 instances
* Add tag-based instance scheduling
* Add monitoring and logging

---

## 👨‍💻 Author

Chetan Bhiwagade
