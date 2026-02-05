# Cloud & Infrastructure as a Service (IaaS) Foundations

This directory contains hands-on projects focused on **cloud infrastructure fundamentals** and **Infrastructure as a Service (IaaS)** concepts.

The projects here form the foundation of my DevOps skill set and demonstrate how cloud servers, networking, security, and core services are provisioned, configured, and managed before higher-level automation and orchestration are introduced.

---

## 🎯 Purpose of This Section

The goal of these projects is to demonstrate:

- How to provision and manage cloud servers
- Secure Linux server configuration following best practices
- Deploying applications on raw infrastructure
- Managing artifacts and repositories
- Interacting with cloud platforms programmatically

These projects intentionally start **without heavy automation**, to show a clear understanding of what tools like Terraform, Ansible, and Kubernetes later abstract away.

---

## 🧱 Projects Included

### 1️⃣ DigitalOcean Server Setup & Application Deployment
**Focus:** Core IaaS concepts and Linux server management

**What’s covered:**
- Provisioning a cloud server (Droplet)
- Creating and securing Linux users
- Applying basic server hardening practices
- Deploying and running a Java application on a remote server

**Key DevOps Concepts:**
- Infrastructure provisioning
- Linux user and permission management
- Secure server access (SSH)
- Manual deployment workflows

---

### 2️⃣ Nexus Artifact Repository on Cloud Server
**Focus:** Artifact management and dependency handling

**What’s covered:**
- Installing and configuring Nexus from scratch
- Managing users, roles, and permissions
- Publishing Java artifacts using:
  - Gradle
  - Maven
- Understanding artifact versioning and storage

**Key DevOps Concepts:**
- Artifact repositories
- Build outputs and dependencies
- Repository security and access control

---

### 3️⃣ AWS CLI & Cloud Resource Interaction
**Focus:** Programmatic interaction with cloud infrastructure

**What’s covered:**
- Installing and configuring AWS CLI
- Creating EC2 instances via CLI
- Managing:
  - IAM users, groups, and policies
  - Security groups
  - SSH key pairs
- Listing and inspecting AWS resources from the terminal

**Key DevOps Concepts:**
- Infrastructure via command-line tools
- IAM fundamentals
- Cloud resource lifecycle management

---

## 🛠 Technologies Used

- Cloud Platforms: AWS, DigitalOcean
- Operating System: Linux (Ubuntu)
- Build Tools: Maven, Gradle
- Artifact Management: Nexus
- Languages: Java
- Tooling: AWS CLI, SSH

---

## 📚 Why This Matters in a DevOps Context

Understanding cloud infrastructure at this level is critical because:

- CI/CD pipelines deploy **onto infrastructure**
- Containers still run **on servers**
- Kubernetes abstracts resources that still need to exist
- Automation tools are only effective if the underlying infrastructure is understood

These projects ensure a strong foundation before introducing:
- Containers
- Kubernetes
- Infrastructure as Code
- Configuration Management

---

## 🔜 Next Steps

Later sections in this repository build on this foundation by introducing:
- Docker and containerization
- CI/CD pipelines with Jenkins
- Kubernetes orchestration
- Terraform and Ansible automation

---

## 👤 Author

**Nonso Iwedinobi**  
DevOps / Platform Engineer (in progress)

