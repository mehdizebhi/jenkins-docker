# Jenkins Docker

A customized **Jenkins** version with **Docker CLI** and **kubectl** support, containerized for easy deployment.

## Features ✨
- **Based on Jenkins 2.492.1 with JDK 17**
- **Includes Docker CLI** for running containers within Jenkins
- **Includes kubectl** for managing Kubernetes clusters from Jenkins
- **Pre-installed essential plugins**:
  - [Blue Ocean](https://plugins.jenkins.io/blueocean/)
  - [Docker Workflow](https://plugins.jenkins.io/docker-workflow/)

## Usage 🚀
1. Clone the repository:
   ```sh
   git clone https://github.com/mehdizebhi/jenkins-docker.git
   cd jenkins-docker
   ```
2. Build the Docker image:
   ```sh
   docker build -t custom-jenkins .
   ```
3. Run the Jenkins container:
   ```sh
   docker run -d -p 8080:8080 -p 50000:50000 --name jenkins custom-jenkins
   ```
4. Access Jenkins at **http://localhost:8080** and log in.

## Prerequisites 🛠️
- **Docker** must be installed on your system. [Download Docker](https://docs.docker.com/get-docker/)