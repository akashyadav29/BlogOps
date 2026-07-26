# 🚀 BlogOps - End-to-End DevSecOps CI/CD Pipeline on Amazon EKS

![Jenkins](https://img.shields.io/badge/Jenkins-CI-red?logo=jenkins)
![Docker](https://img.shields.io/badge/Docker-2496ED?logo=docker&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?logo=kubernetes&logoColor=white)
![ArgoCD](https://img.shields.io/badge/ArgoCD-EF7B4D?logo=argo&logoColor=white)
![AWS](https://img.shields.io/badge/AWS-EKS-FF9900?logo=amazon-aws&logoColor=white)
![SonarQube](https://img.shields.io/badge/SonarQube-Code%20Quality-4E9BCD?logo=sonarqube)
![Trivy](https://img.shields.io/badge/Trivy-Security-blue)
![Prometheus](https://img.shields.io/badge/Prometheus-Monitoring-E6522C?logo=prometheus)
![Grafana](https://img.shields.io/badge/Grafana-Dashboard-F46800?logo=grafana)

---

# 📌 Overview

**BlogOps** is a production-style **three-tier MERN blogging application** deployed on **Amazon EKS** using a complete **DevSecOps CI/CD pipeline**.

The project automates application build, security scanning, code quality analysis, Docker image creation, GitOps deployment, Kubernetes orchestration, and monitoring.

---

# 🏗 Architecture

```
Developer
     │
     ▼
 GitHub Repository
     │
     ▼
 Jenkins CI Pipeline
 ├── Source Code Checkout
 ├── Trivy Filesystem Scan
 ├── OWASP Dependency Check
 ├── SonarQube Code Analysis
 ├── Quality Gate
 ├── Build Docker Images
 ├── Push Images to Docker Hub
 └── Trigger CD Pipeline
     │
     ▼
 Jenkins CD Pipeline
 ├── Update Kubernetes YAML
 ├── Commit Changes
 └── Push to GitHub
     │
     ▼
 GitHub (GitOps)
     │
     ▼
 ArgoCD
     │
     ▼
 Amazon EKS Cluster
 ├── React Frontend
 ├── Node.js Backend
 ├── MongoDB
 └── Redis
     │
     ▼
 Prometheus
     │
     ▼
 Grafana
```

---

# 🚀 Tech Stack

### Cloud
- AWS EC2
- Amazon EKS
- IAM

### CI/CD
- Jenkins
- GitHub
- Docker Hub

### Containerization
- Docker
- Kubernetes

### GitOps
- ArgoCD

### DevSecOps
- SonarQube
- Trivy
- OWASP Dependency Check

### Monitoring
- Prometheus
- Grafana

### Backend
- Node.js
- Express.js
- MongoDB
- Redis

### Frontend
- React
- TypeScript
- Tailwind CSS
- Vite

---

# 📂 Project Structure

```
BlogOps
│
├── frontend/
├── backend/
├── database/
├── kubernetes/
├── Automations/
├── GitOps/
├── Jenkinsfile
├── docker-compose.yml
└── README.md
```

---

# ⚙ CI Pipeline

The Jenkins CI pipeline performs:

- Checkout Source Code
- Trivy Filesystem Scan
- OWASP Dependency Check
- SonarQube Code Analysis
- SonarQube Quality Gate
- Generate Environment Variables
- Build Docker Images
- Push Images to Docker Hub
- Trigger CD Pipeline

---

# 🚀 CD Pipeline

The CD pipeline automatically:

- Checks out Kubernetes manifests
- Updates Docker image tags
- Commits updated manifests
- Pushes changes to GitHub
- ArgoCD detects changes
- Automatically deploys the latest application to Amazon EKS

---

# 🔐 DevSecOps

The pipeline integrates multiple security tools.

### SonarQube

- Code Quality
- Bugs Detection
- Vulnerability Analysis
- Code Smells
- Quality Gates

### Trivy

- Filesystem Vulnerability Scan
- Docker Image Security Scan

### OWASP Dependency Check

- Dependency Vulnerability Analysis
- CVE Detection
- XML Report Generation

---

# ☸ Kubernetes Components

The application is deployed using Kubernetes resources including:

- Deployments
- Services
- Persistent Volume
- Persistent Volume Claim

---

# 📊 Monitoring

Monitoring is implemented using:

- Prometheus
- Grafana

Used for:

- Cluster Monitoring
- Node Monitoring
- Pod Monitoring
- Resource Utilization

---

# 🐳 Docker Images

Backend

```
akashyadav29/blogops-backend-beta
```

Frontend

```
akashyadav29/blogops-frontend-beta
```

---

# 🔄 CI/CD Workflow

```
Developer
     │
     ▼
GitHub
     │
     ▼
Jenkins CI
     │
     ▼
Security Scan
     │
     ▼
Code Quality
     │
     ▼
Docker Build
     │
     ▼
Docker Hub
     │
     ▼
Jenkins CD
     │
     ▼
GitHub (Manifest Update)
     │
     ▼
ArgoCD
     │
     ▼
Amazon EKS
     │
     ▼
Prometheus & Grafana
```

---

# ✨ Features

- Automated CI/CD Pipeline
- GitOps Deployment
- Dockerized MERN Application
- Kubernetes Deployment
- Automated Image Versioning
- SonarQube Code Quality
- Trivy Vulnerability Scanning
- OWASP Dependency Analysis
- Monitoring with Prometheus & Grafana
- Email Notifications from Jenkins

---

# 📸 Screenshots


<img width="960" height="507" alt="Screenshot 2026-07-18 052731" src="https://github.com/user-attachments/assets/f7336fa0-972a-4296-9fed-0646ad17774b" />

---

<img width="960" height="505" alt="Screenshot 2026-07-18 052656" src="https://github.com/user-attachments/assets/9ad1d371-a2b5-4d07-a7e8-1eabe79e8b40" />

---

<img width="960" height="505" alt="Screenshot 2026-07-18 052800" src="https://github.com/user-attachments/assets/c6540c17-26b0-4c85-8aa9-5ec697dadf8d" />

---

<img width="960" height="503" alt="Screenshot 2026-07-18 052556" src="https://github.com/user-attachments/assets/4211f325-c933-4bc4-9edd-17549eb845c0" />

---

<img width="960" height="503" alt="Screenshot 2026-07-18 060806" src="https://github.com/user-attachments/assets/55a380bf-e50a-4885-8fbe-ed4ed44e721e" />

---

<img width="960" height="507" alt="Screenshot 2026-07-18 051936" src="https://github.com/user-attachments/assets/36a47f74-5894-49d7-b595-dfc7719cffb9" />

---

<img width="960" height="500" alt="Screenshot 2026-07-18 062320" src="https://github.com/user-attachments/assets/ff0eec99-d085-4ba3-8f8b-d31fab90bea4" />

---

<img width="960" height="505" alt="Screenshot 2026-07-18 063501" src="https://github.com/user-attachments/assets/a6b91176-299f-427e-9849-a3ea5e392160" />

---

<img width="960" height="503" alt="Screenshot 2026-07-18 062143" src="https://github.com/user-attachments/assets/a04c2872-9e8c-41cc-bb14-a7b6d200376d" />


---

# 🛠 Prerequisites

- AWS Account
- Docker
- Kubernetes Cluster (Amazon EKS)
- Jenkins
- GitHub
- Docker Hub
- SonarQube
- ArgoCD
- Prometheus
- Grafana

---

# 👨‍💻 Author

**Akash Yadav**
