# Node Secure Auth API

A production-style Node.js backend API featuring secure authentication, JWT access & refresh tokens, file uploads, and full account lifecycle management.

Built to mirror real-world SaaS backend architecture — not a CRUD demo.

---

## Features

### Authentication & Security
- User registration with hashed passwords (bcrypt)
- JWT Access Tokens (short-lived)
- JWT Refresh Tokens (long-lived with DB storage)
- Secure logout with refresh token invalidation
- Email verification after registration
- Forgot password & secure reset flow (token-based)

### Product Management
- Create product with image upload (Multer)
- Get all products
- Get product by ID
- Update product (with optional new image)
- Delete product

### Protected Routes
- Auth middleware for secured endpoints
- Public read / private write access model

### File Handling
- Image uploads stored on disk
- Automatic filename generation
- Optional update support

---

##  Tech Stack

- Node.js
- Express.js
- MongoDB + Mongoose
- JWT (jsonwebtoken)
- Multer (file uploads)
- Bcrypt (password hashing)
- Crypto (secure token generation)

---

## 🔄 Auth Flow Overview
