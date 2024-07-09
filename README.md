# Full Stack FastAPI Project


Welcome to the Full-Stack FastAPI and React template repository. This repository is a demo application for interns, showcasing how to set up and run a full-stack application with a FastAPI backend and a ReactJS frontend using ChakraUI.

A web application with a backend written in Python using FastAPI, PostgreSQL as the database, and Adminer for database management. The frontend is built with React. The project is containerized using Docker, and Docker Compose is used to set up the complete application. Nginx Proxy Manager is used for reverse proxy and SSL certificate generation.

## Project Structure

The repository is organized into two main directories:

- **frontend**: Contains the ReactJS application.
- **backend**: Contains the FastAPI application and PostgreSQL database integration.

Each directory has its own README file with detailed instructions specific to that part of the application.

## Getting Started

To get started with this template, please follow the instructions in the respective directories:

- [Frontend README](./frontend/README.md)
- [Backend README](./backend/README.md)

## Table of Contents

- Features
- Prerequisites
- Setup and Installation
- Usage
- API Documentation
- Frontend
- Database Management
- Reverse Proxy & SSL

## Features

- Frontend page of FAST API
- Creation of a Database Automatically with data
- API Documentation page
- Database Management with Adminer
- Reversed Proxy with Nginx

## Prerequisites

- Docker
- Docker-compose

## Setup and Installation

1. Clone the repository:

        git clone https://github.com/harfoh/stage-dev-2.git
        cd stage-dev-2
2. Build and start the Docker containers:

        docker-compose up --build

3. Access the application:

  - Frontend: `http://localhost`
  - Backend: `http://localhost:8000`
  - Adminer: `http://localhost:8080`
  - Nginx Proxy Manager: `http://localhost:81` (default login is `admin@example.com / changeme`)        

## Usage

### Running the application

To start the application, simply run:

        docker-compose up

### Stopping the application

To stop the application, run:

        docker-compose down

## API Documentation

The API documentation is available via Chakra UI at `http://localhost:8000/docs`.

## Frontend

The frontend is a React application. The Nginx container serves it. You can access it at `http://localhost`.

## Database Management

Adminer is used for database management and can be accessed at `http://localhost:8080`. Use the following credentials to log in:

  - System: PostgreSQL
  - Server: db
  - Username: `PostgreSQL_db_username`
  - Password: `PostgreSQL_db_password`
  - Database: `PostgreSQL_database_name`  

## Reverse Proxy & SSL

Nginx Proxy Manager is used for reverse proxy and SSL certificate generation. Access it at `http://localhost:8`1 with the default credentials (`admin@example.com / changeme`). Configure your **`domains`** and SSL **`certificates`** through the Nginx Proxy Manager interface.

