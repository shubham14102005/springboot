# springboot
# 🏋️‍♂️ Fitness Tracker API

A Spring Boot REST API for tracking users, workouts, meals, goals, and roles. Designed for use in health & fitness tracking applications.

---

## 🚀 Features

- User registration & management
- Workout logging (type, duration, calories)
- Meal tracking (name, calories, date)
- Goal setting per user
- Role-based access control (Admin, Manager, User)
- Spring Security (HTTP Basic Auth)
- MySQL database integration with JPA

---

## 🛠️ Tech Stack

- Java 17+
- Spring Boot
- Spring Data JPA
- Spring Security
- MySQL
- Maven

---

## 🔐 Authentication

This project uses **HTTP Basic Authentication**.  
Roles are defined in the database (admin, manager, user) and control access to different endpoints.

---

## 📦 API Endpoints

| Method | Endpoint | Access |
|--------|----------|--------|
| GET    | `/api/users`       | user, manager, admin |
| POST   | `/api/goals`       | manager, admin |
| GET    | `/api/roles`       | manager, admin |
| PUT    | `/api/users/{id}`  | admin only |
| DELETE | `/api/meals/{id}`  | admin only |
... and more!

> Access is controlled using `@PreAuthorize` and Spring Security configurations.

---

## 🧑‍💻 Setup Instructions

### ✅ Prerequisites

- Java 17+
- Maven
- MySQL

### ⚙️ Clone and Run

```bash
git clone https://github.com/shubham14102005/springboot.git
cd springboot
