# tdd-drfproject
---

# Python Django Microservice Project

## Overview

This project demonstrates how to set up a development environment using Docker to build and deploy a microservice powered by Python, Django, and Django REST Framework. Emphasizing the practices of Test-Driven Development (TDD), it includes a RESTful API developed with `pytest` to ensure that all code meets functionality requirements through rigorous testing before deployment.

## Technologies Used

- **Python**: The core programming language used for backend development.
- **Django**: A high-level Python web framework that encourages rapid development and clean, pragmatic design.
- **Django REST Framework**: A powerful and flexible toolkit for building Web APIs with Django.
- **Docker**: A set of platform-as-a-service (PaaS) products that use OS-level virtualization to deliver software in packages called containers.
- **pytest**: A framework that makes it easy to write simple tests, yet scales to support complex functional testing.
- **GitHub Actions**: Used for Continuous Integration/Continuous Deployment (CI/CD) workflows to automate testing and deployment processes.

## Project Goals

The goal of this project is to:
- Demonstrate the setup of a Docker-based development environment for a Python Django project.
- Apply Test-Driven Development (TDD) practices to build a reliable and maintainable RESTful API.
- Showcase the integration of continuous testing and deployment workflows using GitHub Actions.

## Getting Started

### Prerequisites

Ensure you have Docker installed on your machine. Docker will be used to containerize the application and its dependencies for a consistent development environment.

### Setup and Running the Project

1. **Clone the repository:**

```sh
git clone <repository-url>
cd <project-directory>
```

2. **Build the Docker Containers:**

Navigate to the project directory and run:

```sh
docker-compose build
```

3. **Start the Containers:**

```sh
docker-compose up -d
```

4. **Run Migrations:**

```sh
docker-compose exec web python manage.py migrate
```

5. **Running Tests:**

Ensure your application works correctly by running:

```sh
docker-compose exec web pytest
```
