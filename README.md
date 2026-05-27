# production-like-aws-observability-stack

Production-like AWS deployment using Docker, ECS, RDS, Terraform, GitHub Actions and an observability stack with Prometheus, Grafana, Loki and OpenTelemetry.

production-like-aws-observability-stack/

├── README.md
├── LICENSE
├── .gitignore
├── docker-compose.yml
├── docs/
│   ├── architecture.md
│   ├── deployment-guide.md
│   ├── observability-guide.md
│   ├── troubleshooting.md
│   └── cost-estimation.md
├── diagrams/
│   ├── architecture.drawio
│   └── architecture.png
├── app/
│   ├── frontend/
│   └── backend/
├── infra/
│   └── terraform/
│       ├── main.tf
│       ├── variables.tf
│       ├── outputs.tf
│       └── README.md
├── observability/
│   ├── prometheus/
│   ├── grafana/
│   ├── loki/
│   └── otel-collector/
├── scripts/
│   ├── build.sh
│   ├── deploy.sh
│   └── destroy.sh
├── screenshots/
└── .github/
    └── workflows/
        └── ci-cd.yml

# Production-Like AWS Deployment with Observability Stack

## 1. Overview
## 2. Architecture
## 3. Technologies
## 4. AWS Services
## 5. Observability Stack
## 6. Deployment Steps
## 7. CI/CD Pipeline
## 8. Screenshots
## 9. Troubleshooting
## 10. Cost Considerations
## 11. Roadmap
## 12. Author

Roadmap:

- [x] Local Docker environment
- [x] AWS EC2 deployment
- [x] PostgreSQL with Amazon RDS
- [x] Image registry with Amazon ECR
- [x] Container orchestration with Amazon ECS
- [ ] Infrastructure as Code with Terraform
- [ ] CI/CD with GitHub Actions
- [ ] Metrics with Prometheus
- [ ] Dashboards with Grafana
- [ ] Logs with Loki
- [ ] Traces with OpenTelemetry
- [ ] Alerting rules
- [ ] Final architecture documentation

