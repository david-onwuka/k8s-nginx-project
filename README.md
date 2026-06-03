# Kubernetes Nginx Deployment Project

## Overview
This project demonstrates a basic Kubernetes deployment using Minikube.  
It deploys an Nginx web server using Kubernetes Deployments and exposes it using a NodePort Service.

---

## Architecture

- Kubernetes Cluster (Minikube)
- Deployment (2 replicas of Nginx)
- Service (NodePort exposure)
- Browser access via Minikube URL

---

## Tools Used

- Kubernetes
- Minikube
- kubectl
- Git & GitHub
- Nginx Docker Image

---

## Deployment Steps

### 1. Apply Deployment
```bash
kubectl apply -f nginx-deployment.yaml
```

### 2. Apply Service
```bash
kubectl apply -f nginx-service.yaml
```

### 3. Access Application
```bash
minikube service nginx-service --url
```

---

## Project Structure

```
k8s-nginx-project/
├── nginx-deployment.yaml
├── nginx-service.yaml
└── README.md
```

---

## Key Learnings

- Kubernetes Deployments and Pods
- Service exposure using NodePort
- Self-healing and scaling
- Infrastructure as Code (YAML)
- GitHub project versioning

---

## Result

A containerized web application running on Kubernetes and accessible via browser.
