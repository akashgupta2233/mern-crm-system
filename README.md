# 📇 CRM Web App (MERN Stack + Figma Design)

A complete full-stack CRM (Customer Relationship Management) web application built using the **MERN stack** — MongoDB, Express.js, React.js, Node.js — with a modern frontend architecture and **Figma-based UI design**.

> I followed a full tutorial by [@DentedCode](https://www.youtube.com/@DentedCode), writing all the code myself with minimal changes. Through this project, I explored how real-world full-stack applications are designed, developed, and structured.

---

## 💡 What I Learned

- How full-stack CRM systems are built in the real world
- Importance of **Figma design** and UI planning before development
- Advanced **React architecture** using features, layouts, and components
- How to handle **authentication, routing, API calls, and modularization**
- The discipline of **code organization**, scalable folder structures, and naming conventions
- Basic business logic flow in CRM systems

> This project taught me more than just coding — it taught me **how to think like a developer**.

---

## 🚀 What This App Does

This CRM app allows businesses to:

- 📥 Register and log in
- 👤 Manage customers, leads, and contacts
- 📝 Track queries, tickets, or service issues
- 🔐 Authenticate and secure routes
- 📊 Use a modern and clean interface

The goal is to **simulate a professional CRM system**, like those used by real businesses for managing interactions and services.

---

## 🛠 Tech Stack

### Frontend:
- React.js (Vite)
- React Router DOM
- Axios
- Tailwind CSS (or other CSS frameworks depending on branch)

### Backend:
- Express.js
- MongoDB (with Mongoose)
- JSON Web Tokens for authentication
- CORS, dotenv, and other middlewares

### Design:
- Figma prototypes (see `/prototype and files`)

---

## 📁 Folder Structure
```
crm-web-app/
├── prototype and files/              # UI Design files (Figma, assets)
├── client-api/                      # Node + Express backend
│   ├── src/
│   │   ├── helper/
│   │   ├── middleware/
│   │   ├── model/
│   │   ├── router/
│   │   └── utils/
│   ├── app.js
│   └── readme.md
├── frontend/                        # React frontend
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
│   └── index.html
└── README.md                        # This file
```
---

## 🧪 How to Run Locally

### 1. Clone the Repository

```bash
git clone https://github.com/hemantsinghdev/crm-system
cd crm-web-app
````

### 2. Backend Setup

```bash
cd client-api
npm install
npm run dev
```

Make sure to create a `.env` file with the following:

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

Frontend will run on `http://localhost:5173`
Backend will run on `http://localhost:5000`

---


