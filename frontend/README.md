# Login Application (React + Node.js)

## Project Overview

This project is a simple **Full-Stack Login Application** built using **React for the frontend** and **Node.js with Express for the backend**.
The application allows a user to log in using a username and password, validates the credentials using a backend API, and redirects the user to a welcome page upon successful authentication.

---

## Features

* Login page with **username and password fields**
* **Backend API** for validating credentials
* Redirect to **Welcome page** after successful login
* Display **error message** for incorrect credentials
* **Username remembered** using localStorage for subsequent logins
* Uses **proper HTTP status codes**

---

## Tech Stack

Frontend:

* React
* React Router
* Axios

Backend:

* Node.js
* Express
* CORS
* Body Parser

---

## Project Structure

login-app
│
├── backend
│   ├── server.js
│
└── frontend
├── src
│   ├── App.js
│   ├── Login.js
│   ├── Welcome.js
│   └── index.js

---

## Installation & Setup

### 1. Clone the Repository

git clone https://github.com/Laharivanaja/login-app.git

cd login-app

---

### 2. Setup Backend

cd backend

npm install

Run the server:

node server.js

Backend runs on:

http://localhost:5000

---

### 3. Setup Frontend

Open a new terminal:

cd frontend

npm install

Start React app:

npm start

Frontend runs on:

http://localhost:3000

---

## Login Credentials

Username: admin
Password: admin

---

## API Endpoint

POST /login

Request Body:

{
"username": "admin",
"password": "admin"
}

Response:

Success:

Status: 200

{
"message": "Login successful"
}

Failure:

Status: 401

{
"message": "Invalid credentials"
}

---

## Application Flow

User enters username and password on the login page.

React sends a POST request to the backend `/login` API.

The backend validates the credentials.

If valid → user is redirected to the Welcome page.

If invalid → an error message is displayed.

---

## Improvements (Future Enhancements)

* Password hashing using **bcrypt**
* **JWT authentication**
* Database integration (MongoDB)
* HTTPS security
* Rate limiting for login attempts

---

## Author

Lahari Prasanna
