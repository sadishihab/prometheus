# Monitoring with Prometheus

## Technologies used:

- Prometheus, Kubernetes, Helm, AWS EKS, eksctl, Grafana, Linux, Redis, Node.js, Docker, Docker Hub

## Job 1: Install Prometheus Stack in Kubernetes
#### Job description:

- Setup EKS cluster using eksctl
- Deploy Prometheus, Alert Manager and Grafana in cluster as part of the Prometheus Operator using Helm chart

## Job 2: Configure Alerting for our Application
#### Job description:

Configure our Monitoring Stack to notify us whenever CPU usage > 50% or Pod cannot start
- Configure Alert Rules in Prometheus Server
- Configure Alertmanager with Email Receiver

## Job 3: Configure Monitoring for a Third-Party Application
#### Job description:

- Deploy Redis service in our cluster
- Deploy Redis exporter using Helm Chart
- Configure Alert Rules (when Redis is down or has too many connections)
- Import Grafana Dashboard for Redis to visualize monitoring data in Grafana

## Job 4: Configure Monitoring for Own Application
#### Job description:

- Configure our NodeJS application to collect & expose Metrics with Prometheus Client Library
- Deploy the NodeJS application, which has a metrics endpoint configured, into Kubernetes cluster
- Configure Prometheus to scrape this exposed metrics and visualize it in Grafana Dashboard
