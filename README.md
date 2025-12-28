# 🚀 Task Management System – AI-Powered (Flutter + Node.js + PostgreSQL)

### 📌 Internship Assessment – Hybrid Backend + Flutter App

A smart task automation system that **reads task descriptions**, **auto-classifies** them using NLP rules (category, priority, assigned person, dates), and provides **action suggestions**.
Includes **Task CRUD**, **Audit History**, **Soft Delete**, **Stats Dashboard**, and **Flutter Frontend UI**.

---

## 🧩 Project Overview

| Component      | Tech Used                      | Description                                                         |
| -------------- | ------------------------------ | ------------------------------------------------------------------- |
| **Frontend**   | Flutter (Riverpod + REST API)  | Create, view, edit, delete tasks & use AI-assisted classification   |
| **Backend**    | Node.js + Express + PostgreSQL | REST API, validation, classification logic, soft delete, audit logs |
| **Database**   | PostgreSQL + JSONB             | Relational + JSON based extracted entities & suggestions            |
| **Deployment** | Render.com                     | Live production deployment                                          |

---

## 🧠 Key Features

✔ Auto AI-classification of tasks (category, priority, actions, suggested actions, dates, assigned user)
✔ CRUD Operations (Create, Update, Soft Delete, Restore)
✔ Audit Logging / Task History
✔ Stats API → Pending, Completed, Deleted Count
✔ Clean DB connection pooling (production-safe)
✔ Fully tested classification logic (Jest)
✔ Flutter responsive UI

---

## 📂 Repository Structure

```
/ (root)
 ├── backend/              # Node.js + PostgreSQL API
 │   ├── src/
 │   ├── tests/
 │   ├── package.json
 │   └── README.md         # Backend detailed README
 │
 ├── frontend/             # Flutter Mobile App
 │   ├── lib/
 │   ├── pubspec.yaml
 │   └── README.md         # Frontend detailed README
 │
 └── README.md             # <- THIS FILE (root overview)
```

---

## 🚦 Quick Start – Run Both Apps

### 🔧 1️⃣ Clone Repo

```bash
git clone https://github.com/abhishek-navicon/task-management.git
cd task-management
```

### 🖥 2️⃣ Backend Setup

```bash
cd backend
npm install
cp .env.example .env      # add DB credentials
npm start
```

### 📱 3️⃣ Flutter App Setup

```bash
cd ../frontend/smart_task_app
flutter pub get
flutter run
```

---

## 🌍 Live Demo Links

| Environment      | URL                                                                                                                                                                      |
| ---------------- | ------------------------------------------------------------------------------------------------------------------------------------------------------------------------ |
| 🟢 Backend (API) | [https://task-management-navicon-infraprojects-2.onrender.com/api/v1/tasks](https://task-management-navicon-infraprojects-2.onrender.com/api/v1/tasks)                   |
| 🟢 Classify API  | [https://task-management-navicon-infraprojects-2.onrender.com/api/v1/tasks/classify](https://task-management-navicon-infraprojects-2.onrender.com/api/v1/tasks/classify) |
| 🟢 Frontend APK  | *(Provide link if deployed / APK uploaded)*                                                                                                                              |

⚠️ Backend on free Render may sleep → first request may take 20-30s.

---

## 🧪 API Quick Test Examples

```http
POST /api/v1/tasks/classify
{
  "title": "Backup database",
  "description": "Fix login bug and assign technician now"
}

GET  /api/v1/tasks
PATCH /api/v1/tasks/:id
DELETE /api/v1/tasks/:id
GET  /api/v1/tasks/:id
GET  /api/v1/tasks/stats
```

---

## 🧱 System Architecture

```
Flutter UI  →  REST API  → PostgreSQL
                    ↓
              Classification Engine
                (regex + NLP-rules)
```

---

## 🧑‍💻 Author

**Abhishek Barik**
Computer Engineering – DYPTC
💼 GitHub: *[update your link](https://github.com/Tracebycode)*
📧 Email: *abhishekbarik974@gmail.com*

---


