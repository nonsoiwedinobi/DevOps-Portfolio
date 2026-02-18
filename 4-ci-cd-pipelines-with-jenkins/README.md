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

  <img width="1301" height="782" alt="image" src="https://github.com/user-attachments/assets/189deb2f-eda0-4bff-8796-31dfdc558ec0" />

  <img width="1453" height="712" alt="image" src="https://github.com/user-attachments/assets/ba93bdce-2ddd-4958-affd-487f50897a43" />

- Built Docker images from application code

  <img width="1046" height="290" alt="image" src="https://github.com/user-attachments/assets/cce8d007-2b18-44c3-9e56-b5ea0f51f491" />

- Pushed images to private container registries

  <img width="1241" height="707" alt="image" src="https://github.com/user-attachments/assets/7b75c01e-e794-4c31-9e4e-d0eadb6e817f" />

  <img width="1341" height="706" alt="image" src="https://github.com/user-attachments/assets/01603420-930b-4c74-bfb6-5b0561f8f187" />

- Pushed complete pipeline to docker

  <img width="1250" height="975" alt="image" src="https://github.com/user-attachments/assets/d3d37c2b-2608-4c5c-acf1-e696c1a56bc7" />

---

### 3️⃣ Jenkins Shared Library

- Created a separate Git repository for shared pipeline logic

  <img width="1322" height="781" alt="image" src="https://github.com/user-attachments/assets/5397a676-2176-4fb4-99fe-cac8c9028731" />

- Implemented reusable Groovy functions

  <img width="1883" height="796" alt="image" src="https://github.com/user-attachments/assets/5839e430-f928-41d2-a095-55851cbb03f4" />

- Integrated shared library globally and per-project

  <img width="1725" height="856" alt="image" src="https://github.com/user-attachments/assets/6c44092b-e8e1-459e-96a7-84a44c9c4b28" />

  <img width="918" height="831" alt="image" src="https://github.com/user-attachments/assets/8c928fd1-ecd8-4f31-83e2-66bc54d2e8b3" />


---

### 4️⃣ Webhook Integration for Automatic Builds

- Configured GitHub webhooks

  <img width="1696" height="737" alt="image" src="https://github.com/user-attachments/assets/cc0f0551-6e84-4047-a759-8f318c2b90f8" />

- Installed GitLab plugin in Jenkins

  <img width="1902" height="758" alt="image" src="https://github.com/user-attachments/assets/d30f1cab-37a9-4fe3-b1d4-77234a722a39" />

- Verified webhook-triggered builds

  <img width="1215" height="757" alt="image" src="https://github.com/user-attachments/assets/2b76e4bd-6d99-45f5-b705-aa127e17dd99" />

---

### 5️⃣ Dynamic Application Versioning in CI/CD

- Automatically incremented application version during CI

  <img width="1905" height="902" alt="image" src="https://github.com/user-attachments/assets/d7895845-4e30-4d1a-a4b1-8f7c5254ec43" />

- Built Docker images with dynamic tags

  <img width="1527" height="522" alt="image" src="https://github.com/user-attachments/assets/e41f4fcc-54d9-4d97-90ee-d1e103854b05" />

- Committed version updates back to Git

  <img width="1567" height="562" alt="image" src="https://github.com/user-attachments/assets/67856f99-0619-45ee-9384-727dc3b31649" />

- Prevented infinite build loops from CI commits

  <img width="1523" height="160" alt="image" src="https://github.com/user-attachments/assets/a3713e3c-abf3-4c8b-b7c5-5d66a71c7bec" />

  <img width="1895" height="927" alt="image" src="https://github.com/user-attachments/assets/f979b03f-c8b5-47e6-a5f0-534a2cb3b289" />


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

