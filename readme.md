# Palworld Helm Chart

This Helm chart deploys a Palworld server on a Kubernetes cluster. Palworld is a multiplayer, open-world survival
crafting game. This chart simplifies the process of deploying and managing a Palworld server in a Kubernetes
environment.

## Prerequisites

- Kubernetes cluster
- Helm 3+

## Installation



```bash
# Clone the repository:
git clone https://github.com/bcjarrett/pal-world-k8s.git
cd pal-world-k8s

# Update values.yaml

# Install the Helm chart
helm install palworld ./k8s/palworld
```

## Configuration

The values.yaml file contains configuration options for the server. You can customize the deployment by
modifying these values. Key configurations include:

    service: Service type and port configuration - Important for realworld hosting. 
    storage: Persistent storage configuration for game data - Tested working with NFS.
    serverConfig: Game server settings as of this release.

Password and admin credentials are supported via an existing secret. Please see `values.yaml` for an example.

For detailed configuration options, refer to the `values.yaml` file.
