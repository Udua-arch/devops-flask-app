[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)
[![Docker](https://img.shields.io/badge/Docker-published-blue)](https://hub.docker.com/)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-ready-blue)](https://kubernetes.io/)
[![CI/CD](https://github.com/Udua-arch/devops-flask-app/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Udua-arch/devops-flask-app/actions/workflows/ci-cd.yml)


# DevOps Flask App

This project demonstrates a full DevOps workflow: building, containerizing, and deploying a web service.

### Features

- Python Flask API
- Docker Containerization
- Kubernetes Deployment Manifests
- GitHub Actions CI/CD Pipeline

### Run Locally

```
docker build -t devops-app .
docker run -p 8080:8080 devops-app
```

### Deploy to Minikube

```
minikube start
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
kubectl get svc devops-service
```

## Badges

[![Python](https://img.shields.io/badge/Python-3.10-blue)](https://www.python.org/)
[![Docker](https://img.shields.io/badge/Docker-published-blue)](https://hub.docker.com/)
[![Kubernetes](https://img.shields.io/badge/Kubernetes-ready-blue)](https://kubernetes.io/)
[![CI/CD](https://github.com/Udua-arch/devops-flask-app/actions/workflows/ci-cd.yml/badge.svg)](https://github.com/Udua-arch/devops-flask-app/actions/workflows/ci-cd.yml)
![Docker Image Version (latest)](https://img.shields.io/docker/v/uduarch/devops-app?sort=semver)



## DockerHub

This project is configured to push the built Docker image to **DockerHub** under the repository `uduarch/devops-app`.
To enable automatic pushes from GitHub Actions:

The GitHub Actions workflow `ci-cd.yml` will then build and push `uduarch/devops-app:latest` on every push to `main`.

hub.docker.com/repository/docker/uduarch/devops-app/general

## Architecture Diagram

See `architecture.png` for a simple diagram showing how the pieces connect.

---

trigger
retry
