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

`apt install default-jre` to install java
<img width="991" height="97" alt="image" src="https://github.com/user-attachments/assets/71a4613c-9a5a-4211-b1de-8336274df612" />

I used th secure copy to copy a light weight application from my local device to the server using the command below

`scp build/libs/java-react-example.jar nonso@167.99.89.145:/root
<img width="867" height="43" alt="image" src="https://github.com/user-attachments/assets/6f493653-ba27-46c0-9139-a7076c85c24a" />

Ran application on the server
<img width="1476" height="702" alt="image" src="https://github.com/user-attachments/assets/bfd3bba0-3232-44b5-a275-8cc0a9aa3c38" />


Application is running on port 7071, so to access this application from the web, we would need to allow this port on the firewall

<img width="1491" height="108" alt="image" src="https://github.com/user-attachments/assets/649a95c8-fac8-4601-b17d-19ec8961c804" />

Application is now running on the web

<img width="827" height="967" alt="image" src="https://github.com/user-attachments/assets/3eb04758-f0a2-4cac-868e-a611c514351c" />


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
DevOps Engineer

