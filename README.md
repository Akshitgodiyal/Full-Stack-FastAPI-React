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

### Frontend
Load `localhost` in your browser to access the frontend.
<img width="1680" alt="Screenshot 2024-07-09 at 20 51 46" src="https://github.com/FavourDaniel/containerization-hng/assets/89241109/9e8477ea-9574-481a-8ad9-59e648f9498e">

To login:
| Value | Credential |
|----------|----------|
| Email | devops@hng.tech |
| Password | devops#HNG11  |

<img width="1196" alt="Screenshot 2024-07-08 at 20 04 52" src="https://github.com/FavourDaniel/containerization-hng/assets/89241109/1ecfb7b7-40ed-4d0c-9573-98012eb59f50">

### Backend
Load `localhost/api` in your browser to access the backend.
<img width="1196" alt="Screenshot 2024-07-08 at 20 14 57" src="https://github.com/FavourDaniel/containerization-hng/assets/89241109/a633aa16-d3c7-4174-a08a-66296889373d">

### Backend Docs
Load `localhost/docs` in your browser to access the backend docs.
<img width="1196" alt="Screenshot 2024-07-08 at 20 04 30" src="https://github.com/FavourDaniel/containerization-hng/assets/89241109/18a8b680-dd28-4009-ba56-b076f24146a8">

### Backend Redoc
Load `localhost/redoc` in your browser to access the backend redoc.
<img width="1196" alt="Screenshot 2024-07-08 at 20 04 37" src="https://github.com/FavourDaniel/containerization-hng/assets/89241109/c127015e-524d-41b4-9df7-e916ebcd22b4">


### Adminer
Load `db.localhost` or `localhost:8080` in your browser to access Adminer.
<img width="1196" alt="Screenshot 2024-07-08 at 19 59 52" src="https://github.com/FavourDaniel/containerization-hng/assets/89241109/36b54ad5-7a1e-4fd1-95bf-830529ee1c03">
<img width="1196" alt="Screenshot 2024-07-08 at 20 18 29" src="https://github.com/FavourDaniel/containerization-hng/assets/89241109/6c71b1c7-7820-4ff8-8d93-eec85739af39">

The login creds are:
| Value | Credential |
|----------|----------|
| System | PostgreSQL |
| Server | db   |
| Username | app   |
| Password | password   |
| Database | app   |

### Proxy Manager GUI

Load `proxy.localhost` or `localhost:8090` in your browser to access Nginx Proxy Manager GUI.
<img width="1196" alt="Screenshot 2024-07-08 at 20 04 04" src="https://github.com/FavourDaniel/containerization-hng/assets/89241109/83abdf29-a785-4ece-baec-5a5377176135">
<img width="1196" alt="Screenshot 2024-07-08 at 20 03 51" src="https://github.com/FavourDaniel/containerization-hng/assets/89241109/a8e89846-95df-4d6b-bbf3-4aa8a15fafd2">


The default login creds for Nginx Proxy Manager are:
| Value | Credential |
|----------|----------|
| Email | admin@example.com |
| Password | changeme |


## License

This project is licensed under the MIT License - see the [LICENSE](./LICENSE) file for details.
