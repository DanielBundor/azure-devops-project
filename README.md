# azure-devops-project

# Node.js Application Dockerized

This is a simple Node.js application Dockerized for demonstration purposes.

## Table of Contents

- [Prerequisites](#prerequisites)
- [Getting Started](#getting-started)
- [Docker Build](#docker-build)
- [Docker Run](#docker-run)
- [Application Access](#application-access)

## Prerequisites

Before you begin, ensure you have the following installed:

- [Docker](https://www.docker.com/) - The containerization platform.

## Getting Started

Clone this repository to your local machine:

```shell
git clone https://github.com/DanielBundor/nodejs-docker-app.git

cd nodejs-docker-app

```

## Docker Build

Build a Docker image for the Node.js application:


```shell
docker build -t nodejs-docker-app .

```
Replace nodejs-docker-app with your desired image name.

## Docker Run

Run a Docker container based on the image:


```shell
docker run -d -p 3000:3000 --name nodejs-app nodejs-docker-app

```
- -d: Runs the container in detached mode (in the background).
- -p 3000:3000: Maps container port 3000 to host port 3000. Modify this if your application uses a different port.
- --name nodejs-app: Assigns the name "nodejs-app" to the container.

## Application Access

Access the Node.js application in your web browser at http://localhost:3000 (or the appropriate host and port if you modified the mapping).
