# CI/CD Pipelines with Jenkins

This section focuses on building **Continuous Integration and Continuous Delivery (CI/CD) pipelines** using Jenkins.

The projects here demonstrate how application builds, container images, and deployments can be automated using Jenkins pipelines, Jenkinsfiles, shared libraries, and webhook integrations.

These pipelines build on previous sections by integrating:
- Docker images
- Artifact repositories
- Cloud servers
- Kubernetes clusters

---

## 🎯 Purpose of This Section

The objective of these projects is to demonstrate:

- Installing and operating Jenkins in a cloud environment
- Creating different Jenkins job types
- Writing Jenkinsfiles for CI pipelines
- Automating build, test, and image creation steps
- Using shared libraries to reuse pipeline logic
- Triggering pipelines automatically using webhooks
- Implementing versioning strategies in CI/CD

---

## 🧱 Architecture Overview

- **CI/CD Tool:** Jenkins
- **Runtime:** Docker
- **Source Control:** Git / GitLab
- **Build Tools:** Maven, Gradle
- **Container Registry:** Docker Hub / Nexus
- **Deployment Targets:** Linux servers, Kubernetes clusters

---

## 🛠 Technologies Used

- Jenkins
- Docker
- Git / GitLab
- Java
- Maven
- Gradle
- Linux
- Docker Hub
- Nexus Repository Manager

---

## 📁 Projects Included

### 1️⃣ Install and Configure Jenkins

- Provisioned a cloud server
  
  <img width="1575" height="788" alt="image" src="https://github.com/user-attachments/assets/63657796-3922-4a6b-9816-6035302d8fc7" />

- Created a firewall for Jenkins
  
  <img width="1520" height="714" alt="image" src="https://github.com/user-attachments/assets/8d223ada-279e-42e7-a967-56cea130d09d" />

- Installed Docker on the Jenkins server
  
  <img width="1427" height="751" alt="image" src="https://github.com/user-attachments/assets/d89e13e6-9d47-469d-a634-864c6e4b7216" />

- Installed Jenkins as a Docker container

  <img width="1480" height="579" alt="image" src="https://github.com/user-attachments/assets/f80bef3c-13ac-42ec-9140-e6961a31d88a" />

- Installed required plugins

  <img width="1479" height="847" alt="image" src="https://github.com/user-attachments/assets/b8e2e3bb-d64e-458c-9579-9c9754e4f7ad" />

---

### 2️⃣ Create CI Pipelines with Jenkinsfile

- Created Freestyle, Pipeline, and Multibranch Pipeline jobs
- Connected Jenkins to Git repositories
- Installed build tools inside Jenkins

  <img width="1888" height="941" alt="image" src="https://github.com/user-attachments/assets/88143b65-400f-465a-9c6c-d5d9776ec5af" />

  <img width="816" height="303" alt="image" src="https://github.com/user-attachments/assets/9c752fd8-2dc4-44a8-98d8-e6e62993f3fb" />

  <img width="865" height="365" alt="image" src="https://github.com/user-attachments/assets/1ccfd95e-db47-419d-bdf4-0c1d7a2d3c45" />

- Installed stage view pipeline

  <img width="1836" height="709" alt="image" src="https://github.com/user-attachments/assets/c517ce9d-db83-4295-81f7-e553721a8459" />

- Freestyle job demo build

  <img width="1873" height="904" alt="image" src="https://github.com/user-attachments/assets/22410adc-13d4-478e-a480-4fc1f67a8e64" />

- Built Java artifacts using Maven
- Built Docker images from application code
- Pushed images to private container registries

📸 *Screenshot: Jenkins pipeline execution*

---

### 3️⃣ Jenkins Shared Library

- Created a separate Git repository for shared pipeline logic
- Implemented reusable Groovy functions
- Integrated shared library globally and per-project
- Reduced duplication across Jenkinsfiles

📸 *Screenshot: Jenkins shared library usage*

---

### 4️⃣ Webhook Integration for Automatic Builds

- Configured GitLab webhooks
- Installed GitLab plugin in Jenkins
- Triggered CI pipelines automatically on code changes
- Verified webhook-triggered builds

📸 *Screenshot: Webhook-triggered pipeline*

---

### 5️⃣ Dynamic Application Versioning in CI/CD

- Automatically incremented application version during CI
- Built Docker images with dynamic tags
- Pushed versioned images to private registries
- Committed version updates back to Git
- Prevented infinite build loops from CI commits

📸 *Screenshot: Versioned Docker image build*

---

### 6️⃣ Continuous Deployment Targets

- Extended CI pipelines with deployment stages
- Deployed applications to:
  - Linux servers (Docker)
  - EC2 instances
  - Kubernetes clusters
- Used SSH-based deployments and container orchestration

📸 *Screenshot: Successful deployment from Jenkins*

---

## 🔐 Security Considerations

- Credential management using Jenkins credentials store
- SSH keys managed securely
- Registry credentials not hard-coded
- Controlled access to Jenkins jobs and pipelines

---

## 🧠 Key DevOps Concepts Demonstrated

- CI vs CD responsibilities
- Pipeline-as-Code (Jenkinsfile)
- Build reproducibility
- Artifact promotion
- Automated versioning
- Deployment automation
- Reusable pipeline design

---

## 📚 Lessons Learned

- Why Jenkinsfile is preferred over UI-only jobs
- Benefits of shared libraries in large pipelines
- Common CI/CD pitfalls and how to avoid them
- Importance of idempotent deployments
- How CI/CD enables faster and safer releases

---

## 🔜 Future Improvements

- Add automated testing stages
- Introduce pipeline approval gates
- Integrate security scanning (SAST / image scanning)
- Migrate pipelines to cloud-native CI tools for comparison

---

## 👤 Author

**Nonso Iwedinobi**  
DevOps Engineer

