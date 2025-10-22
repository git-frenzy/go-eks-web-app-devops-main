# 🦦 Go Web App — Kubernetes EKS | Helm | Docker | AWS Integration

[![Go](https://img.shields.io/badge/Go-1.21+-blue?logo=go)](https://go.dev/)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-EKS-blue?logo=kubernetes)](https://aws.amazon.com/eks/)
[![Helm](https://img.shields.io/badge/Helm-Chart-orange?logo=helm)](https://helm.sh/)
[![Docker](https://img.shields.io/badge/Docker-Containerization-blue?logo=docker)](https://www.docker.com/)
[![AWS](https://img.shields.io/badge/AWS-Cloud-yellow?logo=amazon-aws)](https://aws.amazon.com/)
[![License](https://img.shields.io/badge/License-MIT-green.svg)](LICENSE)

---

## 🌐 Demo (Static Overview)
> The live cluster isn’t currently hosted due to budget constraints.  
> However, you can explore a **static demo and overview** of this project here:  
> 🔗 [Go EKS Web App Demo (S3 Hosted)](http://go-eks-web-app-devops-main.s3-website-us-east-1.amazonaws.com/home.html)

---

## 🚀 Project Overview
This project demonstrates a **cloud-native Go web application** deployed using:
- **Docker** for containerization  
- **Helm** for Kubernetes deployment management  
- **Amazon EKS** for orchestration  
- **AWS services** (S3, ECR, CloudWatch, IAM) for integration  

It serves as a complete DevOps example for scalable Go applications in a production-like AWS environment.

---

## 🧱 Architecture Overview

```mermaid
graph TD
A[Developer] --> B[GitHub Repository]
B --> C[GitHub Actions / Jenkins CI]
C --> D[Docker Build & Push → AWS ECR]
D --> E[Helm Deploy → EKS Cluster]
E --> F[Go Web App Pods]
F --> G[CloudWatch Logs & Metrics]
F --> H[Public Load Balancer / Ingress]
