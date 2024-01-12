# Kubernetes Deployment for SonarQube

## Overview

This repository provides a basic Kubernetes deployment configuration for SonarQube. The purpose of this project is to help you learn Kubernetes concepts and practices by deploying a common tool like SonarQube in a Kubernetes cluster.

## Prerequisites

Before you begin, ensure you have the following tools installed on your machine:

- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)
- [Minikube](https://minikube.sigs.k8s.io/docs/start/)
- [Docker](https://docs.docker.com/get-docker/)

## Getting Started

1. **Start Minikube Cluster:**

   ```bash
   minikube start
   ```

2. **Apply SonarQube Deployment:**

   ```bash
   kubectl apply -f sonarqube-deployment.yaml
   ```

3. **Access SonarQube:**

   ```bash
   minikube service sonarqube-service
   ```

4. **Apply SonarQube Deployment:**

   Once you are done experimenting, clean up the resources:
   ```bash
   kubectl delete -f sonarqube-deployment.yaml
   ```
   Stop Minikube:
   ```bash
   minikube stop
   ```

## Resources

- [Kubernetes Documentation](https://kubernetes.io/docs)
- [SonarQube Official Documentation](https://docs.sonarsource.com/sonarqube/latest/)

## Learn More

This project is designed to be a starting point for learning Kubernetes. Feel free to explore and modify the Kubernetes deployment files (sonarqube-deployment.yaml) to deepen your understanding.

If you encounter issues or have questions, refer to the official documentation or seek help from the Kubernetes community.

Happy learning!
