# Artifact Repository Manager – Nexus on DigitalOcean

This project demonstrates how to install, configure, and use **Nexus Repository Manager** on a cloud server to manage build artifacts.

It focuses on setting up Nexus from scratch on a DigitalOcean Droplet, securing access using users and permissions, and publishing Java artifacts using both **Gradle** and **Maven**.

---

## 🎯 Project Objectives

- Install and configure Nexus Repository Manager on a cloud server
- Understand artifact repositories and why they are critical in DevOps
- Create Nexus users with appropriate roles and permissions
- Publish Java build artifacts to Nexus using Gradle and Maven

---

## 🧱 Architecture Overview

- **Cloud Provider:** DigitalOcean
- **Compute:** Linux Droplet (Ubuntu)
- **Artifact Repository:** Nexus Repository Manager
- **Applications:** Java (Gradle & Maven)
- **Access:** Web UI + CLI

---

## 🛠 Technologies Used

- Nexus Repository Manager
- DigitalOcean
- Linux (Ubuntu)
- Java
- Gradle
- Maven

---

## 🚀 Implementation Steps

### 1️⃣ Provision and Prepare the Cloud Server

- Created a DigitalOcean Droplet running Ubuntu
- Configured secure SSH access
- Installed Java and required system dependencies

📸 *Screenshot: Droplet creation and server login*

---

### 2️⃣ Install and Configure Nexus Repository Manager

- Downloaded Nexus Repository Manager
- Installed Nexus as a service on the server
- Configured Nexus to run on a dedicated port
- Verified Nexus was accessible via browser

📸 *Screenshot: Nexus web interface running*

---

### 3️⃣ Create Nexus Users and Assign Permissions

- Created a new Nexus user
- Assigned repository-specific roles and permissions
- Applied the principle of least privilege
- Tested access using the new user account

📸 *Screenshot: Nexus user and role configuration*

---

### 4️⃣ Publish Java Artifacts Using Gradle

- Configured Gradle build to point to Nexus repository
- Built Java application artifact
- Authenticated with Nexus using user credentials
- Uploaded artifact to Nexus repository

📸 *Screenshot: Gradle build and artifact upload*

---

### 5️⃣ Publish Java Artifacts Using Maven

- Configured Maven `settings.xml` for Nexus authentication
- Updated `pom.xml` to use Nexus repository
- Built Java artifact with Maven
- Verified successful upload to Nexus

📸 *Screenshot: Maven build and artifact upload*

---

## 🔐 Security Considerations

- Nexus deployed on a secured server
- User-based authentication enabled
- Role-based access control applied
- Credentials stored securely in build tool configuration

---

## 🧠 Key DevOps Concepts Demonstrated

- Artifact management and versioning
- Dependency repositories
- Secure access control and permissions
- Build tool integration (Gradle & Maven)
- Preparing for CI/CD pipelines

---

## 📚 Lessons Learned

- Why artifact repositories are central to CI/CD workflows
- Differences between Gradle and Maven repository configuration
- Importance of permissions and role separation
- Common issues when publishing artifacts

---

## 🔜 Future Improvements

- Run Nexus as a Docker container
- Integrate Nexus with Jenkins pipelines
- Store Docker images in Nexus
- Automate Nexus provisioning with Ansible

---

## 👤 Author

**Nonso Iwedinobi**  
DevOps / Platform Engineer (in progress)

