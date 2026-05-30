# gitops-argocd

> Phase 3 Project 2 — GitOps with ArgoCD. Git is the single source of truth.

![ArgoCD](https://img.shields.io/badge/ArgoCD-EF7B4D?style=flat&logo=argo&logoColor=white)
![Kubernetes](https://img.shields.io/badge/Kubernetes-326CE5?style=flat&logo=kubernetes&logoColor=white)
![GitOps](https://img.shields.io/badge/GitOps-enabled-green)

## How it works

git push → ArgoCD detects change → syncs cluster automatically

## Structure

k8s/deployment.yaml  — 2 replicas, health checks, resource limits
k8s/service.yaml     — NodePort service on port 80
k8s/hpa.yaml         — autoscale 2-10 pods based on CPU
