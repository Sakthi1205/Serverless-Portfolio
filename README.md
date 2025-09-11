🚀 Containerized Portfolio Deployment

This project demonstrates how to containerize a personal portfolio website and deploy it on a local Kubernetes cluster (Minikube). It highlights containerization, orchestration, and service exposure using NodePort.

📌 Project Overview

Problem: Hosting personal projects reliably with real-world deployment practices.

Approach: Dockerized the portfolio app and deployed it on Minikube with a Kubernetes Service.

Outcome: Achieved smooth local deployment with browser access through Kubernetes NodePort service.

🛠️ Tech Stack

Docker – Containerization

Kubernetes – Orchestration

Minikube – Local Kubernetes cluster

NodePort Service – Service exposure

⚙️ Setup & Installation
1️⃣ Clone the Repository
git clone https://github.com/Sakthi1205/portfolio-k8s.git
cd portfolio-k8s

2️⃣ Build Docker Image
docker build -t sakthi-portfolio:1.0 .

3️⃣ Start Minikube
minikube start

4️⃣ Deploy to Kubernetes
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml

5️⃣ Access the Portfolio
minikube service portfolio-service


This will open your portfolio in the browser.
Or, you can manually access via:

http://<minikube-ip>:30080



🌟 Features

Dockerized portfolio application

Kubernetes Deployment & Service (NodePort)

Verified browser access using Minikube tunnel

Easily portable and cloud-ready

📂 Repository Structure

<img width="240" height="188" alt="image" src="https://github.com/user-attachments/assets/29f12953-813d-464b-8b9e-9e2f87a16d54" />


🔮 Future Enhancements

Configure Ingress with a custom domain (portfolio.local).

Deploy on AWS EKS / GKE / AKS for cloud availability.

Add CI/CD pipeline using GitHub Actions or Jenkins.

