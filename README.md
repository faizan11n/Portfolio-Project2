# Portfolio Website (Dockerized)

My personal DevOps portfolio: about me, skills, projects and contact, served by nginx in a Docker container.
The page also shows live numbers (public repos, followers) fetched from the GitHub API in the browser.

## Run
```bash
docker compose up -d --build
```
Open `http://<host>:8101`.

## Files
```
index.html           single-page site, no frameworks or build step
nginx.conf           gzip and basic security headers
Dockerfile           nginx:alpine + healthcheck
docker-compose.yaml  runs it on port 8101
```

## Before you publish
Replace the LinkedIn and email placeholders in the Contact section of `index.html`.

## Roadmap
- [x] Phase 1: static site in a container
- [ ] Phase 2: CI/CD with Jenkins (push, build, deploy)
- [ ] Phase 3: Kubernetes Deployment, Service and Ingress
- [ ] Phase 4: domain and HTTPS
