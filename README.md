# 🚀 CI/CD Pipeline Project using GitHub, Jenkins, Docker & AWS EC2

## 📌 Project Overview

This project demonstrates a complete CI/CD pipeline that automatically builds and deploys a Dockerized website using Jenkins whenever code is pushed to GitHub.

The application is containerized using Docker and deployed on an AWS EC2 instance. GitHub Webhooks trigger Jenkins automatically for continuous deployment.

---

## 🛠 Technologies Used

* GitHub
* Jenkins
* Docker
* AWS EC2
* Nginx
* GitHub Webhooks
* Amazon Linux 2023

---

## 📂 Project Structure

```text
capstone-project/
│
├── screenshots/
│   ├── github-repo.png
│   ├── jenkins-dashboard.png
│   ├── jenkins-success.png
│   ├── webhook.png
│   ├── website.png
│   └── docker-ps.png
│
├── Dockerfile
├── index.html
├── Jenkinsfile
└── README.md
```

---

## 🏗 Architecture

```text
Developer
   ↓
GitHub Repository
   ↓
GitHub Webhook
   ↓
Jenkins Pipeline
   ↓
Docker Build
   ↓
Deploy Container
   ↓
AWS EC2 Instance
   ↓
Website Running
```

---

## ⚙️ Docker Configuration

The application is containerized using Docker with an Nginx base image.

The Dockerfile:

* Uses Nginx image
* Copies website files into the Nginx web directory
* Creates a lightweight web server container

---

## 🔄 Jenkins Pipeline Stages

### 1. Clone Repository

Jenkins clones the latest code from GitHub.

### 2. Build Docker Image

Docker image is built automatically using the Dockerfile.

### 3. Deploy Container

Jenkins:

* Stops previous container
* Removes old container
* Deploys latest version automatically

---

## 🔗 Webhook Integration

GitHub Webhooks automatically trigger Jenkins whenever code changes are pushed.

Workflow:

```text
Push Code
   ↓
Webhook Trigger
   ↓
Jenkins Pipeline
   ↓
Docker Deployment
```

---

## 🌐 Deployment

The website is deployed on AWS EC2 using Docker containers.

Since AWS Educate Sandbox environments are temporary, infrastructure resources such as EC2 instances and public IP addresses may change after session expiration.

All project files remain safely stored in GitHub.

---

## ✨ Features

* Automated Deployment
* CI/CD Pipeline
* Docker Containerization
* Jenkins Automation
* GitHub Webhook Integration
* AWS Deployment
* Continuous Delivery

---

## 📸 Screenshots

### GitHub Repository

![GitHub Repository](screenshots/github-repo.png)

### Jenkins Dashboard

![Jenkins Dashboard](screenshots/jenkins-dashboard.png)

### Successful Jenkins Build

![Jenkins Build](screenshots/jenkins-success.png)

### Webhook Configuration

![Webhook](screenshots/webhook.png)

### Running Website

![Website](screenshots/website.png)

### Docker Container Running

![Docker](screenshots/docker-ps.png)

---

## 🧪 Verification Commands

Check running containers:

```bash
docker ps
```

Check Jenkins status:

```bash
sudo systemctl status jenkins
```

Check website response:

```bash
curl localhost
```

---

## 🎯 Conclusion

This project demonstrates a complete CI/CD workflow using GitHub, Jenkins, Docker, and AWS EC2.

By integrating GitHub Webhooks with Jenkins, deployments become automated, reducing manual effort and enabling continuous delivery practices.
