<!-- 
# Simple Node.js Todo App with CI/CD on Minikube

## Run Locally

```bash
docker build -t todo-app:latest .
minikube start
kubectl apply -f k8s/
minikube service todo-app-service
```

## API Endpoints

- `GET /todos` - List todos
- `POST /todos` - Add todo (JSON)
- `DELETE /todos/:id` - Delete todo -->

# 🧩 Super Todo App – DevOps Edition (Kubernetes + CI/CD)

A stylish, full-featured Todo App built with **Node.js + HTML/CSS** and deployed using **Docker & Kubernetes (Minikube)** with **GitHub Actions CI/CD** pipeline support.

![screenshot](./C:\Users\amirt\Downloads\todo-app-k8s-with-frontend\todo-app\app\public\Screenshot 2025-07-10 224602.png) <!-- Add this file manually if needed -->


---

## 🚀 Features

- ✅ Add/Delete todos with real-time UI updates
- 🔘 Mark tasks as complete/incomplete (checkboxes)
- 📊 Live progress tracking bar
- 💅 Clean, modern HTML/CSS UI
- 🐳 Dockerized backend + frontend
- ☸️ Deployed on Kubernetes (via Minikube)
- ⚙️ CI/CD pipeline with GitHub Actions (optional)
- 🔒 Ready for Trivy vulnerability scanning

---

## 🧰 Tech Stack

| Layer            | Tech                      |
|------------------|---------------------------|
| Frontend         | HTML, CSS, JavaScript     |
| Backend          | Node.js + Express         |
| Containerization | Docker                    |
| Orchestration    | Kubernetes (Minikube)     |
| CI/CD            | GitHub Actions            |


---

## 🛠️ Setup & Run Locally (Minikube)

```bash
# Start minikube
minikube start

# Connect local shell to Minikube's Docker
& minikube -p minikube docker-env | Invoke-Expression

# Build the Docker image
docker build -t todo-app:latest .

# Deploy to Kubernetes
kubectl apply -f k8s/

# Access in browser
minikube service todo-app-service
