# Capstone Project: CI/CD Pipeline with Jenkins, Docker, GitHub, and AWS EC2

## Project Overview

This project demonstrates a complete CI/CD (Continuous Integration and Continuous Deployment) pipeline using GitHub, Jenkins, Docker, and AWS EC2.

The application is a static website hosted inside an Nginx Docker container. Jenkins automatically builds and deploys the application on an AWS EC2 instance.

---

## Technologies Used

* GitHub
* Jenkins
* Docker
* AWS EC2
* Nginx
* Amazon Linux 2023

---

## Project Architecture

Developer → GitHub → Jenkins → Docker → AWS EC2 → Website

---

## Project Files

* `index.html` – Website source code
* `Dockerfile` – Creates Docker image using Nginx
* `Jenkinsfile` – CI/CD pipeline configuration
* `README.md` – Project documentation

---

## Dockerfile

The Dockerfile creates an Nginx-based Docker image and copies the website files into the Nginx web directory.

---

## CI/CD Pipeline Stages

### 1. Clone Repository

Jenkins clones the latest code from the GitHub repository.

### 2. Build Docker Image

Jenkins builds a Docker image using the Dockerfile.

### 3. Deploy Container

Jenkins stops the old container (if running), removes it, and deploys the latest version.

---

## Features

* Automated deployment using Jenkins
* Docker containerization
* Cloud hosting on AWS EC2
* Version control with GitHub
* Reusable CI/CD pipeline

---

## Outcome

Successfully deployed a website on AWS EC2 using Docker and automated the deployment process using Jenkins Pipeline.

This project demonstrates practical DevOps concepts including Continuous Integration, Continuous Deployment, Infrastructure Management, and Containerization.
