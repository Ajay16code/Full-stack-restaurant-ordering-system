# 🍽️ Restaurant Ordering System

A full-stack **Restaurant Ordering Web Application** built using **Vue.js (frontend)**, **Node.js + Express (backend)**, and **MySQL (database)**.  
Customers can browse menus, add food items to their cart, and place orders online. Admins can manage food items, tables, bills, and more.

---

## 🚀 Features

### 👨‍💻 User Features
- View all food items with images, descriptions, and prices  
- Add or remove items from the cart  
- Book a table or place an online order  
- Checkout and view bill details  

### 🧑‍🍳 Admin Features
- Add, update, and delete food items  
- Manage tables and booking status  
- View and update order & billing details  
- Monitor sales and restaurant data  

---

## 🧩 Tech Stack

| Layer | Technology |
|-------|-------------|
| **Frontend** | Vue.js |
| **Backend** | Node.js + Express.js |
| **Database** | MySQL |
| **Tools** | phpMyAdmin, XAMPP |
| **Development** | Nodemon, Axios, CORS |

---

## 🗂️ Project Structure

```

restaurant-ordering-system/
│
├── backend/
│   ├── controllers/            # Handles business logic
│   ├── models/                 # MySQL table models
│   ├── routes/                 # Express API routes
│   ├── index.js                # Main server file
│   ├── package.json
│   └── restaurant_management/  # Static build files
│
├── frontend/
│   ├── public/
│   ├── src/
│   │   ├── components/         # Vue components (FoodList, Cart, etc.)
│   │   ├── views/              # Page views
│   │   ├── router/             # Vue Router setup
│   │   ├── store/              # Vuex store (if used)
│   │   └── App.vue
│   ├── vue.config.js           # Proxy setup
│   ├── package.json
│   └── README.md
│
└── README.md                   # (this file)

````

---

## ⚙️ Installation Guide

### 🧠 Prerequisites

Make sure the following are installed:
- **Node.js** (v16 or higher)
- **npm** (comes with Node)
- **MySQL** (via XAMPP or Workbench)
- **phpMyAdmin** (for database management)

---

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/restaurant-ordering-system.git
cd restaurant-ordering-system
````

---

### 2️⃣ Set Up the Database

1. Start **XAMPP** → Turn on **Apache** and **MySQL**
2. Open [http://localhost/phpmyadmin](http://localhost/phpmyadmin)
3. Create a new database:

```sql
CREATE DATABASE db_restaurant;
```

4. Import your SQL file (if available) or manually create tables like:

   * `food`
   * `cart`
   * `user`
   * `booktable`
   * `bill`

---

### 3️⃣ Configure Environment Variables

Create a file named **.env** inside the `backend/` folder:

```env
PORT=8001
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=
DB_NAME=db_restaurant
```

---

### 4️⃣ Install Dependencies

#### 📦 Backend

```bash
cd backend
npm install
```

#### 💻 Frontend

```bash
cd ../frontend
npm install
```

---

### 5️⃣ Run the Application

#### ▶️ Run Backend (Node + Express)

```bash
cd backend
npx nodemon index.js
```

Server runs at 👉 [http://localhost:8001](http://localhost:8001)

#### 🌐 Run Frontend (Vue)

```bash
cd frontend
npm run serve
```

Frontend runs at 👉 [http://localhost:8080](http://localhost:8080)

---

## 🔗 API Endpoints (Examples)

| Method | Endpoint         | Description             |
| ------ | ---------------- | ----------------------- |
| GET    | `/api/food`      | Get all food items      |
| POST   | `/api/food`      | Add a new food item     |
| PUT    | `/api/food/:id`  | Update a food item      |
| DELETE | `/api/food/:id`  | Delete a food item      |
| GET    | `/api/cart`      | Fetch user cart         |
| POST   | `/api/booktable` | Book a restaurant table |

---

## 🧠 Common Issues & Fixes

### ❌ Error: Unknown database 'db_restaurant'

✅ Ensure the database name in `.env` exactly matches your phpMyAdmin database name.

### ❌ Proxy Error: ECONNREFUSED

✅ Make sure your backend (running with `nodemon index.js`) is started **before** running the frontend.

### ❌ MySQL Connection Error

✅ Start MySQL in XAMPP and verify your `.env` credentials are correct.

---

## 📦 Build for Production

To build your Vue frontend for deployment:

```bash
cd frontend
npm run build
```

This creates a `/dist` folder that can be served by Express or any static hosting service.

---

## 🖥️ Deployment (Optional)

| Layer                 | Recommended Platform       |
| --------------------- | -------------------------- |
| **Backend (Node.js)** | Render / Railway           |
| **Database (MySQL)**  | PlanetScale / Clever Cloud |
| **Frontend (Vue)**    | Netlify / Vercel           |

---

## 📸 Screenshots (Optional)

### 🧾 Example UI

You can add screenshots to show how the system looks:

```markdown
![Home Page](screenshots/home.png)
![Food List](screenshots/food-list.png)
![Admin Dashboard](screenshots/admin.png)
```

---

## 👨‍💻 Author

**Ajay / Abinav**
💻 Full Stack Developer
📧 [your-email@example.com](mailto:your-email@example.com)
🌐 GitHub: [https://github.com/<your-username>](https://github.com/<your-username>)

---

## 🪪 License

This project is licensed under the **MIT License** — feel free to modify and use it.

---

## ⭐ Acknowledgements

* Quang’s Restaurant System Repository
* BezKoder Node + MySQL Tutorials
* Vue CLI Documentation
* Express.js Documentation
* MySQL Official Docs

```
