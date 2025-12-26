# Task 4 – AWS Production Deployment using Terraform

This task describes how the application would be deployed to AWS in a production environment using Terraform.

## Architecture Overview
- Docker images are built by CI/CD
- Images are pushed to Amazon ECR
- Application is deployed to Amazon EKS
- IAM roles are used to grant least-privilege access

---

## Resources Managed by Terraform

### Amazon ECR
- Stores Docker images
- Used by EKS to pull application images

Terraform resource:
- aws_ecr_repository

---

### Amazon EKS
- Managed Kubernetes cluster
- Runs application workloads
- Uses worker node groups

Terraform resources:
- aws_eks_cluster
- aws_eks_node_group

---

### IAM Roles and Policies

#### CI/CD Role (GitHub Actions / Jenkins)
Permissions required:
- ecr:GetAuthorizationToken
- ecr:PutImage
- ecr:InitiateLayerUpload
- ecr:CompleteLayerUpload
- eks:DescribeCluster
- eks:UpdateClusterConfig

#### EKS Node Role
Permissions required:
- Pull images from ECR
- Write logs to CloudWatch

---

## Deployment Flow
1. CI/CD pipeline builds Docker image
2. Image is pushed to Amazon ECR
3. Terraform provisions / updates EKS
4. Kubernetes manifests are applied to EKS
5. Application is exposed using a LoadBalancer or Ingress

---

## Notes
Actual AWS infrastructure provisioning is not executed in this assignment due to time and cost constraints.

