# Production-Grade Cloud-Native DevOps Platform

A production-focused DevOps implementation of the OpenTelemetry Demo microservices application, covering the complete lifecycle from containerization and infrastructure provisioning to Kubernetes deployment, GitOps, observability, autoscaling, security, resilience, and AWS cost optimisation.

The project uses **Docker, AWS, Terraform, Amazon EKS, Kubernetes, Helm, GitHub Actions, Argo CD, Karpenter, OpenTelemetry, Prometheus, Grafana, CloudWatch, and AWS managed services** to demonstrate how a real-world microservices platform can be built, deployed, operated, secured, and observed in production.

Key areas include:

* Multi-stage, multi-platform Docker builds targeting AMD64 and ARM64, with images published to Amazon ECR.
* Reproducible AWS infrastructure provisioned with Terraform, including VPC, EKS, RDS, ElastiCache, DynamoDB, SQS, IAM, and remote state management.
* Production Kubernetes workloads on Amazon EKS with Helm, Ingress, AWS Load Balancers, TLS, External DNS, resource requests/limits, RBAC, HPA, StatefulSets, persistent storage, and the EBS CSI driver.
* GitHub Actions CI/CD pipelines integrated with Argo CD for GitOps-based deployments, automated synchronization, self-healing, and rollback.
* Karpenter-based cluster autoscaling with Spot instances, interruption handling, and workload disruption controls to optimize infrastructure costs.
* End-to-end observability using OpenTelemetry instrumentation and collectors, Prometheus metrics, Grafana dashboards, CloudWatch logs, and AWS X-Ray tracing.
* Resilient Spot interruption handling using AWS EventBridge, SQS, Kubernetes PodDisruptionBudgets, and graceful workload replacement.
* Production security using least-privilege IAM, Kubernetes RBAC, AWS Secrets Manager, IMDSv2, and secure workload-to-AWS authentication.
* Environment-aware Helm configuration and deployment patterns for managing complex microservices consistently across environments.
* Production troubleshooting across Kubernetes workloads, EKS nodes, Terraform state, networking, AWS integrations, and distributed services.
* Local development with Docker Compose before promoting workloads through the CI/CD and GitOps pipeline.
* Automatic analysis and promotion using ArgoCD and Prometheus.

The goal is to go beyond simply deploying an application and demonstrate the engineering practices required to **build, secure, observe, scale, troubleshoot, and operate a cloud-native platform as a production system**.
