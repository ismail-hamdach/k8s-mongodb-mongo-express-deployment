## k8s-mongodb-mongo-express-deployment

This repository contains the resources and configurations to deploy MongoDB alongside mongo-express using Kubernetes. The deployment is designed to provide a scalable and easily manageable database solution with a web-based interface for managing MongoDB.

### Features

- **MongoDB Deployment**: Set up and manage MongoDB instances using Kubernetes.
- **mongo-express Integration**: Web-based MongoDB admin interface for easy database management.
- **Scalable Architecture**: Designed to scale with your application needs using Kubernetes' powerful orchestration capabilities.
- **Configuration Files**: Includes Kubernetes YAML configuration files for deploying both MongoDB and mongo-express.


### Getting Started

To get started with deploying MongoDB and mongo-express on your Kubernetes cluster, follow the steps below:

1. **Clone the Repository**:
    ```bash
    git clone https://github.com/ismail-hamdach/k8s-mongodb-mongo-express-deployment.git
    cd k8s-mongodb-mongo-express-deployment
    ```

2. **Apply Kubernetes Configurations**:
    ```bash
    kubectl apply -f mongodb-secret.yaml
    kubectl apply -f mongodb-deployment.yaml
    kubectl apply -f mongo-configmap.yaml
    kubectl apply -f mongo-express-deployment.yaml
    ```

3. **Access mongo-express**:
    - Obtain the external IP of the mongo-express service.
    - Open your web browser and navigate to `http://<EXTERNAL_IP>:<PORT>`.

### Prerequisites

- **Kubernetes Cluster**: A running Kubernetes cluster (minikube, EKS, GKE, etc.).
- **kubectl**: Kubernetes command-line tool installed and configured.

### Contributing

Contributions are welcome! Please feel free to submit issues, fork the repository, and send pull requests.

### License

This project is licensed under the MIT License.
