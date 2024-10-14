
# User Management System

## 📑 Description  
A simple user management system built with Node.js and MongoDB. It allows users to **register**, **login**, and manage their profiles securely with JWT-based authentication.

---

## 🚀 Features Implemented  
- **User Registration**: Creates a new user with a hashed password.  
- **User Login**: Issues JWT token for authentication.  
- **User Profile**: Displays user information (protected route).  
- **Authentication Middleware**: Protects private endpoints.  
- **Environment Configuration**: Uses `.env` for sensitive information.

---

## 🧪 Testing Instructions
Test the following API endpoints using Postman or any other API testing tool.
I tested This using CURL from my termilan itself.
**Some tests that I used were the following**:
- **USER Registration**: POST /api/users/register
   ```bash
    curl -X POST http://localhost:5000/api/users/register \-H "Content-Type: application/json" \-d '{"name": "John Doe", "email": "john@example.com", "password": "password123"}'

- **User Login**:  POST /api/users/login
- **User Profile**: GET /api/users/profile

---

## 🛠️ Setup Instructions  
Follow these steps to run the project locally:

1. **Clone the Repository**:
   ```bash
   git clone git@github.com:Vanshikashah318/User_Management_System.git
   cd User_Management_System
2. **Install Dependencies loaclly**:
    ```bash
   npm install

3.**Set Up Environment Variables**:
Create a .env file in the root directory and add the following:
 ```bash
MONGODB_URI=mongodb+srv://<username>:<password>@cluster.mongodb.net/myDatabase?retryWrites=true&w=majority
JWT_SECRET=your_jwt_secret
---



