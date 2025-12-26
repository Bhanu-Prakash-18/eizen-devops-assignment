# Task 5 – CI/CD Pipeline (GitHub Actions)

This pipeline represents a CI/CD workflow for deploying the application.

## Pipeline Flow
1. Code pushed to main branch
2. Docker image is built
3. Image is pushed to ECR (in production)
4. Application is deployed to EKS

## Notes
Actual deployment steps are not executed in this assignment due to lack of AWS credentials.

