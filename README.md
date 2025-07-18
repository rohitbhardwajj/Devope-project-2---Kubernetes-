# kube-todo-app 📝🚀

A minimal TODO web app deployed on Kubernetes using a Deployment and Service configuration.

## 🧱 Tech Stack
- Kubernetes
- Docker
- Vite + React (frontend)
- Node.js (optional backend)

---

## 🚀 How to Run This Project on Kubernetes

### 1. Clone the Repository
```bash
git clone https://github.com/your-username/kube-todo-app.git
cd kube-todo-app
2. Apply Kubernetes Deployment & Service
bash
Copy
Edit
kubectl apply -f deployment.yaml
kubectl apply -f service.yaml
3. Port Forward to Access the App
bash
Copy
Edit
kubectl port-forward --address=0.0.0.0 service/my-service 5173:80
Now open: http://<EC2-PUBLIC-IP>:5173 in your browser

📁 Files Explained
deployment.yaml: Deploys the app as a pod with labels and container image

service.yaml: Exposes the pod via a Kubernetes Service (ClusterIP by default)
