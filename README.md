# Kubernetes Application Developer Project

## Project Overview

This project is designed to help me study for the Certified Kubernetes Application Developer (CKAD) certification. It includes deploying two applications with different deployment strategies and various Kubernetes features.

## Requirements

### Application 1: Canary Deployment Strategy | PSQL - Shared Storage

14. **PostgreSQL Deployment**
    - Create a Deployment for PostgreSQL.
    - Configure Persistent Volumes (PVs), Persistent Volume Claims (PVCs), and StorageClasses for storage.

1. **Develop a Dockerfile for the App**
   - Create a Dockerfile to containerize your application.

2. **Deploy the Application**
   - Override the entrypoint and arguments in the Deployment manifest.
   - Include an InitContainer and a sidecar container in the Deployment manifest.

4. **Inject Environment Variables**
   - Use ConfigMaps to inject non-sensitive environment variables.
   - Use Secrets to inject sensitive environment variables.

5. **Inject Configuration Files**
   - Use ConfigMaps for configuration files.
   - Use Secrets for sensitive configuration files.


6. **Configure the App to Assume a Service Account**
   - Create and bind a Service Account to the Deployment.
   - That Service Account will have permission to call the API Server.

7. **Set Resource Requests and Limits**
   - Define CPU and memory requests and limits for the containers.

8. **Manage Pod Scheduling**
   - Use NodeSelectors, Node affinities, and tolerations for pod scheduling.

9. **Configure Readiness and Liveness Probes**
   - Define readiness and liveness probes to monitor the application's health.

10. **Create a CronJob**
    - Create a CronJob to perform periodic tasks related to the application.

11. **Add Annotations and Labels**
    - Add annotations and labels to the pods for better organization and management.

12. **Configure Canary Deployment Strategy**
    - Implement a canary deployment strategy using Kubernetes Deployment and Services.

13. **Expose the App to the Internet**
    - Create an Ingress resource to expose the application.
    - Use a valid DNS domain to access the application.


### Application 2: Blue-Green Deployment Strategy

1. **Develop a Dockerfile for the App**
   - Create a Dockerfile to containerize your application (e.g., Node.js or Python).

2. **Override Entrypoint and Arguments**
   - Override the entrypoint and arguments in the Deployment manifest.

3. **Create a Deployment Manifest for a Multicontainer App**
   - Include an InitContainer and a sidecar container in the Deployment manifest.

4. **Inject Environment Variables**
   - Use ConfigMaps to inject non-sensitive environment variables.
   - Use Secrets to inject sensitive environment variables.

5. **Inject Configuration Files**
   - Use ConfigMaps for configuration files.
   - Use Secrets for sensitive configuration files.

6. **Configure the App to Assume a Service Account**
   - Create and bind a Service Account to the Deployment.

7. **Set Resource Requests and Limits**
   - Define CPU and memory requests and limits for the containers.

8. **Manage Pod Scheduling**
   - Use NodeSelectors, Node affinities, and tolerations for pod scheduling.

9. **Configure Readiness and Liveness Probes**
   - Define readiness and liveness probes to monitor the application's health.

10. **Create a CronJob**
    - Create a CronJob to perform periodic tasks related to the application.

11. **Add Annotations and Labels**
    - Add annotations and labels to the pods for better organization and management.

12. **Configure Blue-Green Deployment Strategy**
    - Implement a blue-green deployment strategy using Kubernetes Deployment and Services.

13. **Expose the App to the Internet**
    - Create an Ingress resource to expose the application.
    - Use a valid DNS domain to access the application.

14. **PostgreSQL StatefulSet Deployment**
    - Create a StatefulSet for PostgreSQL.
    - Configure Persistent Volumes (PVs), Persistent Volume Claims (PVCs), and StorageClasses for storage.

## Extra Work

1. **Configure Network Policies**
   - Define NetworkPolicies to control traffic flow to and from the application pods.

2. **Configure RBAC**
   - Implement Role-Based Access Control (RBAC) policies to manage access to Kubernetes resources.

