# AWS Services – Cloud Deployment & Automation

This section focuses on deploying and managing applications using Amazon Web Services (AWS).

The projects here demonstrate how cloud infrastructure, containerized applications, and CI/CD pipelines integrate with AWS services such as EC2, ECR, and the AWS CLI.

This section bridges the gap between local/container development and production cloud environments.

---

## 🎯 Purpose of This Section

The objective of these projects is to demonstrate:

- Provisioning and configuring EC2 instances
- Deploying Docker applications on AWS
- Using AWS CLI for infrastructure management
- Integrating Jenkins CI/CD pipelines with AWS
- Creating and using private Docker registries with Amazon ECR
- Automating deployments to cloud servers

---

## 🧱 Architecture Overview

- **Cloud Provider:** AWS
- **Compute:** EC2
- **Container Runtime:** Docker
- **CI/CD Tool:** Jenkins
- **Container Registry:** Amazon ECR
- **Access Method:** SSH & AWS CLI

---

## 🛠 Technologies Used

- AWS EC2
- AWS ECR
- AWS CLI
- Docker
- Jenkins
- Linux
- Java (Maven)
- Git

---

## 📁 Projects Included

### 1️⃣ Deploy Web Application on EC2 (Manual Deployment)

- Created and configured an EC2 instance
- Installed Docker on EC2
- Pulled Docker image from private registry
- Deployed application manually on EC2

📸 *Screenshot: Application running on EC2*

---

### 2️⃣ CI/CD – Deploy Application from Jenkins to EC2

- Created SSH credentials in Jenkins
- Extended CI pipeline with deployment stage
- SSH into EC2 from Jenkins
- Pulled and ran updated Docker image automatically

📸 *Screenshot: Jenkins deploying to EC2*

---

### 3️⃣ Deploy Application with Docker Compose on EC2

- Installed Docker Compose on EC2
- Created `docker-compose.yml`
- Deployed multi-container application remotely
- Extracted remote commands into reusable shell scripts

📸 *Screenshot: Docker Compose deployment on EC2*

---

### 4️⃣ Interacting with AWS CLI

- Installed and configured AWS CLI
- Created EC2 instances using CLI
- Created IAM users, groups, and policies
- Managed SSH key pairs
- Listed and inspected AWS resources

📸 *Screenshot: AWS CLI creating EC2 instance*

---

### 5️⃣ Create Private Docker Registry with Amazon ECR

- Created private Docker repository in ECR
- Authenticated Docker client with AWS
- Tagged and pushed Docker images to ECR
- Pulled images from ECR for deployment

📸 *Screenshot: Docker image in ECR repository*

---

## 🔐 Security Considerations

- Configured EC2 Security Groups
- Restricted inbound traffic to necessary ports only
- Managed IAM roles and policies with least privilege
- Stored AWS credentials securely in Jenkins
- Used SSH key authentication instead of passwords

---

## 🧠 Key DevOps Concepts Demonstrated

- Cloud infrastructure provisioning
- Manual vs automated deployment comparison
- Secure cloud access management
- Private container registries
- CI/CD cloud integration
- Infrastructure lifecycle management

---

## 📚 Lessons Learned

- Differences between local and cloud container execution
- Security implications of exposed ports
- Importance of IAM role configuration
- Challenges of remote deployment automation
- Why ECR improves enterprise container workflows

---

## 🔜 Future Improvements

- Deploy to EKS instead of EC2
- Use Terraform for EC2 provisioning
- Implement Blue/Green deployments
- Add monitoring and alerting
- Use Auto Scaling Groups

---

## 👤 Author

**Nonso Iwedinobi**  
DevOps Engineer
