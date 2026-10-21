# Task 20 – MERN Application Deployment on AWS EKS

## Introduction

In this task, I deployed a MERN e-commerce application on AWS using Kubernetes, Terraform, Helm, and ArgoCD.

The main goal was to deploy the application on the cloud and manage it through GitHub.

## Tools Used

- AWS
- Terraform
- Kubernetes (EKS)
- Docker
- Helm
- ArgoCD
- GitHub
- MongoDB

## Steps I Followed

### Step 1: Created an EKS Cluster

First, I used Terraform to create an EKS cluster on AWS.

After creating the cluster, I checked that the worker nodes were ready.

### Step 2: Deployed the Application

Next, I used Helm to deploy the MERN application on Kubernetes.

The application included a frontend, backend, and MongoDB database.

### Step 3: Set Up MongoDB Storage

I configured persistent storage for MongoDB so that the database could store application data.

### Step 4: Configured ArgoCD

I installed ArgoCD and connected it to my GitHub repository.

ArgoCD helped me manage the application and automatically apply changes from GitHub.

### Step 5: Tested Auto-Sync

I changed the number of frontend replicas from 3 to 4 in GitHub.

ArgoCD detected the change and updated the application automatically.

### Step 6: Checked the Application

Finally, I checked the Kubernetes pods, services, and ArgoCD status.

I also opened the e-commerce frontend in the browser to verify that it was accessible.

## Results

- Successfully created the AWS EKS cluster.
- Deployed the MERN application using Helm.
- Configured MongoDB persistent storage.
- Connected GitHub with ArgoCD.
- Successfully tested automatic synchronization.
- Accessed the frontend application in the browser.

## Screenshots

### 1. Terraform Deployment
![Terraform Deployment](screenshots/terraform-completed.png)

### 2. EKS Nodes and Pods
![EKS Nodes](screenshots/eks-nodes-pods.png)

### 3. ArgoCD Installation
![ArgoCD Installation](screenshots/argocd-installation.png)

### 4. ArgoCD Healthy and Synced
![ArgoCD Status](screenshots/argocd-healthy-synced.png)

### 5. Kubernetes Resources
![Kubernetes Resources](screenshots/kubernetes-resources.png)

### 6. MongoDB Storage
![MongoDB Storage](screenshots/mongodb-storage.png)

### 7. Frontend Replicas
![Frontend Replicas](screenshots/frontend-replicas.png)

### 8. ArgoCD Auto-Sync
![ArgoCD Auto-Sync](screenshots/argocd-auto-sync.png)

### 9. Frontend Application
![Frontend Application](screenshots/frontend-running.png)

## Conclusion

In this task, I learned how to deploy an application on AWS EKS using Terraform, Helm, and ArgoCD.

I also learned how GitHub and ArgoCD work together to automatically update an application.

This task helped me improve my practical DevOps skills.
