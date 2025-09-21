# 🧪 DevOps Intern Assignment – Nginx Reverse Proxy with Docker  

[![Docker](https://img.shields.io/badge/Docker-2496ED?style=for-the-badge&logo=docker&logoColor=white)](https://www.docker.com/)  
[![Nginx](https://img.shields.io/badge/Nginx-009639?style=for-the-badge&logo=nginx&logoColor=white)](https://www.nginx.com/)  
[![Python](https://img.shields.io/badge/Python-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://www.python.org/)  
[![Compose](https://img.shields.io/badge/Docker--Compose-000000?style=for-the-badge&logo=docker&logoColor=white)](https://docs.docker.com/compose/)  

This project sets up a simple system with **two backend services** and an **Nginx reverse proxy** running in Docker containers.  
The reverse proxy routes traffic to the appropriate backend service, making both accessible from a single endpoint.  

---

## 📌 Requirements
- Two Dockerized backend services (dummy services are fine) running on different ports.  
- An Nginx reverse proxy container that routes traffic:  
  - `/service1` → Backend Service 1  
  - `/service2` → Backend Service 2  
- All services accessible via a single exposed port (e.g., `http://localhost:8080`).  

---

## 📂 Project Structure  

```bash
.
├── docker-compose.yml
├── nginx
│   ├── default.conf
│   └── Dockerfile
├── service_1
│   ├── app.py
│   └── Dockerfile
├── service_2
│   ├── app.py
│   └── Dockerfile
└── README.md


---

## ⚙️ How to Run

```bash
git clone https://github.com/ShivaniH20/devops-nginx-proxy.git
cd devops-nginx-proxy

docker-compose up --build

---

✅ Summary

Built two simple backend services with Docker

Configured Nginx reverse proxy for routing

Managed services with Docker Compose

Exposed everything via a single port for easy access

