Extreme CI/CD Pipeline & Multi-Cloud Deployment for Mobile Applications

📌 Overview

This project implements a fully automated CI/CD pipeline for a mobile application that ensures seamless deployment across AWS and GCP. It includes automated rollback mechanisms, observability integration, and multi-cloud deployment simulation.

📂 Repository Structure

/ci-cd         # CI/CD pipeline configuration files
/scripts       # Deployment, rollback, and monitoring scripts
/src           # Mobile application source code
/tests         # Unit, integration, and UI test scripts
/docs          # Documentation and screenshots

🚀 CI/CD Pipeline Workflow

1️⃣ Build Stage

Install dependencies

Run static analysis (linting, formatting)

Compile the mobile application

2️⃣ Test Stage

Execute unit, integration, and UI tests

Enforce a minimum of 80% test coverage

Publish test coverage badges

3️⃣ Deploy Stage

Android & iOS builds created (APK & IPA)

Deploy to AWS (Elastic Beanstalk/ECS) & GCP (Cloud Run)

Push Docker images to AWS ECR & Google Container Registry

4️⃣ Observability & Monitoring

Prometheus for collecting custom metrics

Grafana dashboards for real-time visualization

Automated alerts via Slack/email for failures

5️⃣ Automated Rollback

If error rate >5%, rollback is triggered

Deployment reverts to last stable release

Logs captured for debugging

🛠️ Deployment Scripts

AWS Deployment (``)

Builds & pushes the Docker image to AWS ECR

Deploys to AWS ECS using update-service

GCP Deployment (``)

Builds & pushes the Docker image to Google Container Registry

Deploys to Google Cloud Run

Rollback (``)

Reverts AWS/GCP deployment to the last stable release

Triggered automatically when failure conditions are met

Monitoring & Observability (**, **)

Sends metrics to Prometheus

Updates Grafana dashboards with latest deployment data

📸 Evidence & Screenshots

✅ CI/CD Pipeline Execution Logs ✅ Prometheus Metrics & Grafana Dashboard ✅ Multi-Cloud Deployment Success Logs ✅ Automated Rollback Demonstration

📌 Submission Checklist

✅ GitHub Repository: XNL-21BCEXXXX-MAD-3 ✅ Add `` as a collaborator ✅ Commit logs with detailed messages ✅ Screenshots & d
