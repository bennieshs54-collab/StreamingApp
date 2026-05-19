# StreamingApp - Orchestration and Scaling Project

## Project Overview

This project demonstrates the deployment, orchestration, CI/CD automation, scaling, and monitoring of a MERN Stack Streaming Application using AWS cloud services.

The project includes:

- Docker Containerization
- Jenkins CI/CD Pipeline
- Amazon ECR
- Amazon EKS
- Helm Charts
- CloudWatch Monitoring
- Kubernetes Scaling

---

# Technology Stack

| Technology | Purpose |
|---|---|
| React.js | Frontend |
| Node.js | Backend |
| Express.js | API |
| MongoDB | Database |
| Docker | Containerization |
| Jenkins | CI/CD |
| Amazon ECR | Image Repository |
| Amazon EKS | Kubernetes Cluster |
| Helm | Kubernetes Package Manager |
| CloudWatch | Monitoring & Logging |

---

# Project Architecture

GitHub → Jenkins → Docker → Amazon ECR → Amazon EKS → Helm → CloudWatch

---

# Clone Repository

```bash
git clone https://github.com/YOUR_USERNAME/StreamingApp.git
cd StreamingApp
```

---

# Docker Setup

## Backend Build

```bash
cd backend
docker build -t streaming-backend .
```

## Frontend Build

```bash
cd frontend
docker build -t streaming-frontend .
```

---

# AWS ECR Setup

## Create ECR Repositories

```bash
aws ecr create-repository --repository-name streaming-backend

aws ecr create-repository --repository-name streaming-frontend
```

---

# Jenkins Pipeline

Jenkins automates:

- Code Pull
- Docker Build
- Docker Push
- Kubernetes Deployment

---

# EKS Cluster Creation

```bash
eksctl create cluster \
--name streaming-cluster \
--region ap-south-1 \
--nodegroup-name workers \
--node-type t3.medium \
--nodes 2
```

---

# Kubernetes Deployment

```bash
kubectl apply -f kubernetes/
```

---

# Helm Deployment

```bash
helm install streaming-release ./helm/streaming-app
```

---

# Monitoring

CloudWatch is used for:

- Pod Logs
- Container Logs
- Metrics
- Monitoring

---

# Scaling

```bash
kubectl scale deployment backend --replicas=4
```

---

# Screenshots

Screenshots available in:

<img width="940" height="449" alt="image" src="https://github.com/user-attachments/assets/e627a48b-fcaf-46e3-920a-2eb3ec7f9d74" />

<img width="940" height="385" alt="image" src="https://github.com/user-attachments/assets/14f42073-b721-4001-a01b-5d5c01caada9" />

<img width="940" height="253" alt="image" src="https://github.com/user-attachments/assets/266e12aa-93e5-4c18-b91c-0a7c69085759" />

<img width="940" height="503" alt="image" src="https://github.com/user-attachments/assets/a49c3262-2017-4bc3-a6f3-8fbbc714e007" />

<img width="940" height="502" alt="image" src="https://github.com/user-attachments/assets/9105c8c9-8b70-485e-9757-424cd180cc06" />

<img width="940" height="506" alt="image" src="https://github.com/user-attachments/assets/c4f961ef-cfaf-4f2b-80e0-8fd62bbeb9fd" />

<img width="940" height="380" alt="image" src="https://github.com/user-attachments/assets/381ea768-a8b2-43b5-8dc8-fb62a4bb37e3" />

<img width="940" height="205" alt="image" src="https://github.com/user-attachments/assets/9e87a27c-8fba-4bf6-bfd6-a9eaf73dcc32" />

<img width="940" height="436" alt="image" src="https://github.com/user-attachments/assets/c1313a6a-fbe6-4ffa-acbc-5993c90bd09c" />

<img width="940" height="237" alt="image" src="https://github.com/user-attachments/assets/c8064088-a00a-49dc-ba41-72730996ca69" />

<img width="940" height="431" alt="image" src="https://github.com/user-attachments/assets/dda1850d-03c9-48cc-b751-6d6efd041d6a" />

<img width="940" height="539" alt="image" src="https://github.com/user-attachments/assets/69d1586a-6103-4aad-bd8c-480392da043f" />

<img width="940" height="456" alt="image" src="https://github.com/user-attachments/assets/1f0d250e-4e8e-429a-8879-ee496b4c2c17" />

<img width="940" height="451" alt="image" src="https://github.com/user-attachments/assets/d77d2b79-af5d-4c80-9d6b-b219dc44dede" />

<img width="940" height="442" alt="image" src="https://github.com/user-attachments/assets/8f1c61ee-5677-40b8-aa42-a8b763e99786" />

<img width="940" height="256" alt="image" src="https://github.com/user-attachments/assets/2f243b7f-cb4b-4e1f-85ee-f62f778fd8e1" />

<img width="940" height="482" alt="image" src="https://github.com/user-attachments/assets/de725739-de20-4de1-a844-a5df33f36119" />

<img width="940" height="549" alt="image" src="https://github.com/user-attachments/assets/7c4c3336-89a0-4ddd-9556-5a051de81a2a" />

<img width="940" height="501" alt="image" src="https://github.com/user-attachments/assets/ff0f4b5f-d6d6-4712-8f1d-ce4d70ab6ff7" />

<img width="940" height="435" alt="image" src="https://github.com/user-attachments/assets/c78b1134-1b59-4f00-ac73-df4e04c16610" />

<img width="940" height="454" alt="image" src="https://github.com/user-attachments/assets/62a13d32-6c12-45eb-83f0-69abf4311e3b" />

<img width="940" height="498" alt="image" src="https://github.com/user-attachments/assets/5fb77856-fa04-451a-8afc-b227809f2198" />

<img width="940" height="811" alt="image" src="https://github.com/user-attachments/assets/5f220204-82e3-49a6-8734-5e40e5a88158" />

<img width="940" height="482" alt="image" src="https://github.com/user-attachments/assets/05aa408e-0f17-4cf3-9e12-b6b14cb53c29" />























