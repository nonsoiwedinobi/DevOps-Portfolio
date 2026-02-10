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
- Built Docker images locally
- Ran application and database containers
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
- Configured Docker client authentication
- Built Docker images locally
- Tagged and pushed images to Nexus Docker registry

📸 *Screenshot: Docker image stored in Nexus*

---

### 5️⃣ Deploy Nexus as a Docker Container

- Provisioned a cloud server
- Ran Nexus Repository Manager as a Docker container
- Exposed required ports
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

