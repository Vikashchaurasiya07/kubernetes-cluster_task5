# Kubernetes Cluster Deployment with Minikube

## Objective
In this project, we set up a local Kubernetes cluster using **Minikube** to deploy and manage an app. The goal was to deploy an app, expose it via a service, and scale it using Kubernetes commands.

## Tools Used
- **Minikube**: A tool to run Kubernetes clusters locally.
- **kubectl**: Command-line tool for interacting with Kubernetes.
- **Docker**: Used for containerizing the application.

## Steps Completed

### 1. Install Minikube and Start the Cluster
- Installed Minikube and started the Kubernetes cluster.

```bash
minikube start
```

### 2. Create Deployment YAML for the App
- Created a `deployment.yaml` file to define the app deployment.


### 3. Expose the App Using `service.yaml`
- Created a `service.yaml` file to expose the app.


### 4. Apply the YAML Files
- Applied the `deployment.yaml` and `service.yaml` to the Kubernetes cluster.

```bash
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
```
![image](https://github.com/user-attachments/assets/136ca91b-365a-46c6-99da-bdc4caf50192)

### 5. Verify Pods and Services
- Used the `kubectl get pods` and `kubectl get services` commands to verify the status of the pods and services.

```bash
kubectl get pods
kubectl get services
```
![image](https://github.com/user-attachments/assets/336edcdf-afdd-49f7-9412-7806d889fb6d)


### 6. Access the App via Minikube Service
- Accessed the app by running the following command, which creates a tunnel for the app.

```bash
minikube service inspireme-service
```
![image](https://github.com/user-attachments/assets/6847b6e1-75f4-4552-a714-fedd500b887f)

