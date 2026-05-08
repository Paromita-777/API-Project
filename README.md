# Grocery Management System REST API

A secure and scalable Grocery Management System developed for Gelos Enterprises using MongoDB, Node.js, Express.js and JWT authentication.

The project was designed to manage grocery store operations by storing and analysing product, order, employee and cart data using a NoSQL database architecture.

---

##  Project Overview

This project was developed as part of a software development task for Gelos Enterprises.

The system provides:
- Product management
- Employee authentication
- Role-based access control
- RESTful API functionality
- MongoDB database integration
- Secure JWT authentication
- CORS support
- API testing using Postman

The API allows front-end developers to consume data efficiently while supporting scalability and high availability using MongoDB Atlas.

---

## 🛠 Technologies Used

### Backend
- Node.js
- Express.js
- MongoDB
- MongoDB Atlas
- Mongoose
- JWT (JSON Web Token)
- bcrypt.js

### Testing & Documentation
- Postman
- Swagger 

### Other Tools
- CORS
- dotenv
- Nodemon

---

## 📂 Database Collections

### 1. Products Collection

| Field | Type |
|---|---|
| sku | String |
| name | String |
| price | Number |
| stockOnHand | Number |

### 2. Orders Collection

| Field | Type |
|---|---|
| orderNo | Number |
| orderDate | Date |
| customerNo | Number |
| paymentMethod | String |
| productSku | String |
| productName | String |
| productPrice | Number |
| quantity | Number |

### 3. Employees Collection

| Field | Type |
|---|---|
| empId | Number |
| firstName | String |
| lastName | String |
| username | String |
| password | String / Hash |

### 4. Carts Collection

| Field | Type |
|---|---|
| customerNo | Number |
| products | Array |
| createdAt | Date |

---

## 🔐 User Roles & Permissions

### Store Manager
- Full CRUD access
- Can view, update, and delete:
  - Products
  - Orders
  - Employees
  - Carts

### Billing Employee
- Limited access
- Can:
  - View orders
  - Update orders
  - View carts

---

## 🚀 Features

- RESTful API architecture
- CRUD operations for products
- JWT authentication and authorisation
- Role-based access control
- MongoDB Atlas cloud database
- Password hashing using bcrypt
- Middleware-based authentication
- Secure API endpoints
- CORS implementation
- MongoDB indexing and performance testing
- Trigger notification testing
- API endpoint testing using Postman

---


## 📌 REST API Endpoints

### Authentication

| Method | Endpoint | Description |
|---|---|---|
| POST | /employees/login | Employee login |

### Products CRUD

| Method | Endpoint | Description |
|---|---|---|
| GET | /products | Get all products |
| GET | /products/:id | Get single product |
| POST | /products | Create product |
| PUT | /products/:id | Replace product |
| PATCH | /products/:id | Update product |
| DELETE | /products/:id | Delete product |

---

## 🔐 JWT Authentication

The API uses:
- JSON Web Tokens (JWT)
- Bearer Authentication
- Protected routes
- Role-based authorisation

Example Authorization Header:

```http
Authorization: Bearer your_jwt_token
```

---

## 🌐 CORS Implementation

CORS has been enabled for all origins using Express middleware.

Features tested:
- Cross-origin requests
- Pre-flight OPTIONS requests
- Allowed headers
- API accessibility from browsers

---

## 🧪 Testing

### MongoDB Testing
- Inserted sample JSON data
- Tested CRUD operations
- Created single indexes
- Created compound indexes
- Tested query performance improvements
- Tested MongoDB Atlas trigger notifications

### REST API Testing
All endpoints tested using Postman:
- GET
- POST
- PUT
- PATCH
- DELETE

### Authentication Testing
Tested:
- Valid login credentials
- Invalid login credentials
- Protected endpoints with token
- Protected endpoints without token
- Role-based authorisation

---

## 📖 Learning Outcomes

Through this project, I gained practical experience in:
- Building RESTful APIs
- NoSQL database design
- MongoDB Atlas integration
- JWT authentication
- Role-based security
- API testing with Postman
- Backend architecture
- Middleware implementation
- CRUD functionality
- MongoDB indexing and optimisation

---

## 👩‍💻 Author

Paromita Sarkar
