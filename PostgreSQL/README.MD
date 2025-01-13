# Intro
This folder include PostgreSQL 16.6 Kubernetes files. Create ns:
```bash
kubectl create ns postgres
````
After apply all files sequencly:
```bash
kubectl apply -f postgres-secret.yaml
kubectl apply -f postgres-pvc.yaml
kubectl apply -f postgres-service.yaml
kubectl apply -f postgres-deploy.yaml
```