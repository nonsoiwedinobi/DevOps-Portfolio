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
  <img width="1756" height="802" alt="image" src="https://github.com/user-attachments/assets/a0979f9b-881d-4f09-a43f-98256e82b6bb" />

- Installed Nexus as a service on the server
  <img width="988" height="47" alt="image" src="https://github.com/user-attachments/assets/a56293fc-2910-4d77-a800-298f701c7a4d" />

- Configured Nexus to run on a dedicated port
- Verified Nexus was accessible via browser

📸 *Screenshot: Nexus web interface running*

---

### 3️⃣ Create Nexus Users and Assign Permissions

- Created a new Nexus user
  <img width="906" height="510" alt="image" src="https://github.com/user-attachments/assets/6ff7e823-d436-4570-8b65-bb0edbfbb476" />

- Assigned repository-specific roles and permissions
  <img width="1021" height="207" alt="image" src="https://github.com/user-attachments/assets/b268e4ad-05f6-467e-b957-8a1ed802b55a" />

- Applied the principle of least privilege
  <img width="713" height="712" alt="image" src="https://github.com/user-attachments/assets/7d2429aa-e19f-432c-93e9-ba92e777b9a1" />

- Tested access using the new user account
  <img width="846" height="47" alt="image" src="https://github.com/user-attachments/assets/95265a18-d73d-4204-a1d6-baa7b35e3f7e" />
- Starting Nexus
  <img width="1027" height="91" alt="image" src="https://github.com/user-attachments/assets/27fb3a09-414f-472b-bb08-07afb0d8323b" />
- Check to conform nexus service running
  <img width="1452" height="447" alt="image" src="https://github.com/user-attachments/assets/e97760d4-7bbf-4fdb-a840-b2033db26484" />

  <img width="1885" height="905" alt="image" src="https://github.com/user-attachments/assets/fffb1de9-c5e1-44eb-a194-25b4fa7d4385" />

  <img width="1880" height="871" alt="image" src="https://github.com/user-attachments/assets/0f1f3d8b-2863-481e-af07-84a8f1e81ca7" />
  
  <img width="1280" height="812" alt="image" src="https://github.com/user-attachments/assets/a7420176-d53f-4af5-80b0-05586ab02aa9" />


---

### 4️⃣ Publish Java Artifacts Using Gradle

- Configured Gradle build to point to Nexus repository
  <img width="1067" height="905" alt="image" src="https://github.com/user-attachments/assets/5ac73389-3aa1-4d63-9fc3-35a1b0dfc5a5" />

- Built Java application artifact
  <img width="1417" height="322" alt="image" src="https://github.com/user-attachments/assets/f1c340cb-93be-45b7-a55f-3edbd9dba765" />


- Authenticated with Nexus using user credentials
  <img width="832" height="157" alt="image" src="https://github.com/user-attachments/assets/c71ddf0a-ee60-4f34-9995-8878238cee2d" />

- Uploaded artifact to Nexus repository
  <img width="1457" height="380" alt="image" src="https://github.com/user-attachments/assets/910260b9-43ce-4667-98ae-8a4407531c19" />

  <img width="1222" height="677" alt="image" src="https://github.com/user-attachments/assets/7eeeffcd-befb-4eb7-bd7f-fa0a52408f53" />


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
DevOps Engineer

