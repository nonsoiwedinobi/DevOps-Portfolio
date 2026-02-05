# Cloud & IaaS Foundations – DigitalOcean Server Setup & Application Deployment

This project demonstrates foundational **Infrastructure as a Service (IaaS)** concepts by provisioning a cloud server on DigitalOcean, securing it using Linux best practices, and deploying a Java Gradle application.

The goal is to show a clear understanding of **what happens before automation tools** (Terraform, Ansible, Kubernetes) are introduced.

---

## 🎯 Project Objectives

- Provision a cloud server from scratch
- Secure the server using Linux best practices
- Deploy and run a Java application on raw infrastructure
- Understand manual deployment workflows in a real cloud environment

---

## 🧱 Architecture Overview

- **Cloud Provider:** DigitalOcean
- **Compute:** Linux Droplet (Ubuntu)
- **Application:** Java application built with Gradle
- **Access:** SSH
- **Deployment Type:** Manual (no automation)

---

## 🛠 Technologies Used

- DigitalOcean
- Linux (Ubuntu)
- Java
- Gradle
- SSH

---

## 🚀 Implementation Steps

### 1️⃣ Set up and Configure a Server on DigitalOcean

- Created a new DigitalOcean Droplet
- Selected Ubuntu as the operating system
- Configured region and server size
- Generated and attached SSH keys for secure access

<img width="1876" height="902" alt="image" src="https://github.com/user-attachments/assets/746adb5f-a157-494f-a005-ddc2e223153f" />



---

### 2️⃣ Create and Configure a Secure Linux User (Best Practice)

- Logged into the server using the root account
- Created a new non-root user for application deployment
- Assigned sudo privileges to the new user

<img width="903" height="507" alt="image" src="https://github.com/user-attachments/assets/c0e20a15-ad1c-4026-a753-f3cef97ad9f7" />

<img width="791" height="30" alt="image" src="https://github.com/user-attachments/assets/ec5ae151-c6f4-4ef6-a6d1-3ad4d2a9df88" />



---

### 3️⃣ Deploy and Run a Java Gradle Application on the Droplet

- Installed required system dependencies (Java, Gradle)
- Transferred application files to the server
- Built the application using Gradle
- Executed the Java application on the server
- Verified application was running successfully

📸 *Screenshot: Gradle build output and running application*

---

## 🔐 Security Considerations

- Root SSH login disabled
- Least-privilege user model applied
- SSH key-based authentication used
- Separation of system administration and application execution

---

## 🧠 Key DevOps Concepts Demonstrated

- Infrastructure provisioning
- Linux user and permission management
- Secure remote access
- Manual deployment lifecycle
- Understanding infrastructure before automation

---

## 📚 Lessons Learned

- Why non-root users are essential for security
- The importance of understanding infrastructure fundamentals
- How automation tools abstract these manual steps
- Common pitfalls during manual application deployment

---

## 🔜 Future Improvements

- Automate server provisioning using Terraform
- Automate configuration using Ansible
- Containerize the application using Docker
- Integrate CI/CD pipeline for automated deployment

---

## 👤 Author

**Nonso Iwedinobi**  
DevOps / Platform Engineer (in progress)

