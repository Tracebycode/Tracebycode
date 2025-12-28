# 📱 Smart Task Manager — Flutter App

A productivity application to create, classify, edit, manage and track tasks — built as part of the Navicon InfraProjects Full-Stack Assessment.

This app connects to a backend (Node.js + PostgreSQL) to provide real-time task management with categories, priority levels, assignment, due dates, auto-classification, and change history.

---

## 🧑‍💻 Features

| Feature                                    | Status |
| ------------------------------------------ | ------ |
| Create / Edit / Delete Tasks               | ✅      |
| Auto-classification using backend ML logic | ✅      |
| Task history tracking (update timeline)    | ✅      |
| Offline indicator (network monitoring)     | ✅      |
| Filtering by Category, Priority, Status    | ✅      |
| Sort by Due Date / Priority                | ✅      |
| Search tasks                               | ✅      |
| Pull-to-refresh                            | ✅      |
| Error handling & snackbars                 | ✅      |

---

## 🛠️ Tech Stack

| Layer    | Technology                                                                |
| -------- | ------------------------------------------------------------------------- |
| Frontend | Flutter (Dart), Riverpod (State Management), Dio (Networking), Material 3 |
| Backend  | Node.js, Express.js                                                       |
| Database | PostgreSQL                                                                |
| Hosting  | Render (Backend), Flutter – locally                                       |

---

## 🧰 Folder Structure

```
lib/
 ├─ app/
 │   ├─ app.dart
 │   ├─ router.dart
 │   └─ bootstrap.dart
 ├─ core/
 │   ├─ constants/api_endpoints.dart
 │   ├─ network/dio_client.dart
 │   └─ utils/offline_banner.dart
 ├─ data/
 │   ├─ datasources/remote/task_api.dart
 │   ├─ models/task_model.dart
 │   └─ repositories/task_repository.dart
 ├─ state/
 │   ├─ controllers/task_controller.dart
 │   ├─ providers/*.dart
 ├─ ui/
 │   ├─ screens/dashboard/dashboard_screen.dart
 │   ├─ screens/create_task/create_task_sheet.dart
 │   └─ widgets/
 └─ main.dart

```

---

## 🚀 How to Run — Flutter App

### 1️⃣ Install Dependencies

```bash
flutter pub get
```

### 2️⃣ Update API URL

Edit `lib/data/datasources/task_api.dart`

```dart
static const baseUrl = "https://task-management-navicon-infraprojects-2.onrender.com/api/v1";
```

### 3️⃣ Run App

```bash
flutter run
```

---

## 🧪 API Reference (Backend Summary)

| Method   | Endpoint     | Description               |
| -------- | ------------ | ------------------------- |
| `POST`   | `/tasks`     | Create task               |
| `GET`    | `/tasks`     | List tasks                |
| `GET`    | `/tasks/:id` | Fetch full task + history |
| `PATCH`  | `/tasks/:id` | Update task               |
| `DELETE` | `/tasks/:id` | Soft delete               |


---

## 🖼 Screenshots

| Dashboard    | Create Task                                     | Edit Sheet                                    |
|--------------|-------------------------------------------------|-----------------------------------------------|
| ![dash](../screenshots/create_tasksheet.jpeg) | ![create](../screenshots/create_tasksheet.jpeg) | ![edit](../screenshots/Update_Tasksheet.jpeg) |


---

## 🧠 Architecture Decisions

### Why Riverpod?

* More predictable state flow → AsyncNotifier fits CRUD APIs best
* Auto UI refresh on API events
* Cleaner code compared to Provider / Bloc for small apps

### Why Dio?

* Interceptors
* Error handling
* Better logging

### Offline Design

* We **only show indicator** → disable actions in offline mode
* ❌ No auto offline syncing (not required per assessment)

---

## ⏭️ What I’d Improve If Given More Time

| Possible Next Improvements                          |
| --------------------------------------------------- |
| Dark mode toggle                                    |
| Optimistic UI update (delete instantly, sync later) |
| Local storage (SQLite) for offline task caching     |
| Push notifications / reminders                      |

---




