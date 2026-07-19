# 🚀 AWS DevOps Handbook

::: {align="center"}
# AWS DevOps Handbook

### Enterprise-Grade CI/CD • GitOps • Kubernetes • Observability on AWS

![AWS](https://img.shields.io/badge/AWS-Cloud-orange?style=for-the-badge&logo=amazonaws)
![Docker](https://img.shields.io/badge/Docker-Container-blue?style=for-the-badge&logo=docker)
![Kubernetes](https://img.shields.io/badge/Kubernetes-EKS-326CE5?style=for-the-badge&logo=kubernetes)
![GitHub
Actions](https://img.shields.io/badge/GitHub_Actions-CI/CD-2088FF?style=for-the-badge&logo=githubactions)
![ArgoCD](https://img.shields.io/badge/ArgoCD-GitOps-EF7B4D?style=for-the-badge&logo=argo)
![Prometheus](https://img.shields.io/badge/Prometheus-Monitoring-E6522C?style=for-the-badge&logo=prometheus)
![Grafana](https://img.shields.io/badge/Grafana-Dashboards-F46800?style=for-the-badge&logo=grafana)
![Loki](https://img.shields.io/badge/Loki-Logging-2F4F4F?style=for-the-badge)
:::

------------------------------------------------------------------------

## 📖 Overview

AWS DevOps Handbook demonstrates a modern DevOps workflow on AWS using
Docker, Amazon ECR, Amazon EKS, GitHub Actions, ArgoCD and a complete
observability stack.

## ✨ Features

-   Dockerized application
-   Amazon ECR image registry
-   Amazon EKS deployment
-   AWS Load Balancer Controller
-   GitHub Actions CI/CD
-   Git SHA image versioning
-   ArgoCD GitOps auto-sync
-   Prometheus metrics
-   Grafana dashboards
-   Loki centralized logging
-   Alloy log collection
-   Rolling deployments

------------------------------------------------------------------------

# 🏗 Architecture

``` text
Developer
    │
    ▼
GitHub Repository
    │
    ▼
GitHub Actions
    │
    ├── Build Docker Image
    ├── Push Image to Amazon ECR
    └── Update deployment.yaml
              │
              ▼
           ArgoCD
              │
              ▼
          Amazon EKS
              │
              ▼
AWS Load Balancer (ALB)
              │
              ▼
          End Users
```

------------------------------------------------------------------------

# 🛠 Tech Stack

  Category        Technologies
  --------------- ---------------------
  Cloud           AWS, EKS, ECR, IAM
  Containers      Docker
  Orchestration   Kubernetes
  GitOps          ArgoCD
  CI/CD           GitHub Actions
  Monitoring      Prometheus, Grafana
  Logging         Loki, Alloy
  Languages       HTML, CSS

------------------------------------------------------------------------

# 📂 Project Structure

``` text
AWS-DevOps-Handbook/
├── .github/
│   └── workflows/
├── app/
├── argocd/
├── k8s/
├── monitoring/
├── Dockerfile
└── README.md
```

------------------------------------------------------------------------

# 🔄 CI/CD Workflow

1.  Push code to GitHub
2.  GitHub Actions builds Docker image
3.  Push image to Amazon ECR
4.  Update Kubernetes deployment manifest
5.  Commit updated manifest
6.  ArgoCD detects change
7.  EKS performs rolling update
8.  ALB serves latest version

------------------------------------------------------------------------

# ☸ Kubernetes Resources

-   Deployment
-   Service
-   Ingress
-   ReplicaSet
-   Pods

------------------------------------------------------------------------

# 📊 Observability

-   Prometheus for metrics
-   Grafana dashboards
-   Loki log aggregation
-   Alloy log shipping

------------------------------------------------------------------------

# 🚀 Quick Start

``` bash
git clone <repository-url>
cd AWS-DevOps-Handbook
```

Build image:

``` bash
docker build -t aws-devops-handbook ./app
```

Push:

``` bash
docker push <your-ecr-repository>
```

Deploy:

``` bash
kubectl apply -f k8s/
```

------------------------------------------------------------------------

# 📸 Screenshots

Add screenshots here:

-   GitHub Actions
-   Amazon ECR
-   Amazon EKS
-   ArgoCD
-   Grafana
-   Prometheus
-   Loki
-   Website

------------------------------------------------------------------------

# 🎯 Learning Outcomes

-   Docker fundamentals
-   Kubernetes deployments
-   Amazon EKS
-   GitOps
-   CI/CD pipelines
-   Monitoring
-   Logging
-   AWS IAM
-   Production troubleshooting

------------------------------------------------------------------------

# 🗺 Roadmap

-   [x] Docker
-   [x] Amazon ECR
-   [x] Amazon EKS
-   [x] GitHub Actions
-   [x] ArgoCD
-   [x] ALB
-   [x] Prometheus
-   [x] Grafana
-   [x] Loki
-   [x] Alloy
-   [ ] Helm Charts
-   [ ] Terraform Infrastructure
-   [ ] DevSecOps

------------------------------------------------------------------------

# 🤝 Contributing

Contributions, issues and feature requests are welcome.

------------------------------------------------------------------------

# 👨‍💻 Author

**Dharshan R**

-   AWS & DevOps Enthusiast
-   Full Stack Developer

------------------------------------------------------------------------

# ⭐ Support

If you found this repository useful, consider giving it a ⭐ on GitHub.

------------------------------------------------------------------------

# 📄 License

This project is released under the MIT License.
