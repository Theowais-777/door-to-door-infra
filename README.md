# Door-to-Door Infrastructure Repository

This repository maintains all configuration, containerization, reverse proxying, and deployment definitions for the Door-to-Door Kashmir platform.

## Architecture

- **`docker/docker-compose.yml`**: Multi-container orchestration (Redis + FastAPI Backend + Nginx Gateway)
- **`nginx/nginx.conf`**: Nginx edge reverse proxy routing `/api/` to backend and `/` to frontend
- **`k8s/`**: Kubernetes production manifests
- **`.env`**: Centralized environment secrets and runtime configuration
