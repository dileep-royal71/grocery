# 🛒 Grocery Web App

This is a full-stack Grocery Web Application built using **Node.js**, **Express.js**, **MongoDB**, and **JWT Authentication**. It allows users to register, login, and manage their grocery items with secure token-based authentication.

## 🚀 Features

- 🔐 User Authentication (Register/Login with JWT)
- 🧾 Add, Update, Delete Grocery Items
- 📋 View Grocery List
- 🛡️ Secure APIs using JSON Web Tokens (JWT)
- 🧩 RESTful API Design

---

## 📁 Project Structure

grocery-app/
│
├── controllers/ # Request handlers
├── models/ # Mongoose models
├── routes/ # Route definitions
├── middleware/ # Auth middleware (JWT verification)
├── config/ # Database connection
├── .env # Environment variables
├── server.js # Entry point
└── package.json # Dependencies and scripts

yaml
Copy code

---

## 🛠️ Tech Stack

- **Backend**: Node.js, Express.js
- **Database**: MongoDB with Mongoose
- **Authentication**: JWT (JSON Web Token)
- **Tools**: Postman (for testing APIs), dotenv

---

## 📦 Installation

```bash
git clone https://github.com/your-username/grocery-app.git
cd grocery-app
npm install
⚙️ Configuration
Create a .env file in the root directory and add:

env
Copy code
PORT=5000
MONGO_URI=your_mongodb_connection_string
JWT_SECRET=your_jwt_secret_key
▶️ Running the Server
bash
Copy code
npm start
Server will run on http://localhost:5000

🔑 API Endpoints
👤 Auth Routes
Method	Endpoint	Description
POST	/api/register	Register a new user
POST	/api/login	Login and get JWT

🛒 Grocery Routes (Protected)
Method	Endpoint	Description
GET	/api/groceries	Get all groceries
POST	/api/groceries	Add a grocery item
PUT	/api/groceries/:id	Update grocery item
DELETE	/api/groceries/:id	Delete grocery item

🔐 All grocery routes require a valid JWT token in the header.

✅ Sample JWT Usage
Pass the token in headers:

http
Copy code
Authorization: Bearer <your_token>
📬 Future Improvements
🖼️ Frontend with React or Vue

📱 Mobile responsive UI

🔍 Search & Filter options

📊 Dashboard with stats
