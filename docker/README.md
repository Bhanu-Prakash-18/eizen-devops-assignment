# Task 2 – Docker Compose with Nginx Reverse Proxy

This setup runs a Flask application locally using Docker Compose.

## Architecture
- Flask application runs in its own container
- Flask container is NOT exposed directly
- Nginx container acts as a reverse proxy
- Nginx logs all incoming requests

## Files
- Dockerfile
- docker-compose.yml
- nginx/nginx.conf

## Run locally
```bash
docker-compose up --build

