# ✅ Task Manager API

A secure and scalable RESTful API built with **Flask** that allows users to manage personal tasks with full **JWT authentication**. The project is designed for learning and deploying backend APIs, using **PostgreSQL**, **GitHub Actions** for CI, and **Docker** for containerized environments.

---

## 🚀 Features

- 🔐 **JWT Authentication** – Secure token-based login and registration
- 👥 **User-Specific Task Management** – Each user can only manage their own tasks
- 📋 **Full CRUD** – Create, Read, Update, and Delete tasks
- 🛡️ **Protected Routes** – Only authenticated users can access and manipulate their data
- 🧪 **Automated Testing** – With `pytest` and coverage reports via **GitHub Actions**
- 🧊 **Containerized with Docker** – Easy to run, scale, and deploy
- 📅 **Task Due Dates & Priority Levels** – Manage deadlines and prioritize work
- 🔁 **Password Reset (Coming Soon)** – Reset your password via email
- 🧑‍💻 **Frontend Integration Ready** – Compatible with React, Vue, or Flutter frontends
- 📄 **Extensible Design** – Modular structure for rapid scaling and team development

---

## 🧰 Tech Stack

- **Backend:** Flask, Flask-JWT-Extended, Flask-SQLAlchemy
- **Database:** PostgreSQL
- **Auth:** JWT (JSON Web Tokens)
- **DevOps:** GitHub Actions, Docker
- **Testing:** Pytest, Coverage
- **Tools:** Git, Postman, Docker Compose

---

## 🗂️ API Endpoints

### 🔐 Authentication
| Method | Endpoint | Description |
|--------|----------|-------------|
| POST | `/register` | Register a new user |
| POST | `/login` | Login and receive JWT access and refresh tokens |
| POST | `/refresh` | Refresh access token |
| POST | `/logout` | Log out and blacklist refresh token |

### 📋 Task Management (Requires Auth)
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | `/tasks` | Retrieve all tasks for the user |
| POST | `/tasks` | Create a new task |
| GET | `/tasks/<id>` | Retrieve a specific task |
| PUT | `/tasks/<id>` | Update a task |
| DELETE | `/tasks/<id>` | Delete a task |

---

## ⚙️ Setup Instructions

### 1. Clone the Repository

```bash
git clone https://github.com/GearshiftGamesInc/task-manager-api.git
cd task-manager-api
