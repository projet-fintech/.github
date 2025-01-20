## ASMAS BANK

![image](https://github.com/user-attachments/assets/580617f8-cb11-46fd-8db0-d53fc8d64203)

## Overview
This repository contains a cloud-native FinTech application designed to deliver secure, efficient, and scalable financial services. The application is based on a microservices architecture and includes predictive models for loan approval and insurance management. It also provides separate frontend applications for admin and client dashboards.

---

## Architecture

### 1. **Microservices**

![image](https://github.com/user-attachments/assets/6a3013a2-9e44-41d4-b272-58d59c926e00)


The system is built using Spring Boot microservices, each serving a specific purpose:

- **User Microservice**: Manages user accounts, profiles, and authentication data.
- **Transaction Microservice**: Handles financial transactions, including deposits, withdrawals, and transfers.
- **Authentication Microservice**: Manages user authentication using OAuth2/JWT for secure access.
- **Account Microservice**: Manages user accounts, balances, and account details.
- **Notifications Microservice**: Sends email notifications for critical events, such as account creation or loan approvals.
- **Loan Management Microservice**: Handles loan applications, approvals, and repayment schedules.
- **Insurance Management Microservice**: Manages policies for car and health insurance.

Each microservice is deployed in a containerized environment using Docker and orchestrated via Kubernetes (AWS EKS).



### 2. **Predictive Models**
We have implemented three predictive models using Flask to serve machine learning APIs:

- **Loan Approval Model**: Predicts the likelihood of loan approval based on user-provided data.
- **Car Insurance Model**: Assesses the risk and calculates premiums for car insurance policies.
- **Health Insurance Model**: Evaluates health insurance applications and estimates premiums.

### 3. **Frontend Applications**
- **Admin Dashboard**: A web-based application for administrators to manage users, transactions, loans, and insurance policies.
- **Client Dashboard**: A user-friendly interface for clients to interact with the platform, view accounts, apply for loans, and manage insurance policies.

Both applications are built using React and are fully responsive.

---

## Deployment

### 1. **Containerization**
All components, including microservices and Flask models, are containerized using Docker for consistency and portability.

### 2. **Orchestration**
Kubernetes (AWS EKS) is used to manage and scale containers across multiple nodes. Each service has its own deployment and service configuration in Kubernetes.

### 3. **Cloud Infrastructure**
The application is hosted on AWS with the following resources:
- **Compute**: EC2 instances managed by EKS.
- **Database**: RDS (PostgreSQL) for relational data.
- **Storage**: S3 for storing documents and other static assets.
- **Monitoring**: AWS CloudWatch and Prometheus for real-time monitoring and alerting.

---

## Features

### **User Management**
- Registration and login.
- Profile management.


### **Financial Transactions**
- Real-time transaction processing.
- Support for deposits, withdrawals, and transfers.

### **Loan Management**
- Loan application and approval workflows.
- Email notifications for loan status updates.

### **Insurance Management**
- Policy application and approval for car and health insurance.
- Automated premium calculations.

### **Notifications**
- Email notifications for account creation and loan approvals.
- Configurable templates for different events.

### **Dashboards**
- Admin Dashboard: Analytics, user and loan management.
- Client Dashboard: Personalized user experience with account and loan details.

---

## Technology Stack

### **Backend**
- Spring Boot
- Flask (for predictive models)

### **Frontend**
- React

### **DevOps & Cloud**
- AWS (EKS, EC2, RDS, S3, CloudWatch)
- Kubernetes
- Docker
- Jenkins/GitLab CI for CI/CD pipelines

### **Data Science**
- scikit-learn for predictive modeling
- pandas, numpy for data processing

### **Monitoring**
- Prometheus and Grafana

---

## Getting Started

### **Prerequisites**
- Docker
- Kubernetes (kubectl)
- AWS CLI
- Java 21 (for Spring Boot services)

### **Setup Instructions**
1. Clone the repository.
2. Build Docker images for all services:
   ```bash
   docker-compose build
   ```
3. Deploy to Kubernetes:
   ```bash
   kubectl apply -f k8s-manifests/
   ```
4. Access the frontend applications via the respective URLs:
   - Admin Dashboard: `http://<admin-dashboard-url>`
   - Client Dashboard: `http://<client-dashboard-url>`

---

## Contact
For any inquiries or contributions, please reach out via [mouadrguibi900@gmail.com](mailto:mouadrguibi900@gmail.com).

---

## Contributors
- DevOps Engineer: [Mohamed Mouad Rguibi]
- Backend Engineer: [Ait Said Ayoub]
- Frontend Engineer: [Taous Samir]
- Data Scientist Engineer: [Salah El jably]
- Cloud Engineer: [Sabir Achraf]

---

## License
This project is licensed under the MIT License.

## ASMAS BANK



