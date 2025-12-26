# Eizen.ai – DevOps Technical Assignment

This repository contains my solution for the DevOps technical assignment provided by Eizen.ai.

The assignment covers Bash automation, containerization, Kubernetes deployment, CI/CD design, cloud infrastructure, registry maintenance, and monitoring.

---

## Task Completion Summary

### Task 1 – Bash Automation & Git Hygiene  
**Location:** `bash/`

- Bash script to create files of different sizes
- Detection of files larger than 50MB
- Sorting files in descending order by size
- Git large-file cleanup, cron job, and Jenkins job explained as design approach

---

### Task 2 – Docker Compose with Nginx Reverse Proxy  
**Location:** `docker/`

- Dockerized Flask application
- Docker Compose setup
- Flask container not exposed directly
- Nginx reverse proxy with request logging

---

### Task 3 – Kubernetes Deployment (Minikube)  
**Location:** `kubernetes/`

- Local Kubernetes cluster using Minikube
- Deployment and Service manifests
- Application exposed via NodePort

---

### Task 4 – AWS Production Deployment using Terraform 
**Location:** `terraform/`

- Terraform-based design for ECR and EKS
- IAM roles and policies explained
- End-to-end deployment flow documented

---

### Task 5 – CI/CD Pipeline
**Location:** `ci/`

- Sample GitHub Actions workflow
- CI/CD pipeline flow explained (build, push, deploy)

---

### Task 6 – Container Registry Cleanup
**Location:** `registry-cleanup/`

- Strategy to identify and remove dangling images
- Example commands for Amazon ECR cleanup

---

### Task 7 – Monitoring with Grafana  
**Location:** `monitoring/`

- Kubernetes cluster metrics
- Local system metrics
- Monitoring architecture using Prometheus and Grafana

---

## Notes
Tasks involving AWS infrastructure, CI/CD execution, registry cleanup, and monitoring are documented at design level due to time and environment constraints.  
All implementations and documentation are structured in task-specific folders for clarity.

