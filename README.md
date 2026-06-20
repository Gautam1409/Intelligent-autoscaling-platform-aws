# 🚀 Intelligent Auto Scaling & Resource Optimization Platform on AWS

## 📌 Project Overview

This project demonstrates the deployment of a highly available, scalable, and monitored web application on Amazon Web Services (AWS).

The platform automatically adjusts computing resources based on workload demand using AWS Auto Scaling Groups and CloudWatch monitoring. An Application Load Balancer distributes traffic across multiple EC2 instances, ensuring high availability and fault tolerance.

The project also integrates Docker containerization, SNS notifications, and resource optimization concepts to simulate an industry-grade cloud deployment environment.

---

## 🎯 Objectives

* Deploy a Dockerized web application on AWS EC2.
* Implement Application Load Balancing.
* Configure Auto Scaling based on CPU utilization.
* Enable High Availability using multiple Availability Zones.
* Monitor infrastructure using CloudWatch.
* Receive notifications using SNS.
* Demonstrate resource optimization through dynamic scaling.
* Simulate an industry-standard cloud architecture.

---

## 🏗️ Architecture

```text
                     Internet Users
                            │
                            ▼
                Application Load Balancer
                            │
                ┌───────────┴───────────┐
                │                       │
                ▼                       ▼
        Availability Zone A    Availability Zone B
                │                       │
                ▼                       ▼
          EC2 Instance            EC2 Instance
          (Docker App)           (Docker App)
                │                       │
                └───────────┬───────────┘
                            │
                            ▼
                   Auto Scaling Group
                            │
                            ▼
                      CloudWatch
                            │
                            ▼
                     SNS Notifications
                            │
                            ▼
                        Email Alerts
```

---

## 📐 Architecture Components

### 1. Amazon EC2

Hosts the Dockerized Flask web application.

### 2. Docker

Containerizes the application, ensuring consistent deployment across instances.

### 3. Application Load Balancer (ALB)

Distributes incoming traffic across healthy EC2 instances.

### 4. Auto Scaling Group (ASG)

Automatically launches or terminates EC2 instances based on workload demand.

### 5. Launch Template

Defines the EC2 configuration used by the Auto Scaling Group.

### 6. Amazon Machine Image (AMI)

Stores the preconfigured application environment.

### 7. CloudWatch

Monitors infrastructure metrics such as CPU utilization.

### 8. SNS (Simple Notification Service)

Sends email alerts when scaling events occur.

---

## ⚙️ Technology Stack

### Cloud Services

* Amazon EC2
* Application Load Balancer
* Auto Scaling Group
* Launch Templates
* Amazon Machine Image (AMI)
* CloudWatch
* SNS

### Application

* Python
* Flask
* Docker

### DevOps Tools

* Git
* GitHub

---

## 🔄 Auto Scaling Workflow

```text
User Traffic Increases
          │
          ▼
CPU Utilization > 70%
          │
          ▼
CloudWatch Detects High Load
          │
          ▼
Auto Scaling Group Triggers
          │
          ▼
New EC2 Instance Created
          │
          ▼
Load Balancer Starts Routing Traffic
```

---

## 📊 Features Implemented

✅ Dockerized Flask Application

✅ EC2 Deployment

✅ Custom AMI Creation

✅ Launch Template Configuration

✅ Auto Scaling Group

✅ Application Load Balancer

✅ Multi-AZ Deployment

✅ CloudWatch Monitoring

✅ CPU-Based Dynamic Scaling

✅ SNS Email Notifications

✅ High Availability Architecture

---

## 🧪 Testing Performed

### Load Testing

CPU stress was generated using:

```bash
stress --cpu 2 --timeout 600
```

### Result

* CPU utilization increased.
* CloudWatch detected threshold breach.
* Auto Scaling Group launched additional EC2 instances.
* Load Balancer distributed traffic successfully.
* SNS notifications were triggered.

---

## 📈 Future Enhancements

* Resource Optimization Dashboard
* Real-Time CloudWatch Metrics Integration using Boto3
* Amazon S3 Storage for Scaling Reports
* Cost Optimization Recommendations
* CI/CD Pipeline using GitHub Actions
* Infrastructure as Code using Terraform

---

## 🎓 Learning Outcomes

Through this project, the following cloud concepts were implemented and understood:

* Infrastructure Scalability
* High Availability
* Load Balancing
* Cloud Monitoring
* Event-Driven Notifications
* Docker Containerization
* AWS Networking
* Resource Optimization

---

## 👨‍💻 Author

**Gautam Kesharwani**
and 
**Khush Jain**
B.Tech Information Technology

Vidyalankar Institute of Technology

---

## 📄 License

This project is developed for educational and academic purposes.
