# 📝 kube-todo-app

A **minimal TODO web application** deployed on **Kubernetes** using **Deployment** and **Service** configuration.  
Perfect for beginners learning Kubernetes, Docker, and React deployment.

---

## 🧰 Tech Stack

- 🐳 Docker  
- ⚙️ Kubernetes  
- ⚛️ React (Vite)

---

## 🚀 How to Deploy & Run This App on Kubernetes


```bash
git clone https://github.com/your-username/kube-todo-app.git
cd kube-todo-app



📦 2. Apply Kubernetes Deployment & Service


kubectl apply -f deployment.yaml
kubectl apply -f service.yaml



🌐 3. Port Forward to Access the App


kubectl port-forward --address=0.0.0.0 service/my-service 5173:80
Then open in your browser:


http://<EC2-PUBLIC-IP>:5173
Replace <EC2-PUBLIC-IP> with your actual EC2 instance's public IP.




