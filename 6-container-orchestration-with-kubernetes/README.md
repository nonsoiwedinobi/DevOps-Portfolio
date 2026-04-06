# Container Orchestration with Kubernetes

This section focuses on deploying and managing containerized applications using **Kubernetes**, the industry standard container orchestration platform.

The projects in this section demonstrate how Kubernetes automates container deployment, scaling, networking, and configuration management in production environments.

These implementations build on previous sections involving Docker, CI/CD pipelines, and cloud infrastructure.

---

## 🎯 Purpose of This Section

The objective of these projects is to demonstrate:

- Deploying containerized applications in Kubernetes clusters
- Managing application configuration using ConfigMaps and Secrets
- Deploying stateful services in Kubernetes
- Using Helm for Kubernetes package management
- Managing microservices deployments
- Deploying applications from private container registries

---

## 🧱 Architecture Overview

- **Container Runtime:** Docker
- **Container Orchestration:** Kubernetes
- **Cluster Platforms:** Minikube / Managed Kubernetes
- **Package Management:** Helm
- **Container Registry:** AWS ECR / Docker Hub
- **Applications:** MongoDB, Mongo Express, Microservices applications

---

## 🛠 Technologies Used

- Kubernetes
- Docker
- Helm
- Minikube
- AWS ECR
- Linux
- Microservices architecture

---

## 📁 Projects Included

### 1️⃣ Deploy MongoDB and Mongo Express in a Local Kubernetes Cluster

- Set up a local Kubernetes cluster using **Minikube**

  <img width="1461" height="652" alt="image" src="https://github.com/user-attachments/assets/f7d9e686-ba1b-4e3c-8471-5d2df13e4868" />

  <img width="486" height="176" alt="image" src="https://github.com/user-attachments/assets/30d55ecc-ab30-4607-b4db-a32679e3f0b5" />

- Created Kubernetes manifests for:
  - Deployments
    <img width="885" height="222" alt="image" src="https://github.com/user-attachments/assets/25f417c7-df8b-4f70-aaaa-5deb8a43021e" />

- Configured MongoDB credentials using **Secrets**

  <img width="597" height="340" alt="image" src="https://github.com/user-attachments/assets/a406c495-5dba-477f-849c-e05939e3c626" />

  <img width="1021" height="192" alt="image" src="https://github.com/user-attachments/assets/72115835-2167-4378-a23b-8a2f32afd546" />

- Managed application configuration using **ConfigMaps**

  <img width="1078" height="251" alt="image" src="https://github.com/user-attachments/assets/bb456355-ce90-4b02-ad0a-8371d19ce7ea" />

  <img width="1757" height="646" alt="image" src="https://github.com/user-attachments/assets/11548353-934e-4533-ad98-66a76687c96d" />

  <p align="center">
  <img src="screenshots/Screenshot 2026-01-16 220114.png" width="800">
</p>

<p align="center">
  <img src="screenshots/dashboard.png" width="800">
</p>
  
---

### 2️⃣ Deploy Stateful Services Using Helm

- Created a managed Kubernetes cluster

  <p align="center">
  <img src="screenshots/k8s-cluster.png" width="800">
</p>
- Installed MongoDB using a **Helm chart**

<p align="center">
  <img src="screenshots/Installed-mongodb-helm-chart.png" width="800">
</p>
- Configured persistent storage

<p align="center">
  <img src="screenshots/persisted-volume.png" width="800">
</p>
- Configured **NGINX ingress** for external access

<p align="center">
  <img src="screenshots/NGINX-ingress.png" width="800">
</p>

- Deployed Mongo Express as a client UI

  <p align="center">
  <img src="screenshots/mongo-express-ui.png" width="800">
</p>
---

### 3️⃣ Deploy Mosquitto Message Broker Using ConfigMaps and Secrets

- Created Kubernetes configuration for Mosquitto

  <p align="center">
  <img src="screenshots/mosquitto.png" width="800">
</p>

<p align="center">
  <img src="screenshots/mosquitto2.png" width="800">
</p>
---

### 4️⃣ Deploy Application from Private Docker Registry

- Created Kubernetes **image pull secrets**

  <p align="center">
  <img src="screenshots/created-secrets.png" width="800">
  </p>
- Configured Kubernetes deployment to pull images from private registry

  <p align="center">
  <img src="screenshots/pull-image-from-private.png" width="800">
  </p>
- Deployed application to cluster
---

### 5️⃣ Deploy Microservices Application to Kubernetes

- Created Kubernetes manifests for microservices architecture

  <p align="center">
  <img src="screenshots/manifest-file.png" width="800">
  </p>
- Deployed application components into cluster

  <p align="center">
  <img src="screenshots/deployed-application.png" width="800">
  </p>
- Verified service communication between containers

  <p align="center">
  <img src="screenshots/online-boutique.png" width="800">
  </p>
---

### 6️⃣ Create Reusable Helm Charts

- Created reusable Helm chart templates
- Defined Deployment and Service templates
- Parameterized application configuration
- Reused charts across multiple services

📸 *Screenshot: Helm chart deployment*

---

### 7️⃣ Deploy Applications Using Helmfile

- Managed multiple Helm deployments using **Helmfile**
- Simplified management of microservices deployments
- Centralized environment configuration

📸 *Screenshot: Helmfile deployment*

---

## 🔐 Security Considerations

- Stored sensitive credentials using Kubernetes Secrets
- Restricted access to private container registries
- Configured proper role-based access control (RBAC)
- Followed least-privilege access principles

---

## 🧠 Key DevOps Concepts Demonstrated

- Container orchestration
- Infrastructure abstraction
- Declarative infrastructure management
- Stateful vs stateless workloads
- Kubernetes configuration management
- Microservices deployment patterns
- Kubernetes package management with Helm

---

## 📚 Lessons Learned

- Managing complex applications using Kubernetes
- Importance of configuration management
- Benefits of declarative infrastructure
- Helm's role in simplifying Kubernetes deployments
- Challenges of networking and service discovery

---

## 🔜 Future Improvements

- Implement Horizontal Pod Autoscaling
- Add Kubernetes health checks and probes
- Integrate Kubernetes deployments into CI/CD pipelines
- Implement GitOps workflows
- Introduce service mesh technologies

---

## 👤 Author

**Nonso Iwedinobi**  
DevOps Engineer
