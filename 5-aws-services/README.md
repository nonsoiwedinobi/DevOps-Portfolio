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

  <img width="1577" height="697" alt="image" src="https://github.com/user-attachments/assets/06a2e24d-59bf-496b-b7e6-81030a8b3eb4" />

  <img width="780" height="467" alt="image" src="https://github.com/user-attachments/assets/0b43ce1b-3147-41b7-aa73-e5bb2874a3fe" />

- Installed Docker on EC2

  <img width="1861" height="201" alt="image" src="https://github.com/user-attachments/assets/2528335a-3370-414a-9e3f-18eb29c026e4" />

- Pulled Docker image from private registry

  <img width="848" height="380" alt="image" src="https://github.com/user-attachments/assets/868a32c2-87b4-4135-9004-c96c914bfd67" />

- Opened port 3000 for our web app

  <img width="1557" height="602" alt="image" src="https://github.com/user-attachments/assets/5d3dcb49-f8a1-4de3-95b0-d0cabc3d84e3" />

- Deployed application manually on EC2

  <img width="1897" height="683" alt="image" src="https://github.com/user-attachments/assets/d7ed8032-c67b-4afa-a963-7c373ae78bd4" />

---

### 2️⃣ CI/CD – Deploy Application from Jenkins to EC2

- Created SSH credentials in Jenkins

  <img width="1575" height="115" alt="image" src="https://github.com/user-attachments/assets/be88afd0-5ed1-4b8e-b81b-26dce3ca5b5a" />

- Extended CI pipeline with deployment stage

  <img width="1422" height="853" alt="image" src="https://github.com/user-attachments/assets/b8905ccf-1c29-47f8-8cdf-c650e7ef4787" />

- SSH into EC2 from Jenkins

  <img width="1757" height="907" alt="image" src="https://github.com/user-attachments/assets/b766f2f4-986d-40b2-ab1e-4fce62c8ffd5" />

- Pulled and ran updated Docker image automatically

  <img width="845" height="97" alt="image" src="https://github.com/user-attachments/assets/54f5177d-0ff6-4f8f-aed5-878a18c1cf1e" />

  <img width="1917" height="707" alt="image" src="https://github.com/user-attachments/assets/3548f4d9-60c9-4ad7-89ea-1ff55abb2c3b" />

---

### 3️⃣ Deploy Application with Docker Compose on EC2

- Installed Docker Compose on EC2

  <img width="1463" height="281" alt="image" src="https://github.com/user-attachments/assets/ef6a0b10-8980-4735-8228-3366ee50704d" />

- Created `docker-compose.yml`

  <img width="1495" height="520" alt="image" src="https://github.com/user-attachments/assets/a3444951-bd44-4ed0-847e-b87cd552895e" />

  <img width="1895" height="205" alt="image" src="https://github.com/user-attachments/assets/616379d3-5837-4ce8-895c-1f312703a64e" />

- Extracted remote commands into reusable shell scripts

  <img width="1868" height="915" alt="image" src="https://github.com/user-attachments/assets/3dba6c98-b5e5-4824-ade6-105b4d6d97fb" />

  <img width="1887" height="791" alt="image" src="https://github.com/user-attachments/assets/60e0b8a7-11b7-4621-99c7-5b6b686f007c" />

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






