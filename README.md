
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
- `DELETE /todos/:id` - Delete todo
