#  Wanderlust - Airbnb Clone

##  Project Overview

Wanderlust is a full-stack Airbnb clone web application where users can explore listings, create their own stays. The project demonstrates complete backend development along with containerization and Kubernetes deployment.

---

##  Tech Stack

* **Frontend:** HTML, CSS, JavaScript, EJS
* **Backend:** Node.js, Express.js
* **Database:** MongoDB
* **Authentication:** Passport.js
* **Containerization:** Docker
* **Orchestration:** Kubernetes (Minikube)
* **Ingress:** NGINX Ingress Controller

---

##  Features

*  User Authentication (Login/Register)
*  Create, Read, Update, Delete Listings
*  Reviews & Ratings
*  Session Management with MongoDB
*  RESTful APIs
*  Dockerized Application
*  Kubernetes Deployment
*  Ingress Routing (Custom Domain: airbnb.local)

---

##  Project Structure

```
airnb/
│── controllers/
│── models/
│── routes/
│── views/
│── public/
│── utils/
│── k8s/
│   ├── backend.yaml
│   ├── mongodb.yaml
│   ├── ingress.yaml
│── Dockerfile
│── package.json
│── app.js
```

---

##  Setup Instructions

### 1️ Clone Repository

```
git clone https://github.com/aryaautade/backend-airnb.git
cd airnb
```

---

### 2️ Install Dependencies

```
npm install
```

---

### 3️ Run Locally

```
node app.js
```

App runs on:

```
http://localhost:8080
```

---

##  Docker Setup

### Build Image

```
docker build -t aryaautade13/backend-airnb .
```

### Run Container

```
docker run -p 8080:8080 aryaautade13/backend-airnb
```

---

##  Kubernetes Deployment

### Apply Configurations

```
kubectl apply -f k8s/
```

### Check Pods

```
kubectl get pods
```

### Access Service

```
minikube service backend-service
```

---

##  Ingress Setup

### Enable Ingress

```
minikube addons enable ingress
```

### Add Hosts Entry (Windows)

Path:

```
C:\Windows\System32\drivers\etc\hosts
```

Add:

```
127.0.0.1 airbnb.local
```

### Access App

```
http://airbnb.local
```

---

##  Future Improvements

*  Deploy on Cloud (AWS/GCP)
*  HTTPS with SSL
*  CI/CD Pipeline (GitHub Actions)
*  Improved UI/UX



