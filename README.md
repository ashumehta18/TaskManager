# Team Task Manager (MERN Stack)

A full-stack, collaborative Team Task Manager web application built to help teams organize projects and track tasks efficiently. This repository features a cleanly decoupled architecture separating the React frontend and the Express/Node.js backend.

---

## 🚀 Features

* **Secure Authentication:** User onboarding via registration and login secured with JWT (JSON Web Tokens) and password hashing (`bcrypt`).
* **Persistent Sessions:** Seamless user sessions using browser `localStorage` and centralized API handling.
* **Role-Based Access Control (RBAC):** Middleware-enforced permissions for different user tiers (e.g., Admin, Manager, Member).
* **Complete CRUD Operations:** Full control over managing team projects and individual task tracking.
* **Relational Data Modeling:** Structured MongoDB database design connecting users, projects, and tasks.

---

## 🛠️ Tech Stack

### Frontend
* **React:** For building a dynamic, single-page user interface.
* **Axios:** Configured with global interceptors to automatically attach JWT authorization headers to outgoing API requests.

### Backend & Database
* **Node.js & Express:** Clean, modularized backend handling routing, controllers, and custom middleware.
* **MongoDB & Mongoose:** NoSQL database with strict schemas to maintain data integrity.
* **JWT & Bcrypt:** Industry-standard tools for authorization and secure password hashing.

---

## 📂 Code Architecture

The repository is divided into two primary directories to maintain a clear separation of concerns:

```text
├── client/          # React Frontend application
│   └── src/
│       └── pages/   # Login, Register, and main Dashboard
└── server/          # Node.js / Express Backend API
    ├── models/      # MongoDB Mongoose Schemas (User, Project, Task)
    ├── controllers/ # Business logic handlers
    ├── routes/      # REST API Endpoints
    └── middleware/  # Authentication & Role-based guardrails
