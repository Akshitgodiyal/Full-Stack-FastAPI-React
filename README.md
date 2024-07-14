# Full-Stack FastAPI and React

Welcome to the Full-Stack FastAPI and React template repository. This repository serves as a demo application, showcasing how to set up and run a full-stack application with a FastAPI backend and a ReactJS frontend using ChakraUI.

## Table of Contents

- [Project Structure](#project-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Setup Development with Docker](#setup-development-with-docker)
- [Accessing the Application](#accessing-the-application)
- [Stopping the Application](#stopping-the-application)
- [License](#license)

## Project Structure

The repository is organized into two main directories:

- **frontend**: Contains the ReactJS application.
- **backend**: Contains the FastAPI application and PostgreSQL database integration.

Each directory has its own README file with detailed instructions specific to that part of the application.

## Getting Started

To get started with this template, please follow the instructions in the respective directories:

- [Frontend README](./frontend/README.md)
- [Backend README](./backend/README.md)

### Prerequisites

Before you begin, ensure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### Setup Development with Docker

To set up the development environment using Docker, follow these steps:

1. **Build and start the application:**
    ```sh
    docker-compose up --build
    ```

2. **Stop the application:**
    ```sh
    docker-compose down --remove-orphans
    ```

### Accessing the Application

After starting the application, you can access the following services:
```sh
http://localhost:8080/adminer
http://localhost:8000/redoc
http://localhost:8000/docs
http://localhost:5173/login
```

### Stop the application
To stop the application, run:
```sh
docker-compose down --remove-orphans
```

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
