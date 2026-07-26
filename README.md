# 🚀 BlogOps - End-to-End DevSecOps CI/CD Pipeline on Amazon EKS

![Jenkins](https://img.shields.io/badge/Jenkins-CI-red)
![Docker](https://img.shields.io/badge/Docker-Containerization-blue)
![Kubernetes](https://img.shields.io/badge/Kubernetes-EKS-326CE5)
![ArgoCD](https://img.shields.io/badge/ArgoCD-GitOps-orange)
![SonarQube](https://img.shields.io/badge/SonarQube-Code%20Quality-brightgreen)
![Trivy](https://img.shields.io/badge/Trivy-Security-blueviolet)
![Prometheus](https://img.shields.io/badge/Prometheus-Monitoring-orange)
![Grafana](https://img.shields.io/badge/Grafana-Dashboard-F46800)

---

# 📖 Overview

**BlogOps** is a production-style **three-tier MERN application** deployed on **Amazon EKS** using a complete **DevSecOps CI/CD pipeline**.

The project automates code quality analysis, security scanning, Docker image creation, GitOps deployment, Kubernetes orchestration, and monitoring.

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
 ├── Git Checkout
 ├── Trivy Scan
 ├── OWASP Dependency Check
 ├── SonarQube Analysis
 ├── Quality Gate
 ├── Build Docker Images
 ├── Push Images to Docker Hub
 └── Trigger CD Pipeline
     │
     ▼
Jenkins CD Pipeline
 ├── Update Kubernetes Manifests
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
Amazon EKS
 ├── React Frontend
 ├── Node.js Backend
 └── MongoDB Database
     │
     ▼
Prometheus
     │
     ▼
Grafana
```

---

# 🚀 Tech Stack

## Cloud

- AWS EC2
- Amazon EKS
- IAM

## CI/CD

- Jenkins
- GitHub
- Docker Hub

## Containers

- Docker
- Kubernetes

## GitOps

- ArgoCD

## DevSecOps

- SonarQube
- Trivy
- OWASP Dependency Check

## Monitoring

- Prometheus
- Grafana

## Application

- React
- Node.js
- Express.js
- MongoDB

---

# 📂 Project Structure

```
BlogOps
│
├── frontend/
├── backend/
├── kubernetes/
├── Automations/
├── database/
├── GitOps/
├── Jenkinsfile
├── docker-compose.yml
└── README.md
```

---

# ⚙ CI Pipeline

The Jenkins CI pipeline performs:

- Source Code Checkout
- Filesystem Vulnerability Scan using Trivy
- Dependency Vulnerability Scan using OWASP Dependency Check
- Static Code Analysis using SonarQube
- Quality Gate Validation
- Backend & Frontend Environment Configuration
- Docker Image Build
- Docker Image Push to Docker Hub
- Trigger Jenkins CD Pipeline

---

# 🚀 CD Pipeline

The Jenkins CD pipeline performs:

- Checkout GitHub Repository
- Update Kubernetes Deployment Image Tags
- Commit Updated Manifests
- Push Changes to GitHub
- ArgoCD Detects Changes
- Automatic Deployment to Amazon EKS

---

# 🔒 Security

Security scanning is integrated into the CI pipeline.

### Trivy

- Filesystem Scan
- Docker Image Scan

### OWASP Dependency Check

- Detects vulnerable third-party libraries
- Generates XML security report

### SonarQube

- Code Quality
- Bugs
- Vulnerabilities
- Code Smells
- Quality Gate Validation

---

# ☸ Kubernetes

Application consists of

- Frontend Deployment
- Backend Deployment
- MongoDB Deployment
- Services
- ConfigMaps
- Secrets

---

# 📊 Monitoring

Monitoring stack includes

- Prometheus
- Grafana

Used for

- Cluster Monitoring
- Pod Monitoring
- Node Metrics
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

# 🔄 CI/CD Flow

```
Code Commit
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
Code Quality Check
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
GitHub Manifest Update
      │
      ▼
ArgoCD
      │
      ▼
Amazon EKS
      │
      ▼
Prometheus + Grafana
```

---

# 📸 Screenshots

Add screenshots for

- Jenkins CI Pipeline
- Jenkins CD Pipeline
- SonarQube Dashboard
- Trivy Scan
- Docker Hub Images
- ArgoCD Dashboard
- Kubernetes Pods
- Prometheus Dashboard
- Grafana Dashboard
- BlogOps Application

---

# ✨ Features

- Automated CI/CD Pipeline
- GitOps Deployment
- Static Code Analysis
- Dependency Vulnerability Scan
- Filesystem Vulnerability Scan
- Docker Image Automation
- Kubernetes Deployment
- Automatic GitHub Manifest Update
- Monitoring & Alerting
- Production Style Architecture

---

# 🎯 Future Improvements

- Helm Charts
- Horizontal Pod Autoscaler
- Ingress Controller
- AWS Load Balancer Controller
- Terraform Infrastructure
- Slack Notifications
- Blue/Green Deployment

---

# 👨‍💻 Author

**Akash Yadav**

DevOps Engineer | AWS | Docker | Kubernetes | Jenkins | ArgoCD | GitHub | SonarQube | Prometheus | Grafana

GitHub: https://github.com/akashyadav29
LinkedIn: *Add your LinkedIn profile here*

---

# ⭐ If you like this project, give it a Star!
