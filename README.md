# Node Secure Auth API

A production-style Node.js backend API implementing secure authentication, JWT access & refresh tokens, email verification, password reset flows, and protected CRUD operations with file uploads.

Built to reflect real-world SaaS backend architecture — not a tutorial project.

---

## 🚀 Features

### 🔐 Authentication & Security
- User registration with hashed passwords (bcrypt)
- Email verification after signup
- JWT Access Tokens (short-lived)
- JWT Refresh Tokens (long-lived & stored in database)
- Secure logout (refresh token invalidation)
- Forgot password flow with secure reset tokens
- Password reset with expiry & hashing

### 📦 Product Management
- Create product with image upload
- Get all products
- Get product by ID
- Update product (with optional image update)
- Delete product

### 🛡 Route Protection
- Middleware-based authentication
- Public read access
- Authenticated write access

### 📁 File Upload System
- Multer-based image uploads
- Disk storage
- Automatic filename handling

---

## 🧱 Tech Stack

- Node.js
- Express.js
- MongoDB + Mongoose
- JWT (jsonwebtoken)
- Bcrypt
- Multer
- Crypto

---

## 🔄 Authentication Flow

Register → Verify Email → Login  
Login → Access Token + Refresh Token  
Access expires → Refresh token issues new access  
Logout → Refresh token destroyed  
Forgot password → Secure reset token flow  

---

## 📌 API Endpoints

### Auth Routes
- POST /register
- POST /login
- POST /refresh-token
- POST /logout
- POST /forgot-password
- POST /reset-password
- GET  /verify-email

### Product Routes
- POST /products (protected + image upload)
- GET  /products
- GET  /products/:id
- PUT  /products/:id (protected)
- DELETE /products/:id (protected)

---

## ⚙ Setup & Run

```bash
git clone https://github.com/yourusername/node-secure-auth-api.git
cd node-secure-auth-api
npm install
