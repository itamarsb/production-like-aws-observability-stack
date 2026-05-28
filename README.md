# Production-Like AWS Deployment with Observability Stack

Production-like cloud deployment project using AWS, Docker, ECS, RDS, Terraform and a complete observability stack with Prometheus, Grafana, Loki and OpenTelemetry.

---

# Overview

This project was created to simulate a real-world cloud-native deployment environment using AWS services and observability tools commonly adopted in modern DevOps, SRE and Platform Engineering teams.

The main objective is to demonstrate:

- Cloud infrastructure provisioning
- Containerized application deployment
- Managed database integration
- Infrastructure as Code (IaC)
- CI/CD automation
- Metrics, logs and traces collection
- Monitoring and observability practices
- Production-like architecture concepts

This repository is also part of my professional transition into Cloud, DevOps, SRE and Observability Engineering.

---

# Project Goals

- Build a production-like AWS environment
- Deploy containerized applications with Docker
- Use Amazon ECS for orchestration
- Store images in Amazon ECR
- Use Amazon RDS PostgreSQL
- Implement observability with Prometheus, Grafana, Loki and OpenTelemetry
- Automate deployments with GitHub Actions
- Apply Infrastructure as Code with Terraform
- Document the entire architecture and troubleshooting process

---

# Architecture

## High-Level Architecture

```text

![Architecture](diagrams/high-level-architecture.png)

```

---

# AWS Services Used

| Service | Purpose |
|---|---|
| Amazon EC2 | Initial development environment |
| Amazon ECS | Container orchestration |
| Amazon ECR | Docker image registry |
| Amazon RDS | Managed PostgreSQL database |
| IAM | Access management |
| CloudWatch | Basic monitoring |
| Security Groups | Network security |
| VPC | Network isolation |

---

# Observability Stack

## Prometheus
Used for metrics collection and monitoring.

Examples:
- CPU usage
- Memory usage
- Container metrics
- Application metrics
- Request latency

## Grafana
Used for dashboards and visualization.

Dashboards include:
- ECS metrics
- Docker containers
- PostgreSQL monitoring
- Application health
- Infrastructure overview

## Loki
Centralized logging platform for containers and applications.

## OpenTelemetry
Distributed tracing and telemetry collection.

---

# Technologies

| Category | Technologies |
|---|---|
| Cloud | AWS |
| Containers | Docker |
| Orchestration | ECS |
| Database | PostgreSQL |
| IaC | Terraform |
| CI/CD | GitHub Actions |
| Monitoring | Prometheus |
| Visualization | Grafana |
| Logging | Loki |
| Tracing | OpenTelemetry |
| Version Control | Git |

---

# Repository Structure

```text
production-like-aws-observability-stack/
├── app/
├── infra/
├── observability/
├── docs/
├── diagrams/
├── screenshots/
├── scripts/
└── .github/workflows/
```

---

# Infrastructure as Code

Terraform will be used to provision:

- ECS Cluster
- ECR Repository
- RDS PostgreSQL
- Security Groups
- Networking resources
- IAM roles and policies

---

# CI/CD Pipeline

Planned CI/CD workflow:

```text
Git Push
   ↓
GitHub Actions
   ↓
Docker Build
   ↓
Push to Amazon ECR
   ↓
Deploy to Amazon ECS
   ↓
Health Check
```

---

# Deployment Workflow

## Local Environment

```bash
docker compose up -d
```

## Build Docker Image

```bash
docker build -t app-name .
```

## Push to ECR

```bash
./scripts/build.sh
```

## Deploy to ECS

```bash
./scripts/deploy.sh
```

---

# Screenshots

## Planned screenshots

- AWS ECS Cluster
- ECS Tasks
- Amazon RDS
- Grafana Dashboards
- Prometheus Metrics
- Loki Logs
- GitHub Actions Pipeline
- Docker Containers
- Terraform Apply
- OpenTelemetry Traces

---

# Troubleshooting

## Example Issues

### ECS task failing to connect to RDS

Possible causes:
- Incorrect security group rules
- Database endpoint mismatch
- IAM permissions
- Networking issues

### Docker container exiting unexpectedly

Possible causes:
- Environment variables missing
- Port conflicts
- Application startup failure

---

# Security Considerations

- Principle of least privilege with IAM
- Restricted Security Groups
- Secrets management
- Private networking
- Secure container deployment practices

---

# Cost Optimization

This project aims to stay within AWS Free Tier limits whenever possible.

Main strategies:
- Use t3.micro instances
- Avoid unnecessary resources
- Shutdown unused environments
- Monitor resource consumption

---

# Future Improvements

- Kubernetes migration (EKS)
- Auto Scaling
- HTTPS with Load Balancer
- Blue/Green deployments
- Chaos Engineering experiments
- Alerting integrations
- Multi-AZ database deployment
- Distributed tracing dashboards

---

# Learning Objectives

This project was designed to improve skills in:

- AWS Cloud
- DevOps
- Observability Engineering
- SRE concepts
- Infrastructure Automation
- Monitoring and Logging
- CI/CD pipelines
- Production-like deployments

---

# Roadmap

- [x] Initial repository structure
- [x] Initial README
- [ ] Dockerized application
- [ ] Amazon ECS deployment
- [ ] Amazon ECR integration
- [ ] Amazon RDS integration
- [ ] Terraform provisioning
- [ ] GitHub Actions CI/CD
- [ ] Prometheus setup
- [ ] Grafana dashboards
- [ ] Loki integration
- [ ] OpenTelemetry instrumentation
- [ ] Final architecture documentation

---

# Author

Itamar de Sá Britto Júnior

Computer Engineering Student | AWS Certified Cloud Practitioner | Cloud / DevOps / Observability Enthusiast

LinkedIn:
https://www.linkedin.com/in/itamar-de-sa-britto-jr

---

# Disclaimer

This project is intended for educational, portfolio and professional development purposes.
