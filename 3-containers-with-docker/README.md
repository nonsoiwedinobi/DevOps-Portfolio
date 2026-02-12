# Containers with Docker

This section focuses on **containerization using Docker** and demonstrates how applications can be packaged, run, and managed consistently across different environments.

The projects in this folder build on the cloud and artifact repository foundations by introducing Docker as a core DevOps tool for application delivery and environment standardisation.

---

## 🎯 Purpose of This Section

The objective of these projects is to demonstrate:

- How Docker images are built using Dockerfiles
- Running applications in isolated containers
- Managing multi-container applications using Docker Compose
- Persisting application data using Docker volumes
- Pushing and pulling images from private container registries
- Running containerized workloads on cloud servers

---

## 🧱 Key Concepts Covered

- Container vs Virtual Machine
- Docker images and containers
- Dockerfile best practices
- Container networking
- Docker volumes and data persistence
- Private Docker registries
- Docker Compose orchestration

---

## 🛠 Technologies Used

- Docker
- Docker Compose
- Linux
- Node.js
- MongoDB
- Mongo Express
- Nexus Repository Manager
- DigitalOcean

---

## 📁 Projects Included

### 1️⃣ Docker for Local Development (Node.js + MongoDB)

- Created a Dockerfile for a Node.js application
- <img width="622" height="391" alt="image" src="https://github.com/user-attachments/assets/4f5bd392-de28-49c8-a6af-1fd0ddd5e50d" />

- Built Docker images locally
- <img width="1549" height="897" alt="image" src="https://github.com/user-attachments/assets/330f7fb7-8e0d-4961-b583-a48d67fc0ebb" />

- Ran application and database containers
- <img width="666" height="78" alt="image" src="https://github.com/user-attachments/assets/070d59cd-b61b-420e-9801-428b73ee7e8c" />

- <img width="1327" height="71" alt="image" src="https://github.com/user-attachments/assets/97f68f60-5abe-47b0-aaa7-f0d30ab6a841" />

- Connected Node.js application to MongoDB container
- Exposed application and database ports

📸 *Screenshot: Running Node.js and MongoDB containers locally*

---

### 2️⃣ Docker Compose – Multi-Container Application

- Wrote a `docker-compose.yml` file
- Orchestrated multiple services:
  - Node.js application
  - MongoDB database
  - Mongo Express UI
- Simplified multi-container startup and teardown

📸 *Screenshot: Docker Compose services running*

---

### 3️⃣ Persisting Data with Docker Volumes

- Created Docker volumes for MongoDB
- Attached volumes to containers
- Verified data persistence across container restarts

📸 *Screenshot: Docker volume configuration and data persistence*

---

### 4️⃣ Private Docker Registry with Nexus

- Created Docker hosted repository in Nexus
-  <img width="1317" height="871" alt="image" src="https://github.com/user-attachments/assets/1c30974e-eabd-4c00-8c27-edf9aab67ba0" />

-  <img width="1439" height="550" alt="image" src="https://github.com/user-attachments/assets/8946318a-433f-4f4b-8677-ed631e01ed64" />

- Configured Docker client authentication
-  <img width="1422" height="686" alt="image" src="https://github.com/user-attachments/assets/5661e2f7-4c25-43ac-a9d8-1d4bd694a3d7" />

- Opened port 8083 on Digital Ocean
- <img width="1469" height="80" alt="image" src="https://github.com/user-attachments/assets/063fbe6a-5d9a-4150-9a0d-2ed39564e0d3" />

- Authenticated with Nexus login
- <img width="634" height="150" alt="image" src="https://github.com/user-attachments/assets/884c6c80-f55b-4eb9-b4cc-89abbbe8fcdf" />

- Tagged and pushed images to Nexus Docker registry
- <img width="1167" height="273" alt="image" src="https://github.com/user-attachments/assets/82b8a0ee-d183-4f35-8caf-fd23951afb2c" />
- <img width="1664" height="590" alt="image" src="https://github.com/user-attachments/assets/956987bb-c057-471a-9763-3fa4db0bda14" />



📸 *Screenshot: Docker image stored in Nexus*

---

### 5️⃣ Deploy Nexus as a Docker Container

- Provisioned a cloud server
- Ran Nexus Repository Manager as a Docker container
- Exposed required ports
  <img width="1225" height="732" alt="image" src="https://github.com/user-attachments/assets/8ffa8880-2472-449c-801e-3de505986f66" />
- Pushed 
- Persisted Nexus data using Docker volumes

📸 *Screenshot: Nexus running as Docker container*

---

### 6️⃣ Deploy Docker Application on a Server with Docker Compose

- Copied Docker Compose configuration to a remote server
- Authenticated to a private Docker registry
- Pulled application images
- Started multi-container application using Docker Compose

📸 *Screenshot: Application running on remote server*

---

## 🔐 Security Considerations

- Used non-root containers where possible
- Managed credentials securely for private registries
- Restricted exposed ports
- Followed least-privilege principles for container access

---

## 🧠 Key DevOps Concepts Demonstrated

- Application packaging and portability
- Environment consistency across local and remote systems
- Artifact promotion using container images
- Preparation for CI/CD pipelines
- Foundation for Kubernetes orchestration

---

## 📚 Lessons Learned

- Differences between local and cloud container deployments
- Networking challenges in multi-container setups
- Importance of image tagging and versioning
- Best practices for managing container data

---

## 🔜 Future Improvements

- Integrate Docker builds into Jenkins CI pipelines
- Scan images for vulnerabilities
- Migrate Docker Compose workloads to Kubernetes
- Use multi-stage Docker builds for optimisation

---

## 👤 Author

**Nonso Iwedinobi**  
DevOps

