

# 🐳 Docker Project , Frontend + Backend + Database

This project demonstrates how to implement a simple 3-tier architecture using Docker. It includes:

* **Frontend**: A React application
* **Backend**: A Node.js/Express API
* **Database**: MongoDB

The frontend communicates with the backend, and the backend interacts with the database.

---

## 🚀 Getting Started

### Prerequisites

Ensure you have the following installed:

* Docker
* Docker Compose

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/knaopel/docker-frontend-backend-db.git
   cd docker-frontend-backend-db
   ```

2. Build and start the containers:

   ```bash
   docker-compose up --build
   ```

   This command:

   * Builds the Docker images for frontend, backend, and MongoDB
   * Starts the containers as defined in `docker-compose.yml`

---

## 🌐 Accessing the Application

Once the containers are running, you can access the application:

* Frontend: [http://localhost:3000](http://localhost:3000)
* Backend: [http://localhost:5000](http://localhost:5000)

The application is a simple todo app.

---

## 🛑 Stopping the Containers

To stop the running containers:

```bash
docker-compose down
```

This command stops and removes the containers, networks, and volumes defined in the `docker-compose.yml` file.

---

## 🧩 Project Structure

* **`frontend/`**: Contains the React application
* **`backend/`**: Contains the Node.js/Express API
* **`docker-compose.yml`**: Defines services for frontend, backend, and MongoDB

---

For more details, refer to the project's GitHub repository: [https://github.com/knaopel/docker-frontend-backend-db](https://github.com/knaopel/docker-frontend-backend-db)

---



A demonstration of Docker to implement a simple 3 tier architecture

* frontend will be able to access the mid-tier
* mid-tier will be able to access the db

In order to run this in docker, simply type ```docker-compose up``` at the command prompt. Docker will then create the [MongoDB](https://www.mongodb.com/) from the stock [mongo](https://hub.docker.com/_/mongo) image. The api uses [nodejs](https://nodejs.org/) with [express](http://expressjs.com/) and is built from a [node:alpine](https://hub.docker.com/_/node) image. The front end uses [ReactJS](https://reactjs.org/) and built from a [node:alpine](https://hub.docker.com/_/node) image .
