# Dockerized Node.js Express Application

Production-ready containerization of a Node.js Express application using Docker best practices.

This repository demonstrates how to package, run, and distribute a Node.js application as a clean, reliable Docker image suitable for real-world deployments.

---

## 🚀 What This Project Demonstrates

This project focuses on **practical, production-grade Docker skills**, including:

- Use of official **Node.js Alpine** base images
- Clean and optimized Dockerfile layering
- Proper dependency caching using `package.json`
- Reduced image size via npm cache cleanup
- Correct process management using **tini** (PID 1)
- Predictable and safe container startup
- Host-to-container port mapping
- Reproducible builds and runs across environments

---

## 🧱 Technology Stack

- Node.js (Express)
- Docker
- Alpine Linux
- tini (process manager)

---

## 📦 Docker Image

The Docker image is publicly available on Docker Hub:

👉 https://hub.docker.com/r/salioudjalo/node-app

---

## 🔧 Build the Image Locally

Clone the repository and build the image:

```bash
docker build -t salioudjalo/node-app:latest .
docker container run -p 80:3000 salioudjalo/node-app:latest
http://localhost
