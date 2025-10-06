# Monitoring-Stack-Prometheus-Grafana-on-EC2-

## Project Description
Monitor EC2 instance metrics using Prometheus and visualize them using Grafana dashboards.

## Features
- Prometheus metrics collection  
- Grafana dashboards  
- Dockerized setup for easy deployment  

## Prerequisites
- AWS EC2 instance (Ubuntu 22.04)  
- Docker & Docker Compose installed  
- Git & GitHub account  
- Security group ports: 22, 9090, 3000  

## Installation Commands
Install Docker & Docker Compose:
```
sudo apt update
sudo apt install -y docker.io docker-compose
sudo systemctl start docker
sudo systemctl enable docker
```
## Launch stack:
- docker-compose up -d
- Connectivity Commands

## Access Prometheus:
http://<EC2_PUBLIC_IP>:9090

## Access Grafana:
- http://<EC2_PUBLIC_IP>:3000
- Login: admin/admin

## How to Run / Access
- Add Prometheus as data source in Grafana
- Create dashboards for CPU, memory, and system metrics

## Next Steps / Improvements
- Monitor multiple EC2 instances
- Add alerting via Alertmanager
- Use Terraform/Ansible for automated deployment
