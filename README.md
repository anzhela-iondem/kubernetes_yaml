# Kubernetes YAML Configurations

This repository contains YAML configuration files for deploying applications using Kubernetes. The configurations include deployment setups for development and production environments as well as a sample secrets file.

## Files Included

- **dev_app.yaml**: Configuration for deploying the application in the development environment.
- **prod_app.yaml**: Configuration for deploying the application in the production environment.
- **secrets.sample**: A sample file for Kubernetes secrets. Rename to `secrets.yaml` and populate with your secret data.

## Getting Started

### Prerequisites

Ensure you have the following installed:
- [Kubernetes](https://kubernetes.io/docs/tasks/tools/)
- [kubectl](https://kubernetes.io/docs/tasks/tools/install-kubectl/)

### Deployment

1. **Secrets.sample**
   Add needed credentials in the "secrets.sample" file, rename it to "secrets.yaml and run it. 
   ```bash
   kubectl apply -f secrets.yaml

2. **Development Environment**
   ```bash
   kubectl apply -f dev_app.yaml

3. **Production Environment**
   ```bash
   kubectl apply -f prod_app.yaml
