# i2i Academy - Containerization

This repository contains the solution for the i2i Academy Containerization assignment.

## Objectives
1. Understand the fundamentals of Containerization.
2. Deploy a simple static webpage using Docker and Docker Compose on a local environment.
3. Replicate the setup and deploy it on a Cloud Virtual Machine (Hostinger VPS) on port 8086.

## Theoretical Knowledge

**Question 1: What is containerization, and why do we need to containerize applications?**
**Answer: Containerization packages an application with all its dependencies into a single isolated unit, ensuring it runs consistently across any computing environment. This technology is essential to prevent environment-related bugs and to simplify the overall deployment process.**

**Question 2: What are some different containerization technologies and their trade-offs?**
**Answer: While Docker is the industry standard due to its ease of use, alternatives like Podman offer daemonless security, and LXC provides lightweight system-level virtualization.**

**Question 3: How and where is containerization highly beneficial in real-world scenarios?**
**Answer: In real-world scenarios, containerization is highly beneficial for microservices and cloud-native applications because it allows rapid scaling and independent updates. It is also crucial in CI/CD pipelines to guarantee identical environments for development, testing, and production.**

## Deployment Guide

### Local Environment Setup
To build and run the Nginx container locally:
```bash
docker compose up -d
```
Access the custom landing page at: `http://localhost:8080`

### Cloud Deployment (Hostinger VPS)
To deploy the isolated environment on the Hostinger VPS (using port 8086 to prevent conflicts with existing projects):
```bash
docker-compose up -d
```
Access the webpage globally at: `http://72.62.37.67:8086`
