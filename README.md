# Kubernetes Monitoring using Prometheus & Grafana

This project demonstrates an end-to-end monitoring setup for a Kubernetes cluster
using Prometheus and Grafana deployed via Helm on Minikube.

## 🚀 Tech Stack
- Kubernetes (Minikube)
- Prometheus
- Grafana
- Helm
- Docker
- Ubuntu (WSL)

## 📌 Project Overview
- Set up a local Kubernetes cluster using Minikube
- Installed Prometheus and Grafana using Helm (`kube-prometheus-stack`)
- Monitored node-level and pod-level metrics
- Explored Prometheus UI and PromQL queries
- Visualized metrics using Grafana dashboards
- Understood Kubernetes Services, ports, and port-forwarding

## 🏗 Architecture (Logical)
User Browser  
→ Grafana (port-forward)  
→ Prometheus  
→ Kubernetes Metrics (kubelet, node-exporter, kube-state-metrics)

## ⚙️ Setup Steps

### 1. Start Minikube
```bash
minikube start --driver=docker

