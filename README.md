# Kubernetes Multi-Tier Application

## Objective

This project demonstrates a simple multi-tier application deployed on Kubernetes using Deployments, Services, and Persistent Volumes.

## Architecture

Frontend (Nginx)
↓
Service
↓
Database (MySQL)
↓
Persistent Volume Claim

## Kubernetes Resources

### Deployments

* Frontend Deployment
* MySQL Deployment

### Services

* Frontend Service

### Storage

* Persistent Volume Claim for MySQL data

## Commands Used

Apply resources:

```bash
kubectl apply -f frontend-deployment.yaml
kubectl apply -f frontend-service.yaml
kubectl apply -f database-deployment.yaml
kubectl apply -f persistent-volume.yaml
```

Verify resources:

```bash
kubectl get deployments
kubectl get services
kubectl get pvc
```

## What I Learned

* Kubernetes Deployments
* Kubernetes Services
* Persistent Volumes and PVCs
* Multi-tier application architecture
* Container orchestration concepts

## Challenges Faced

Understanding how Deployments, Services, and Persistent Volumes work together in a Kubernetes environment was initially challenging. Through studying Kubernetes architecture and YAML configurations, I gained a better understanding of multi-tier application deployment.
