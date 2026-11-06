# End-to-End CI/CD DevOps Project 🚀

## Project Overview

This project demonstrates an end-to-end CI/CD pipeline using Flask, Docker, DockerHub, GitHub Actions, Terraform, and AWS EC2.

The goal was to automate application deployment from code changes to a live application running on AWS.

---

## Technologies Used

* Linux (Ubuntu)
* Python Flask
* Docker
* DockerHub
* Git & GitHub
* GitHub Actions
* Terraform
* AWS EC2

---

## Project Workflow

### Current CI/CD Workflow

Developer → GitHub → GitHub Actions → Docker Build → DockerHub Push

### Previous AWS Deployment

Terraform → AWS EC2 Provisioning → SSH Connection → Flask Application

## Current Project Status

- GitHub Actions successfully builds and pushes the Docker image to Docker Hub.
- Terraform was used to provision AWS infrastructure.
- The Flask application was previously deployed and tested successfully on AWS EC2.
- Automatic EC2 deployment is currently disabled in the GitHub Actions workflow.
- The EC2 application is not currently maintained as a live service.


---

## Features

* Dockerized Flask application
* Infrastructure provisioning using Terraform
* Automated CI/CD pipeline using GitHub Actions
* Application deployment on AWS EC2
* Automated deployment using DockerHub

---

## Run Locally

### Prerequisites
- Git
- Docker

### Steps

**1. Clone the repository**

```bash
git clone https://github.com/tehreem-tariq901/cicd-project.git
```

**2. Navigate to the project**

```bash
cd cicd-project
```

**3. Build the Docker image**

```bash
docker build -t cicd-app .
```

**4. Run the container**

```bash
docker run -d --name cicd-app -p 5000:5000 cicd-app
```

**5. Open the application**

http://localhost:5000

---

## Screenshots


### 1. CI/CD Pipeline Execution
![CI/CD Pipeline](screenshots/CI-CD%20Pipeline%20run%20Successfully.png)

### 2. DockerHub Image Push
![DockerHub](screenshots/DockerHub%20repository%20shows%20pushed%20image.png)

### 3. Terraform Apply
![Terraform Apply](screenshots/Terraform%20apply.png)

### 4. EC2 Instance Creation
![EC2 Instance](screenshots/Instance%20created%20successfully%20using%20terraform.png)

### 5. EC2 SSH Connection
![EC2 SSH](screenshots/Ec2%20successfully%20connected%20with%20terminal%20using%20SSH.png)

### 6. Application Running on EC2
![Flask Application](screenshots/Browser%20showing%20app%20using%20EC2%20public%20IP.png)


---

## Learning Outcomes

During this project, I learned:

* Infrastructure as Code (Terraform)
* Containerization using Docker
* CI/CD automation using GitHub Actions
* Cloud deployment on AWS EC2
* Troubleshooting real-world deployment issues

