# 🚀 Multi-Service Project – Go + Python + Nginx

This project demonstrates a simple microservices setup using:

- 🐹 Go (Golang) – Service 1
- 🐍 Python Flask – Service 2
- 🌐 Nginx – Reverse Proxy

Each service runs in its own Docker container and is routed by Nginx based on path prefixes.

---

## 📦 Services Overview

| Service     | Tech     | Port  | Path Prefix   | Description                      |
|-------------|----------|-------|----------------|----------------------------------|
| `service_1` | Go       | 8001  | `/service1/`   | Returns JSON responses (ping, hello) |
| `service_2` | Python   | 8002  | `/service2/`   | Flask API with basic endpoints   |
| `nginx`     | Nginx    | 8080  | Reverse proxy | Routes requests to services      |

---

## 🔧 Endpoints

You can access the services through Nginx at:

- [http://localhost:8080/service1/ping](http://localhost:8080/service1/ping)
- [http://localhost:8080/service1/hello](http://localhost:8080/service1/hello)
- [http://localhost:8080/service2/ping](http://localhost:8080/service2/ping)
- [http://localhost:8080/service2/hello](http://localhost:8080/service2/hello)

---

## 🛠️ Run the Project

### ✅ Prerequisites

- Docker

### ▶️ Build and Start

```bash
docker-compose up --build



