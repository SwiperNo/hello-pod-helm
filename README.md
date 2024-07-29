# Hello Pod Helm

This repository showcases a single-pod pattern deployment on Kubernetes. Additionally, it includes a setup for deploying Super Mario using that pattern with a service exposing a NodePort.

## Contents

- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Manual Deployment](#manual-deployment)
- [Helm Deployment](#helm-deployment)
- [Cleanup](#cleanup)
- [Directory Structure](#directory-structure)

## Overview

This repository demonstrates two deployment methods:
1. **Manual Deployment** using `kubectl apply -f`.
2. **Helm Deployment** using `init.sh` script.

The example application, Super Mario, is deployed with a NodePort service for external access.

## Prerequisites

- Kubernetes cluster (Minikube, GKE, EKS, AKS, etc.)
- `kubectl` configured to interact with your Kubernetes cluster
- Optional: Helm installed (if using Helm deployment)

## Manual Deployment

To manually deploy the application, run the following command:

```sh
kubectl apply -f deployment.yaml
