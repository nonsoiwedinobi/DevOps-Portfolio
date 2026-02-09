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

<img width="1427" height="808" alt="image" src="https://github.com/user-attachments/assets/57182400-e2b6-47ee-84a7-53dd0ae230a6" />

<img width="1346" height="531" alt="image" src="https://github.com/user-attachments/assets/8ce6ca97-d462-4bee-b49a-056f186108ee" />44

<img width="1511" height="735" alt="image" src="https://github.com/user-attachments/assets/f0c5caa7-a4cb-43bd-8d9c-83f4d8acf24e" />

<img width="1148" height="747" alt="image" src="https://github.com/user-attachments/assets/b88ba2e2-fd46-4513-bcae-ee4daa9ff6c8" />

<img width="1467" height="602" alt="image" src="https://github.com/user-attachments/assets/db1e15ae-9fce-498f-8b7f-d472cd440472" />

<img width="1466" height="537" alt="image" src="https://github.com/user-attachments/assets/fa019832-c756-416c-8d89-2082cca49ebd" />

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
  <img width="913" height="513" alt="image" src="https://github.com/user-attachments/assets/49136278-7bef-47f5-ad6f-eaa256713ead" />

- Assigned repository-specific roles and permissions
  <img width="1036" height="360" alt="image" src="https://github.com/user-attachments/assets/11f7cca2-274a-4986-9dcb-7b552e3bb61e" />

- Applied the principle of least privilege
  <img width="713" height="712" alt="image" src="https://github.com/user-attachments/assets/7d2429aa-e19f-432c-93e9-ba92e777b9a1" />

  <img width="912" height="26" alt="image" src="https://github.com/user-attachments/assets/4763035d-af71-4cc6-9572-98911131a8e0" />

  <img width="557" height="297" alt="image" src="https://github.com/user-attachments/assets/821545cb-458b-4d36-b31c-74da91998776" />

- Starting Nexus
  <img width="1027" height="91" alt="image" src="https://github.com/user-attachments/assets/27fb3a09-414f-472b-bb08-07afb0d8323b" />
- Check to conform nexus service running
  <img width="1452" height="447" alt="image" src="https://github.com/user-attachments/assets/e97760d4-7bbf-4fdb-a840-b2033db26484" />

  <img width="1905" height="958" alt="image" src="https://github.com/user-attachments/assets/832a4a7d-f96b-4835-8c0d-6c8c230d870a" />



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
  <img width="1114" height="952" alt="image" src="https://github.com/user-attachments/assets/a93331eb-141c-4c48-96e2-c68d0a2ff7dc" />

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

