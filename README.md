
````md
---

## 🚀 API Endpoints

### 🏁 Base URL
| Environment | URL |
|-------------|-----|
| Local       | `http://localhost:3000/api/v1/tasks` |
| Production  | `https://task-management-navicon-infraprojects-2.onrender.com/api/v1/tasks` |

---

### 🔹 1️⃣ Classify Task (Auto NLP Classification)

**POST** `/classify`

#### Request
```json
{
  "title": "Backup Database",
  "description": "Fix login bug and assign technician now"
}
````

#### Response

```json
{
  "category": "technical",
  "priority": "low",
  "assigned_person": "unassigned",
  "actions": ["fix"],
  "suggestions": [
    "Diagnose issue",
    "Check resources",
    "Assign technician",
    "Document fix"
  ],
  "dates": []
}
```

---

### 🔹 2️⃣ Create Task

**POST** `/create`

#### Request

```json
{
  "title": "Meeting with Rahul",
  "description": "Meet Rahul tomorrow for project updates",
  "category": "scheduling",
  "priority": "low",
  "assigned_person": "Rahul",
  "due_date": "2025-12-26",
  "extracted_entities": {
    "actions": ["meet"],
    "dates": ["tomorrow"]
  }
}
```

#### Response

```json
{
  "success": true,
  "message": "Task created successfully",
  "id": "uuid-string"
}
```

---

### 🔹 3️⃣ Get All Tasks (Paginated + Filtered)

**GET** `/`

#### Query Params

| Param      | Example               | Meaning         |
| ---------- | --------------------- | --------------- |
| `page`     | `?page=1`             | pagination      |
| `limit`    | `?limit=10`           | items per page  |
| `status`   | `?status=pending`     | task status     |
| `category` | `?category=technical` | category filter |
| `priority` | `?priority=high`      | priority filter |

#### Response

```json
{
  "tasks": [...],
  "total": 23
}
```

---

### 🔹 4️⃣ Get Single Task (with Audit History)

**GET** `/:id`

Example:

```http
GET /api/v1/tasks/b87a1153-d4a6-404a-bf94-8411fd95bdea
```

Response:

```json
{
  "success": true,
  "data": {
    "id": "b87a1153-d4a6-404a-bf94-8411fd95bdea",
    "title": "Revise Documentation",
    "status": "deleted",
    "extracted_entities": {
      "dates": ["2025-01-10"],
      "actions": ["update docs", "push to repo"]
    },
    "suggested_actions": ["Review PR", "Share with team"],
    "history": [
      { "action": "created" },
      { "action": "updated" },
      { "action": "deleted" }
    ]
  }
}
```

---

### 🔹 5️⃣ Update Task

**PATCH** `/:id`

#### Request

```json
{
  "priority": "high",
  "description": "Update the API docs for task module",
  "assigned_to": "john.doe",
  "extracted_entities": {
    "actions": ["update docs","push to repo"],
    "dates": ["2025-01-10"]
  }
}
```

#### Response

```json
{
  "success": true,
  "message": "Task updated successfully",
  "data": { "id": "uuid", "status": "pending" }
}
```

---

### 🔹 6️⃣ Soft Delete Task

**DELETE** `/:id`

```http
DELETE /api/v1/tasks/f92756ba-4f77-4f9e-8965-ef45e20c0dbe
```

Response:

```json
{
  "success": true,
  "message": "Task deleted successfully"
}
```

---

### 🔹 7️⃣ Dashboard KPI Summary

**GET** `/stats`

```json
{
  "pending": "16",
  "in_progress": "1",
  "completed": "1",
  "deleted": "6",
  "total": "24"
}
```

---

## 🧠 Classification Logic (How it works)

✔ Category based on keywords
✔ Urgency → priority
✔ Regex to extract person name
✔ Verbs list → actions
✔ Suggested actions based on category

### Example:

```js
function classifyTask(text) {
  const category = detectCategory(text) || "general";
  const priority = detectPriority(text) || "low";
  const assigned_person = extractPerson(text) || "unassigned";
  const actions = extractActions(text);
  const dates = extractDates(text);
  const suggestions = suggestedActions(category);
  return { category, priority, assigned_person, actions, dates, suggestions };
}
```

---

## 🧪 Testing (Jest)

Run tests:

```bash
npm test
```

Example:

```js
test("detects urgent → high", () => {
  const result = classifyTask("urgent bug fix needed immediately");
  expect(result.priority).toBe("high");
});
```

---

## 🚀 Deployment (Render)

| Step | Action                    |
| ---- | ------------------------- |
| 1    | Push repo to GitHub       |
| 2    | Create Render Web Service |
| 3    | Build: `npm install`      |
| 4    | Start: `npm start`        |
| 5    | Add ENV `DATABASE_URL`    |

Live Backend:
👉 [https://task-management-navicon-infraprojects-2.onrender.com/](https://task-management-navicon-infraprojects-2.onrender.com/)

---

## 🧭 Architecture Decisions

| Reason                     | Choice                      |
| -------------------------- | --------------------------- |
| Predictable behavior       | Rule-based NLP              |
| Avoid accidental data loss | Soft delete + audit-history |
| Maintainability            | Controller → Service → Repo |
| Scale                      | PostgreSQL connection pool  |

---

## 🚧 Improvements Coming

* Use **AI / Transformer NER** for entity extraction
* Add **JWT-Auth** & User Roles
* Cron jobs for reminders
* WebSocket live updates

---

```

---

### 🎉 Done
Bas isko **directly README.md me paste** karo — ab formatting **100% correct render hogi** ✔

Agar chaho toh main **badges / cover screenshot / GIF demo** bhi add karke ek **full-professional GitHub README** bana du.  
Bole toh — **"Add badges & branding"**
```
