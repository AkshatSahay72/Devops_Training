# Production Steps
1) Code Base 
2) Production (Version Control)
3) Containerization (Docker)
4) Storing the Container (Docker Hub)
5) Container Ochestration (Kubernetes)

# Containerization
Packaging a whole codebase to a single file

# Docker
* Learned about containerisation

* Dockerfile
```
FROM python:3.13

WORKDIR /containerization

COPY requirements.txt .
RUN pip install --no-cache-dir -r requirements.txt

COPY . .

CMD ["python", "app.py"]
```

* For Building
```
docker build -t test:v1 .
```