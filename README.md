# ✅ TaskMan: Modern Task Management System

A robust MERN stack application to streamline personal and team task management, featuring user authentication, task categorization, and a modern, responsive UI.

---

## 📝 Overview

TaskMan is designed for individuals and teams to manage tasks efficiently. It supports user authentication, task filtering (all, important, completed, incompleted), and a clean, mobile-friendly interface. Built with security and productivity in mind.

---

## 🚀 Features

| Feature                  | Description                                      |
|-------------------------|--------------------------------------------------|
| User Authentication     | Secure JWT-based login and signup                |
| Task CRUD               | Create, update, delete, and view tasks           |
| Task Categorization     | Mark tasks as important or completed             |
| Filtering               | View all, important, completed, or incompleted   |
| Responsive UI           | Mobile-friendly, modern design                   |
| Fast API                | Express.js backend with MongoDB                  |
| State Management        | Redux for authentication state                   |
| Secure Passwords        | Passwords hashed with bcrypt                     |

---

## ⚙️ Tech Stack

**Frontend:**
- React.js (with Redux)
- Tailwind CSS (utility-first styling)
- React Router (SPA routing)
- Axios (API requests)

**Backend:**
- Node.js (runtime)
- Express.js (REST API framework)
- MongoDB (NoSQL database)
- Mongoose (ODM for MongoDB)
- JWT (authentication)
- bcryptjs (password hashing)
- CORS

---

## 🛠️ Installation

```bash
git clone https://github.com/yourusername/TaskMan.git
cd TaskMan

# Backend
cd backend
npm install

# Frontend
cd ../frontend
npm install
```

---

## 🌐 Environment Variables

### Backend (`backend/.env`)
```env
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret
```

---

## 📂 Folder Structure

```
TaskMan/
│
├── README.md
├── .gitignore
│
├── backend/
│   ├── app.js
│   ├── conn/
│   ├── models/
│   ├── routes/
│   ├── package.json
│   └── ...
│
├── frontend/
    ├── package.json
    ├── public/
    ├── src/
    │   ├── App.js
    │   ├── components/
    │   ├── pages/
    │   └── store/
    └── ...
```

---

## 📮 API Routes

| Method | Endpoint                      | Description                    |
|--------|-------------------------------|--------------------------------|
| POST   | `/api/v1/sign-in`             | Register a new user            |
| POST   | `/api/v1/log-in`              | User login                     |
| POST   | `/api/v2/create-task`         | Create a new task              |
| GET    | `/api/v2/get-all-tasks`       | Get all tasks for user         |
| DELETE | `/api/v2/delete-task/:id`     | Delete a task                  |
| PUT    | `/api/v2/update-task/:id`     | Update a task                  |
| PUT    | `/api/v2/update-imp-task/:id` | Toggle important status        |
| PUT    | `/api/v2/update-comp-task/:id`| Toggle completed status        |
| GET    | `/api/v2/get-imp-tasks`       | Get important tasks            |
| GET    | `/api/v2/get-comp-tasks`      | Get completed tasks            |
| GET    | `/api/v2/get-incomp-tasks`    | Get incompleted tasks          |

---

## 👤 Author

**Kush Varshney**  
B.Tech CSE | Full Stack Developer  
[Portfolio](https://kushvarshney.vercel.app/) • [GitHub](https://github.com/Kush-Varshney) • [LinkedIn](https://www.linkedin.com/in/kush-varshney-490baa250/)

---

## 📄 License

MIT License

---

## 🛡️ Production Readiness
- All debug logging has been removed from the backend for production.
- Error details are not exposed to clients; only generic error messages are returned for security.
- Passwords are securely hashed and JWT secrets are stored in environment variables.

---

