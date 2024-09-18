# Inventory Management System

## Overview
This project is an **Inventory management system** designed to handle both patient appointments and doctor dashboards. It consists of a frontend, backend, and database, all deployed using **AWS services** for scalability, security, and ease of management.

### Architecture Overview
- **Frontend**: Built using **Next.js** and deployed with **AWS Amplify**, ensuring fast, scalable, and secure user interactions.
- **Backend**: Hosted on an **Amazon EC2 instance** within a public subnet. It handles API requests, manages business logic, and communicates with the database.
- **API Gateway**: Serves as the entry point for frontend API requests and routes them to the backend EC2 instance.
- **Database**: **Amazon RDS (Relational Database Service)** stores all the application data and is securely hosted within a private subnet to enhance security.
- **AWS S3 Bucket**: Hosts static objects and assets required by the frontend.

### AWS Architecture Diagram
![AWS Architecture](https://github.com/user-attachments/assets/1dd738a7-1f3c-415f-a533-01fd66800c85)

### Key Features
- **Scalable architecture** using AWS services to support growing user needs.
- **Frontend deployment** via AWS Amplify for a seamless CI/CD pipeline.
- **Backend** API hosted on EC2 instances, securely communicating with the database.
- **Private Database** hosted on Amazon RDS with access restricted to the backend EC2 instance only.

### Technologies Used
- **Frontend**: Next.js, AWS Amplify, AWS S3
- **Backend**: Node.js, Express.js, AWS EC2
- **Database**: Amazon RDS (MySQL/PostgreSQL)
- **Infrastructure**: AWS VPC, AWS API Gateway, AWS Security Groups

### Getting Started
1. **Clone the repository**:
    ```bash
    git clone https://github.com/Ammb305/inventory-management-nextjs.git
    ```
2. **Install dependencies**:
    ```bash
    cd frontend
    npm install
    cd ../backend
    npm install
    ```
3. **Run locally** (Development):
    ```bash
    npm run dev
    ```

### Deployment
The project is deployed on AWS using **Amplify**, **EC2**, and **RDS** services. Amplify automatically handles the frontend CI/CD pipeline, while the backend is deployed manually to EC2 and connected to an RDS instance in a private subnet.





