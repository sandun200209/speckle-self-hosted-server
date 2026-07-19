# 🚀 Self-Hosted Speckle Server with Docker

![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![Docker Compose](https://img.shields.io/badge/Docker_Compose-2496ED?style=for-the-badge&logo=docker&logoColor=white)
![PostgreSQL](https://img.shields.io/badge/PostgreSQL-316192?style=for-the-badge&logo=postgresql&logoColor=white)
![Redis](https://img.shields.io/badge/Redis-DD0031?style=for-the-badge&logo=redis&logoColor=white)
![MinIO](https://img.shields.io/badge/MinIO-C72E49?style=for-the-badge)
![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)

## 📖 Overview

This project demonstrates the deployment of a production-style self-hosted Speckle Server using Docker Compose.

The infrastructure integrates PostgreSQL, Redis, MinIO Object Storage, and Nginx Reverse Proxy to provide a scalable BIM collaboration platform.

---

# ✨ Features

- Self-hosted Speckle Server
- Docker Compose Deployment
- PostgreSQL Database
- Redis Cache
- MinIO Object Storage
- Nginx Reverse Proxy
- Persistent Storage
- Environment Configuration
- Easy Deployment
- Production-ready Architecture

---

# 🏗 Architecture

![Architecture](docs/architecture.png)

---

# 🛠 Technology Stack

- Docker
- Docker Compose
- PostgreSQL
- Redis
- MinIO
- Nginx
- Linux
- Git
- GitHub

---

# 📷 Screenshots

## Login Page

![Login](docs/login-page.png)

---

## Running Containers

![Docker](docs/docker-containers.png)

---

## Deployment

![Deployment](docs/deployment.png)

---

# 🚀 Getting Started

Clone Repository

```bash
git clone https://github.com/USERNAME/speckle-self-hosted-deployment.git
```

Move into Project

```bash
cd speckle-self-hosted-deployment
```

Start Services

```bash
docker compose -f docker-compose-deps.yml up -d

docker compose -f docker-compose-speckle.yml up -d
```

---

# 📁 Services

| Service | Description |
|----------|-------------|
| PostgreSQL | Database |
| Redis | Cache |
| MinIO | Object Storage |
| Speckle Server | Main Application |
| Nginx | Reverse Proxy |

---

# 📚 Skills Demonstrated

- Docker
- Docker Compose
- Container Networking
- Reverse Proxy
- Infrastructure Deployment
- DevOps
- Linux
- Git Version Control

---

# 📄 License

MIT License


## 🏗 Architecture

```mermaid
graph TD

A[User / Browser]
B[Nginx Reverse Proxy]
C[Speckle Frontend]
D[Speckle Server]
E[PostgreSQL]
F[Redis]
G[MinIO Object Storage]

A --> B
B --> C
C --> D
D --> E
D --> F
D --> G
