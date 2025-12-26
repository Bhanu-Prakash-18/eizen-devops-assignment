# Eizen.ai DevOps Assignment

This repository contains my solution for the DevOps technical assignment.

## Completed Tasks
- Dockerized Flask application
- Kubernetes deployment using Minikube
- Service exposure using NodePort

## Docker
Build image:
docker build -t flask-app:latest .

## Kubernetes (Minikube)
Start cluster:
minikube start --driver=docker

Point docker to minikube:
eval $(minikube docker-env)

Deploy:
kubectl apply -f kubernetes/deployment.yaml
kubectl apply -f kubernetes/service.yaml

Access app:
minikube service flask

## Remaining Tasks
- Bash automation, Jenkins, Terraform, CI/CD, monitoring are documented as design approach due to time constraints.

