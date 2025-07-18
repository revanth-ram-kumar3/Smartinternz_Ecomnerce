﻿# smartinternz_Ecommerce
# 🏍️ ShopEZ - E-commerce Full Stack Application

Welcome to **ShopEZ**, a complete full-stack e-commerce platform built using **MERN stack** (MongoDB, Express, React, Node.js). It allows customers to browse products, manage carts, and place orders. Admins can manage inventory, categories, banners, and orders.

---

## 📁 Project Structure

```
ShopEZ/
🔹 client/                    # Frontend (React)
│   🔹 public/
│   🔹 src/
│   │   🔹 components/        # Reusable components (Navbar, Footer, Login, etc.)
│   │   🔹 context/           # React Context for global state
│   │   🔹 images/            # Static assets
│   │   🔹 pages/             # Main page views (Home, ProductDetails, etc.)
│   │   🔹 styles/            # CSS styles
│   │   🔹 App.js             # Root component
│   │   🔹 index.js           # React entry point
│   🔹 package.json
│
🔹 server/                   # Backend (Node.js, Express)
│   🔹 index.js              # Server & API routes
│   🔹 Schema.js             # MongoDB Schemas (User, Product, Order, etc.)
│   🔹 .env                  # Environment variables
│   🔹 package.json
│
🔹 README.md                 # Project Documentation
🔹 .gitignore
```

---

## 🧠 Key Features

### 👤 User

* Registration/Login (Role-based: Customer/Admin)
* View product list and details
* Add to cart and manage quantity
* Place orders with order details
* View past orders

### 🛒 Admin

* Admin login dashboard
* Add/Edit/Delete products
* Upload banner
* Create new categories
* View all users and orders
* Update order statuses

---

## 💻 Technologies Used

### Frontend:

* React JS
* React Context API
* Axios
* Bootstrap/CSS

### Backend:

* Node.js
* Express.js
* MongoDB + Mongoose
* bcrypt (for password encryption)
* dotenv (for environment configuration)

### Database:

* MongoDB (MongoDB Atlas)

---

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/revanth-ram-kumar3/Smartinternz_Ecomnerce.git
cd Smartinternz_Ecomnerce
```

### 2. Setup Backend

```bash
cd server
npm install
# Create a .env file in /server with the following:
# MONGO_URI=<your-mongodb-uri>
# PORT=6001
npm start
```

### 3. Setup Frontend

```bash
cd client
npm install
npm start
```

---

## 🔐 .env Configuration (Backend)

Create a file named `.env` in the `/server` directory and add:

```env
MONGO_URI=your_mongodb_connection_string
PORT=6001
```

---

## 📬 API Endpoints

| Method | Endpoint             | Description                  |
| ------ | -------------------- | ---------------------------- |
| POST   | /register            | Register new user            |
| POST   | /login               | Login existing user          |
| GET    | /fetch-products      | Get all products             |
| POST   | /add-to-cart         | Add product to cart          |
| GET    | /fetch-cart          | Get user's cart items        |
| POST   | /buy-product         | Direct product purchase      |
| POST   | /place-cart-order    | Place order from cart        |
| PUT    | /cancel-order        | Cancel an order              |
| PUT    | /update-order-status | Update order delivery status |
| GET    | /fetch-orders        | View all orders (admin)      |

---

## 👨‍💼 Admin Access

After registering a user with `usertype = "admin"` manually in DB (or programmatically), login as admin to access the admin dashboard.

Admin capabilities:

* Add/Update/Delete Products
* Manage Orders
* Upload Banners
* Manage Categories

---

## 🔎 Pages Overview

| Page            | Path           | Role       |
| --------------- | -------------- | ---------- |
| Login           | `/login`       | All        |
| Register        | `/register`    | All        |
| Home            | `/`            | Customer   |
| Products        | `/products`    | Customer   |
| Product Details | `/product/:id` | Customer   |
| Admin Dashboard | `/admin`       | Admin Only |
| Cart            | `/cart`        | Customer   |
| Orders          | `/orders`      | Admin      |

---

## 📷 Screenshots

Include in `/README.md` or `/docs`:

* 🗀️ Login Page
* 🛒 Product List
* 📦 Order Placement Page
* 📊 Admin Product Management
* 🌟 Admin Order Status

---

## ⚙️ Deployment Instructions

You can deploy using services like:

* **Frontend**: Vercel / Netlify
* **Backend**: Render / Railway
* **Database**: MongoDB Atlas

---

## 📊 Future Enhancements

* JWT Token Authentication
* Stripe Integration for real payment
* Product Ratings & Reviews
* Email Order Confirmations
* Admin Analytics Dashboard

---

## 🧠 Contributors & Credits

Built by [Tangella Revanth Ram Kumar](https://github.com/revanth-ram-kumar3)
SmartInternz E-Commerce Internship Project

---

## 📄 License

This project is licensed for educational purposes. You may extend, contribute, or customize for personal use.

---

## 🙌 Acknowledgements

* MongoDB University
* React Documentation
* Express JS Guide
* Bootstrap
