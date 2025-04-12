#  Kubernetes Game App using NodePort

This project demonstrates a simple Kubernetes deployment using Minikube.  
It runs a "Game of Life" app exposed via a NodePort service.

##  Features

- Kubernetes Deployment with ReplicaSet
- NodePort Service to expose the app externally
- Easily accessible on Minikube

##  Files

- `deployment.yaml` - defines the pod and container
- `service.yaml` - exposes the app on a NodePort
- `README.md` - documentation

## 🛠️ Steps to Run

```bash
minikube start
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
minikube service game-service
