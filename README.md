# 📇 CRM Web App (MERN Stack)

A full-stack **Customer Relationship Management (CRM)** web application built using the **MERN stack** — MongoDB, Express.js, React.js, and Node.js — with a clean frontend architecture and a **basic DevOps setup** for containerization and automation.

This project is designed to simulate how real-world CRM systems are structured, developed, and deployed.

---

## 💡 What I Learned

* How full-stack CRM systems are designed and built in real-world scenarios
* Importance of **Figma-based UI planning** before development
* Scalable **React architecture** using features, layouts, and reusable components
* Handling **authentication, routing, API calls, and modular backend logic**
* Writing clean, maintainable code with proper **folder structure and naming conventions**
* Basics of DevOps tools like **Docker, Docker Compose, Jenkins, and Kubernetes**

> This project taught me not just how to code, but **how to think like a full-stack developer with DevOps awareness**.

---

## 🚀 What This App Does

This CRM application allows businesses to:

* 📥 Register and log in users
* 👤 Manage customers, leads, and contacts
* 📝 Track queries, tickets, or service issues
* 🔐 Secure routes using authentication
* 📊 Interact with a clean, modern user interface

The goal is to **simulate a professional CRM system** similar to those used by real organizations.

---

## 🛠 Tech Stack

### Frontend

* React.js (Vite)
* React Router DOM
* Axios
* Tailwind CSS (or other CSS frameworks depending on branch)

### Backend

* Node.js
* Express.js
* MongoDB with Mongoose
* JSON Web Tokens (JWT)
* CORS, dotenv, and standard middlewares

### Design

* Figma UI prototypes (see `/prototype and files`)

---

## 🔧 DevOps Setup (Basic)

This project includes a **basic DevOps workflow** to demonstrate core concepts such as containerization, service orchestration, CI automation, and container deployment.

### 🐳 Docker

* Docker is used to containerize both the **backend (Node.js + Express)** and **frontend (React + Vite)** applications.
* Separate `Dockerfile`s are created for frontend and backend to ensure consistent environments across systems.
* This helps eliminate “works on my machine” issues.

### 🧩 Docker Compose

* Docker Compose is used to run frontend and backend services together with a single command.
* The `docker-compose.yml` file builds and starts both services, simplifying local development.

```bash
docker-compose up --build
```

---

### 🔁 Jenkins (CI)

* A basic Jenkins pipeline is defined using a `Jenkinsfile`.
* The pipeline automates:

  * Pulling source code from GitHub
  * Installing frontend and backend dependencies
  * Building Docker images
* This demonstrates a foundational **Continuous Integration (CI)** workflow.

---

### ☸️ Kubernetes

* A basic Kubernetes `Deployment` file is included.
* It deploys the backend container into a Kubernetes-managed pod.
* Kubernetes ensures the application restarts automatically if the container crashes.

> This setup focuses on **learning fundamentals**, not advanced production configurations.

---

## 📁 Folder Structure

```
crm-web-app/
├── prototype and files/              # UI design files (Figma, assets)
├── client-api/                       # Node.js + Express backend
│   ├── src/
│   │   ├── helper/
│   │   ├── middleware/
│   │   ├── model/
│   │   ├── router/
│   │   └── utils/
│   ├── app.js
│   ├── Dockerfile
│   └── readme.md
├── frontend/                         # React frontend
│   ├── src/
│   │   ├── api/
│   │   ├── app/
│   │   ├── assets/
│   │   ├── components/
│   │   ├── features/
│   │   ├── layout/
│   │   ├── pages/
│   │   ├── app.css
│   │   ├── app.jsx
│   │   └── main.jsx
│   ├── Dockerfile
│   └── index.html
├── k8s/
│   └── deployment.yaml               # Basic Kubernetes deployment
├── docker-compose.yml
├── Jenkinsfile
├── .dockerignore
└── README.md
```

---

## 🧪 How to Run Locally (Without Docker)

### 1. Clone the Repository

```bash
git clone https://github.com/hemantsinghdev/crm-system
cd crm-web-app
```

### 2. Backend Setup

```bash
cd client-api
npm install
npm run dev
```

Create a `.env` file:

```env
PORT=5000
MONGO_URI=your_mongo_connection_string
JWT_SECRET=your_jwt_secret_key
```

### 3. Frontend Setup

```bash
cd ../frontend
npm install
npm run dev
```

* Frontend: `http://localhost:5173`
* Backend: `http://localhost:5000`

---

## 🎯 Project Focus

* Full-stack MERN development
* Clean frontend and backend architecture
* Introductory DevOps practices
* Resume-ready and interview-friendly project
