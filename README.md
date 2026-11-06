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

Developer → GitHub Repository → GitHub Actions → Docker Build → DockerHub Push → AWS EC2 Deployment → Live Application

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

1. Clone the repository:

   git clone https://github.com/tehreem-tariq901/cicd-project.git

2. Navigate to the project:

   cd cicd-project

3. Build the Docker image:

   docker build -t cicd-app .

4. Run the container:

   docker run -d --name cicd-app -p 5000:5000 cicd-app

5. Open the application:

   http://localhost:5000

## AWS Deployment Status

The application was deployed and tested on AWS EC2.

The EC2 instance is stopped when not in use to avoid unnecessary AWS compute costs. Therefore, the application is not continuously accessible.

---

## Screenshots

Project screenshots are available inside the `screenshots` folder.

---

## Learning Outcomes

During this project, I learned:

* Infrastructure as Code (Terraform)
* Containerization using Docker
* CI/CD automation using GitHub Actions
* Cloud deployment on AWS EC2
* Troubleshooting real-world deployment issues

