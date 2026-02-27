# Docker Adminer + MySQL Project

## Overview
This project demonstrates a multi-container Docker application using Docker Compose.

Containers:
- Adminer (Web-based database management)
- MySQL (Database server)

Adminer connects to the MySQL database container over a custom Docker network.

---

## Architecture

Client (mgmt01/wks01 browser)
→ Adminer container
→ MySQL container

---

## Installation Steps

### 1. Install Docker
sudo apt update
sudo apt install docker.io docker-compose -y

### 2. Start Containers
docker compose up -d

### 3. Verify Containers
docker ps
docker network ls
docker volume ls

---

## Access Application

From a client machine browser:

http://DOCKER-VM-IP:8080

Login Credentials:
- System: MySQL
- Server: db
- Username: testuser
- Password: testpassword
- Database: testdb

---

## Features Demonstrated
- Multi-container deployment
- Custom Docker bridge network
- Persistent Docker volume
- Database creation and data insertion
- Client access from separate machine
