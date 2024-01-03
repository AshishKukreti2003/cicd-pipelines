# CI/CD Pipeline Project

This project demonstrates a Continuous Integration and Continuous Deployment (CI/CD) pipeline for a Java application using Docker and GitHub Actions.

## Overview

The repository contains the following files:

- `main.yml`: GitHub Actions workflow to build, tag, and push a Docker image to Docker Hub on changes to the main branch.
- `Hello.java`: Simple Java application printing "Hello, Java!" when executed.
- `Dockerfile`: Instructions to build a Docker image containing the Java application.

## Workflow Description

The `main.yml` file in the `.github/workflows` directory triggers the workflow on pushes to the main branch. It performs the following actions:
- Checks out the repository.
- Logs in to Docker Hub using secrets for authentication.
- Extracts metadata for Docker, including tags and labels.
- Builds and pushes a Docker image using the `Dockerfile` and Java application files.

## Files

- `Hello.java`: Contains a basic Java program printing "Hello, Java!".
- `Dockerfile`: Describes the steps to create a Docker image with the Java application.
- `main.yml`: GitHub Actions workflow for CI/CD pipeline setup.

Feel free to explore and modify the files to suit your requirements.
