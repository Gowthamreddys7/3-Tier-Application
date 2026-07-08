# 🚀 3-Tier Application CI/CD Pipeline on Kubernetes (Kops)

## 📌 Project Overview

This project demonstrates an end-to-end CI/CD pipeline for a Java-based 3-tier web application deployed on a Kubernetes cluster provisioned using **Kops** on AWS.

The pipeline automates the complete software delivery process, including application build, artifact management, containerization, image publishing, and deployment to Kubernetes.

## 🛠️ Tech Stack

- Git & GitHub
- Jenkins
- Maven
- Nexus Repository
- Docker
- Docker Hub
- Kubernetes (Kops)
- NGINX Ingress
- MySQL
- RabbitMQ
- Memcached
- Elasticsearch
- AWS EC2
  
## 🔄 CI/CD Workflow

1. Developer pushes code to GitHub.
2. Jenkins triggers the pipeline.
3. Maven builds the application and generates the WAR file.
4. WAR artifact is uploaded to Nexus Repository.
5. Docker images are built.
6. Images are pushed to Docker Hub.
7. Jenkins deploys the application to the Kubernetes cluster.
8. The application is exposed using NGINX Ingress.

## 📂 Project Structure

├── Dockerfiles
├── Kubernetes
│   ├── Manifest-appl
│   ├── Manifest-db
│   ├── rabbitmq
│   ├── memcached
│   ├── elasticsearch
│
├── src
├── pom.xml
├── Jenkinsfile
└── README.md
├── images
│   ├── architecture.png
│   ├── pods.png
│   ├── application-interface.png
│   ├── login-page.png
│   └── jenkins-pipeline.png

## ⚙️ Jenkins Pipeline

Pipeline Stages:

- Checkout Code
- Build Application
- Upload WAR to Nexus
- Build Docker Images
- Push Images to Docker Hub
- Deploy to Kubernetes
  
## 📚 Key Learnings

- CI/CD pipeline automation with Jenkins
- Artifact management using Nexus Repository
- Docker image creation and publishing
- Kubernetes Deployments, StatefulSets, Services, Ingress, and HPA
- Kubernetes cluster management using Kops
- Troubleshooting rollout failures and resource quota issues
- Managing stateful workloads in Kubernetes
  
## 🚀 Future Improvements

- Implement GitOps using Argo CD
- Add monitoring with Prometheus and Grafana
- Configure HTTPS using Cert-Manager
- Add centralized logging with the ELK Stack
- Integrate vulnerability scanning into the CI/CD pipeline

## 👤 Author

**Goutham Reddy**

If you found this project helpful, feel free to ⭐ the repository.
