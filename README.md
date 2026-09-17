# 🎓 Course Management System

A full-stack **Course Management System** built with React, Node.js, Express, and PostgreSQL.

The project provides a web interface where users can register and log in, browse available courses, and access individual course pages. The backend provides REST API endpoints for authentication, courses, categories, and database operations.

## ✨ Features

- 🔐 **User Registration**
  - Create a new account with name, email, and password.
  - Input validation for user details.
  - Passwords are securely hashed using bcrypt.

- 🔑 **User Login**
  - Authenticate users using email and password.
  - JWT-based authentication support.

- 📚 **Course Management**
  - Display available courses.
  - View individual course pages.
  - Course information includes title, description, and enrollment details.

- 🗂️ **Category Management**
  - Backend support for creating course categories.

- 🗄️ **PostgreSQL Database**
  - Database integration using PostgreSQL.
  - Structured models for users, courses, categories, and subscriptions.

- 🌐 **REST API**
  - Express.js backend with organized API routes and controllers.

- ⚛️ **React Frontend**
  - Component-based user interface.
  - Client-side navigation using React Router.

## 🛠️ Technologies Used

### Frontend

- **React.js**
- **React Router DOM**
- **Axios**
- **JavaScript (ES6+)**
- **CSS**

### Backend

- **Node.js**
- **Express.js**
- **JWT**
- **bcrypt**
- **CORS**
- **dotenv**

### Database

- **PostgreSQL**
- **pg**
- SQL

## 📂 Project Structure

```text
CMS-Project/
│
├── client/
│   ├── public/
│   └── src/
│       ├── assets/
│       ├── AdvancedJavaScript.jsx
│       ├── App.jsx
│       ├── Courses.jsx
│       ├── Home.jsx
│       ├── Login.jsx
│       ├── Register.jsx
│       ├── ReactBasics.jsx
│       ├── NodeJsBackend.jsx
│       ├── index.css
│       ├── styles.css
│       └── main.jsx
│
├── server/
│   ├── src/
│   │   ├── controllers/
│   │   │   ├── auth.controller.js
│   │   │   ├── category.controller.js
│   │   │   ├── course.controller.js
│   │   │   └── subscription.controller.js
│   │   │
│   │   ├── db/
│   │   │   └── index.js
│   │   │
│   │   ├── models/
│   │   │   ├── category.model.js
│   │   │   ├── course.model.js
│   │   │   ├── subscription.model.js
│   │   │   └── user.model.js
│   │   │
│   │   ├── routes/
│   │   │   ├── auth.routes.js
│   │   │   ├── category.routes.js
│   │   │   ├── course.routes.js
│   │   │   └── subscription.routes.js
│   │   │
│   │   ├── utils/
│   │   │   └── validators.js
│   │   │
│   │   ├── app.js
│   │   ├── consatns.js
│   │   └── server.js
│   │
│   ├── package.json
│   ├── query.sql
│   └── patterns.cpp
│
└── README.md
```

## 🚀 Getting Started

### Prerequisites

Make sure you have the following installed:

- [Node.js](https://nodejs.org/)
- npm
- PostgreSQL

### 1. Clone the Repository

```bash
git clone <your-repository-url>
cd CMS-Project
```

### 2. Set Up the Backend

Navigate to the server directory:

```bash
cd server
```

Install dependencies:

```bash
npm install
```

Create a `.env` file inside the `server` directory:

```env
PORT=3000
DATABASE_URL=your_postgresql_connection_string
JWT_SECERT=your_jwt_secret
```

Replace the values with your PostgreSQL connection details and a secure JWT secret.

Start the backend:

```bash
npm start
```

The server will run on:

```text
http://localhost:3000
```

### 3. Set Up the Frontend

Open a new terminal and navigate to the client directory:

```bash
cd client
```

Install dependencies:

```bash
npm install
```

Start the React development server:

```bash
npm run dev
```

The frontend will then be available at the local URL provided by Vite.

## 🔌 API Routes

The backend follows a REST-style API structure.

### Authentication

```text
POST /api/v1/auth/register
POST /api/v1/auth/login
```

### Courses

```text
/api/v1/course
```

### Categories

```text
/api/v1/category
```

The API communicates with the PostgreSQL database through the backend models and controllers.

## 🔄 Application Flow

```text
User
 │
 ▼
React Frontend
 │
 │ Axios HTTP Requests
 ▼
Express.js API
 │
 ├── Authentication
 ├── Courses
 ├── Categories
 └── Subscriptions
 │
 ▼
PostgreSQL Database
```

## 🔐 Authentication

The authentication system includes:

- User registration
- Email validation
- Name validation
- Password validation
- Password hashing using bcrypt
- Login credential verification
- JWT token generation

Environment variables are used for sensitive configuration such as the database connection and JWT secret.

## 📚 Available Courses

The frontend currently includes course pages for:

- **React Basics**
- **Advanced JavaScript**
- **Node.js Backend**

Each course can be selected from the course listing and opened through React Router.

## 🗃️ Database

The application uses **PostgreSQL** as its relational database.

The backend contains models for:

- Users
- Courses
- Categories
- Subscriptions

SQL queries and database-related files are located in the `server` directory.

## 🧪 Testing

The backend currently does not contain an automated test suite.

The `package.json` test script is currently configured as a placeholder.

## 🚧 Future Improvements

Some possible improvements for future versions include:

- Implement persistent course enrollment
- Complete subscription functionality
- Add role-based access control
- Add an admin dashboard
- Allow administrators to create, update, and delete courses
- Add course search and filtering
- Improve authentication token handling
- Add protected routes
- Add automated backend and frontend tests
- Improve responsive UI and accessibility
- Add persistent user sessions

## 👨‍💻 Author

**Francis**

A full-stack academic project developed to practice:

- React development
- REST API development
- Node.js and Express
- PostgreSQL database integration
- Authentication
- CRUD-oriented backend architecture
- Client-server communication

---

⭐ **Course Management System**  
Built with React, Node.js, Express, and PostgreSQL.