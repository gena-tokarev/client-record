# Client Record Project Infrastructure

This repository serves as the central point for managing and running the project, which consists of the following services:

- **`app`**: [Frontend and API service](https://github.com/gena-tokarev/client-record-app).
- **`db`**: [Database service (PostgreSQL)](https://github.com/gena-tokarev/client-record-db).
- **`db2search`**: [Database replication service (Golang)](https://github.com/gena-tokarev/client-record-db2search).
- **`devops`**: [Devops infrastructure](https://github.com/gena-tokarev/client-record-devops).

The project uses `docker-compose` to manage and run all services together.

---

## Features

- **`app`**: Contains the frontend and backend logic.
- **`db`**: Provides PostgreSQL configuration and necessary database initialization scripts.
- **`db2search`**: Synchronizes the database with Elasticsearch for search functionality.
- **`devops`**: Contains devops infrastructure stuff.
- **`docker-compose`**: Easily run all services with one command.

---

## Prerequisites

Before you begin, ensure you have the following installed on your machine:

- [Docker](https://www.docker.com/get-started)
- [Docker Compose](https://docs.docker.com/compose/install/)

---

## Getting Started

1. Clone this repository along with its submodules:

   ```bash
   git clone --recurse-submodules https://github.com/gena-tokarev/client-record
   cd client-record
2. Create `.env` file and copy in it the contents of `.env.example`
3. Run `docker-compose up -d`
4. At the moment we have to run the app service manually. So please go to [app repository](https://github.com/gena-tokarev/client-record-app) and follow the instructions of how to run it (the frontend and api service).
