📝 kube-todo-app
A minimal TODO web application deployed on Kubernetes using Deployment and Service configuration. Perfect for beginners learning Kubernetes + Docker + React deployment.

🧰 Tech Stack
🐳 Docker

⚙️ Kubernetes

⚛️ React (via Vite)

🚀 How to Deploy & Run This App on Kubernetes
🔁 1. Clone the Repository
bash
Copy
Edit
git clone https://github.com/your-username/kube-todo-app.git
cd kube-todo-app
📦 2. Apply Kubernetes Deployment & Service
bash
Copy
Edit
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
This will:

Create a pod with your TODO app container.

Expose it using a Kubernetes Service.

🌐 3. Port Forward to Access the App in Browser
bash
Copy
Edit
kubectl port-forward --address=0.0.0.0 service/my-service 5173:80
Now open your browser and visit:

cpp
Copy
Edit
http://<your-EC2-public-IP>:5173
(Replace <your-EC2-public-IP> with your actual EC2 IP address)

📁 File Breakdown
File	Description
deployment.yaml	Defines the Kubernetes Deployment for the TODO app pod
service.yaml	Exposes the app via a Kubernetes Service (default: ClusterIP)
