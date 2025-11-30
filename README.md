# ✅ Full-Stack TODO App (Spring Boot + HTML/JS)

A simple and clean full-stack TODO application built with:

🟦 **Backend:** Spring Boot (Java 21), H2 Database
🟩 **Frontend:** HTML + CSS + JavaScript (no framework)
🐳 **Deployment:** Dockerfile (works with Render / Railway / any Docker host)

This project demonstrates:

* REST API development with Spring Boot
* Full CRUD operations (Create, Read, Update, Delete)
* H2 embedded database
* Frontend communicating with backend using `fetch()`
* CORS-enabled backend for external FE hosting
* Production-ready Docker deployment

---

## 📂 Project Structure

```
todo-fullstack_2025/
│
├── src/
│   ├── main/
│   │   ├── java/com/example/todobackend/
│   │   │   ├── TodoBackendApplication.java
│   │   │   ├── controller/TodoController.java
│   │   │   ├── model/Todo.java
│   │   │   ├── repository/TodoRepository.java
│   │   └── resources/
│   │       ├── application.properties
│   │       └── static/
│   │           └── index.html   ← Frontend UI
│
├── pom.xml
├── Dockerfile
└── README.md
```

---

## 🚀 Features

### Backend (Spring Boot)

* ✔ REST API under `/api/todos`
* ✔ Create a todo
* ✔ Get all todos
* ✔ Mark as done / undone
* ✔ Delete a todo
* ✔ Automatic timestamps
* ✔ H2 database (file mode)
* ✔ CORS enabled for any frontend

### Frontend (index.html)

* ✔ Beautiful responsive UI
* ✔ Fetches all todos from backend
* ✔ Add new todos
* ✔ Mark / Unmark
* ✔ Delete instantly
* ✔ Works locally or through Docker deployment

---

## ▶️ Running Locally

### 1️⃣ Start Backend (IntelliJ)

Run the Spring Boot app:

```
TodoBackendApplication
```

Backend will be available at:

```
http://localhost:8080
```

### 2️⃣ Open the Frontend

Open in browser:

```
http://localhost:8080/index.html
```

Or if using VS Code:

```
Live Server → http://127.0.0.1:5500/index.html
```

---

## 🐳 Docker Deployment (Render / Railway / Local)

This project includes a **production-ready Dockerfile**.

### Build image:

```
docker build -t todo-app .
```

Run container:

```
docker run -p 8080:8080 todo-app
```

Backend will be available at:

```
http://localhost:8080
```

---

## 🌐 Deploy on Render (Free)

1. Upload your project to GitHub
2. In Render → **New Web Service**
3. Choose:

   * **Environment:** Docker
   * **Root Directory:** *leave blank*
   * **Dockerfile path:** `Dockerfile`
4. Deploy

Render will automatically:

* Build the Docker image
* Run your Spring Boot jar
* Expose public URL

Your app will be online globally.

---

## 🛠 Tech Stack

| Layer      | Technology             |
| ---------- | ---------------------- |
| Backend    | Spring Boot 4, Java 21 |
| Database   | H2 (file mode)         |
| Frontend   | HTML5, CSS3, JS        |
| Build Tool | Maven                  |
| Hosting    | Docker (Render)        |

---

## 📌 API Endpoints

| Method | Endpoint          | Description    |
| ------ | ----------------- | -------------- |
| GET    | `/api/todos`      | List all todos |
| POST   | `/api/todos`      | Create todo    |
| PUT    | `/api/todos/{id}` | Toggle done    |
| DELETE | `/api/todos/{id}` | Delete todo    |

Example create request:

```json
{
  "title": "Buy milk",
  "description": "2 litres"
}
```

---

## 🎯 Why This Project?

Perfect for learning:

* Backend development with Java
* REST APIs
* Connecting FE + BE
* H2 DB & JPA
* Full-stack architecture
* Docker deployment for real hosting

---

## 🏁 Future Improvements

* User authentication
* Categories & tags
* Dark/light themes
* Deploy frontend on Netlify
* Mobile app version

---

## 👨‍💻 Author

**Prajwal H C**
Full-Stack Developer (Java + Python)
Passionate about clean software & real-world projects.
