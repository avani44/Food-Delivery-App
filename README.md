# 🍔 Food Delivery Web Application

A full-stack Food Delivery Web Application that allows users to browse food items, manage cart, place orders, and make secure payments. The application also includes an admin panel to manage and track orders.

---

## 🚀 Features

### 👤 User Features

* 🔐 User Authentication (JWT आधारित Login/Register)
* 🍕 Browse Food Items
* 🛒 Add to Cart / Remove from Cart
* 💳 Secure Payment using Stripe
* 📦 Place Orders
* 📜 View Order History (My Orders)
* 📍 Track Order Status

---

### 🧑‍💼 Admin Features

* 📊 View All Orders
* 🔄 Update Order Status (Pending → Paid → Delivered)
* 🍽️ Manage Food Items (Add / Edit / Delete)

---

## 🛠️ Tech Stack

### Frontend

* React.js
* Axios
* CSS

### Backend

* Node.js
* Express.js

### Database

* MySQL

### Authentication

* JWT (JSON Web Token)

### Payment Gateway

* Stripe

---

## 📂 Project Structure

```
Food_Delivery_App/
│
├── frontend/          # React Frontend
│   ├── src/
│   └── package.json
│
├── backend/           # Node.js Backend
│   ├── controllers/
│   ├── routes/
│   ├── middleware/
│   ├── config/
│   └── server.js
│
└── README.md
```

---

## ⚙️ Installation & Setup

### 🔹 Clone the Repository

```
git clone https://github.com/your-username/food-delivery-app.git
cd food-delivery-app
```

---

### 🔹 Backend Setup

```
cd backend
npm install
npm run server
```

---

### 🔹 Frontend Setup

```
cd frontend
npm install
npm run dev
```

---

## 🔐 Environment Variables

Create a `.env` file in backend:

```
JWT_SECRET=your_secret_key
STRIPE_SECRET_KEY=your_stripe_key
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=your_password
DB_NAME=food_app
```

---

## 📊 API Endpoints

### 🔹 User

* POST `/api/user/register`
* POST `/api/user/login`

### 🔹 Cart

* POST `/api/cart/add`
* POST `/api/cart/remove`
* POST `/api/cart/get`

### 🔹 Orders

* POST `/api/order/place`
* POST `/api/order/verify`
* POST `/api/order/userorders`
* GET `/api/order/list` (Admin)

---

## 📌 Example Order

```json
{
  "id": 1,
  "user_id": 4,
  "items": [
    { "name": "Pizza", "price": 200, "quantity": 2 }
  ],
  "amount": 400,
  "status": "pending"
}
```

---

## 🚀 Future Enhancements

* 🔔 Real-time order tracking (Socket.io)
* 🧭 Delivery partner system
* 🤖 AI-based food recommendations
* 📈 Admin analytics dashboard
* ⭐ Ratings & reviews system

---

## 🧠 Challenges Faced

* Handling JSON data from MySQL
* Managing JWT authentication across requests
* Integrating Stripe payment flow
* Debugging API and frontend state issues

---

## 👨‍💻 Author

**Avani Joshi**

---

## ⭐ Support

If you like this project, give it a ⭐ on GitHub!
