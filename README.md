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

- **frontend**: Contains the ReactJS application. Handles user interface and client-side logic
- **backend**: Handles server-side logic, APIs, and database interactions.
- **Database (Postgres)**: Stores persistent data.
- **Admin Tools (PGAdmin, Adminer)**: Provides tools to manage the database.
- **Proxy Manager (NGINX)**: Manages HTTP/HTTPS traffic and routing.

Each directory has its own README file with detailed instructions specific to that part of the application.

## Getting Started

To get started with this template, please follow the instructions in the respective directories:

- [Frontend README](./frontend/README.md)
- [Backend README](./backend/README.md)

### Prerequisites

Before you begin, ensure you have the following installed:

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)
- Python

## Tools
- FastAPI with Uvicorn - Get and Post Data
- SQLAlchemy + Alembic - used to interact with an SQL database in the background and migrate data to DB respectively.
- PostgreSQL + PGAdmin - Postgres Database and web based visual to use the database.
- Nginx Proxy Manager - Server Management Application
- Docker / Docker compose - Setup individual containers.
- Environment variables

## Installation of required tools
To install required tool, navigate to both `frontend` and `backend` folders then run: <br />
`pip install -r requirements.txt`

## Steps
Create virtual environment: <br />
`virtualenv env` or `python -m venv myvenv`

Activate the virtual environment `myvenv` <br />
`source env/bin/activate` or `source myvenv/Scripts/activate`

When done, deactivate the environment: <br />
`deactivate`

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
Frontend - `http://localhost:5173/login`
Nginx Proxy Manager - `http://localhost:8090/login`
Adminer - `http://localhost:8082/adminer`
Redoc - `http://localhost:8000/redoc`
Docs - `http://localhost:8000/docs`
```

### Stop the application
To stop the application, run:
```sh
docker-compose down --remove-orphans
```

## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
