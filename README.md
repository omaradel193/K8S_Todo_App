# 📝 Todo App - Overview

This repository contains Kubernetes manifests to deploy a **Todo App** with a **MySQL database**. The application is exposed using **Ingress**, scaled with **HPA**, and secured using **Secrets**.

## 🚀 Features
✅ **Containerized Todo App** deployed on Kubernetes  
✅ **MySQL StatefulSet** with Persistent Volume for data storage  
✅ **Ingress Controller** for external access  
✅ **Horizontal Pod Autoscaler (HPA)** for auto-scaling  
✅ **Secrets & ConfigMaps** for managing credentials and environment variables  

## 🛠️ Technologies Used
- **Kubernetes** (Minikube / EKS)
- **Docker** (for containerization)
- **MySQL** (database)
- **Ingress** (for routing)
- **HPA** (auto-scaling)
- **Secrets** (configuration management)

## 🎯 Deployment Steps
### 1️⃣ Start Minikube  
```bash
minikube start
```
### 2️⃣ Apply Kubernetes Manifests
```bash
kubectl apply -f .
```
### 3️⃣ Verify Deployment
```bash
kubectl get pods,services,deployments,ingress
```
### 4️⃣ Access the Application
Ensure your /etc/hosts file has the correct domain mapping:
```bash
192.168.49.2  todo-app.com
```
Open http://todo-app.com in your browser.



