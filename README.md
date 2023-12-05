
# Two-Tier Application Deployment with Kubernetes on AWS EKS


This repository contains the code and configurations for deploying a two-tier application using Flask, MySQL, Docker image, and Kubernetes on Amazon EKS (Elastic Kubernetes Service).


![thumbnail](https://s3.ap-northeast-1.amazonaws.com/motulaal.io/projectsimages/architecture.png)


## Overview

The project involves deployment of two-tier application where a Flask web application serves as the backend and interacts with a MySQL database for storing user messages. The deployment is achieved using Docker containers managed by Kubernetes on AWS EKS.

# Repository Content
- **Template** directory contain HTML file for frontend rendering of Web application.

- **app.py** is a python program which handle the backend of the web application in Flask framework.

- **Docker file** is the file that contain sequence of command to develop an environment for our application to run including coping our App and template file in it.

- **EKS manifest files** is the repository that conatin all the manifest file to create a deployment and services.
- **message_table.sql** is an optional file used to create a table in the Mysql database system.
- **docker-compose.yml** is also another optional file, if we want to run the whole deployment locally.


# Situation

Two-teir application needs to be deployed efficiently in a Container for it's high availability and High scalability.

# Task

- Package the whole application in Docker file with it's dependencies and libraries.

- Make this application publicly accessible so that it can be accessed from anywhere.

- Recquire a Database to store messages from the user.

- Create a scalable architecture, which compatible with any environment for running our application concistently.

# Action

- Create a Docker image out of the DOcker file and deploy it on the AWS ECS repository.

- Create an EC2 instance for controling the AWS EKS from there and managing all the deployment and service management from that EC2 instance.

- Install AWS CLI, kubeclt, eksctl in it, and configure the AWS credentials in that instance.
- Created an AWS EKS cluster, and run the manifest file in it.
- We can also use helm Package to do this task more swiftly.

# Result

- Our Application was up and running using AWS EKS cluster.

- THe database is also running properly and storing user fetched messages.

- So much error and bugs to debug.

- Lots of learning and room for improvement.

# Contributors
Your Name @Manish-mech
