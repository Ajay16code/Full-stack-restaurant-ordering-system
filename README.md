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

restaurant-ordering-system/
│
├── backend/
│ ├── controllers/ # Handles business logic
│ ├── models/ # MySQL table models
│ ├── routes/ # Express API routes
│ ├── index.js # Main server file
│ ├── package.json
│ └── restaurant_management/
│
├── frontend/
│ ├── public/
│ ├── src/
│ │ ├── components/ # Vue components (FoodList, Cart, etc.)
│ │ ├── views/ # Page views
│ │ ├── router/ # Vue Router
│ │ ├── store/ # Vuex (if used)
│ │ └── App.vue
│ ├── vue.config.js # Proxy setup
│ ├── package.json
│ └── README.md
│
└── README.md # (this file)

yaml
Copy code

---

## ⚙️ Installation Guide

### 🧠 Prerequisites
Make sure the following are installed:
- **Node.js** (v16 or higher)
- **npm** (comes with Node)
- **MySQL** (via XAMPP or Workbench)
- **phpMyAdmin** (for DB management)

---

### 1️⃣ Clone the Repository

```bash
git clone https://github.com/<your-username>/restaurant-ordering-system.git
cd restaurant-ordering-system
2️⃣ Set Up the Database
Start XAMPP → Turn on Apache and MySQL.

Open phpMyAdmin: http://localhost/phpmyadmin

Create a new database:

sql
Copy code
CREATE DATABASE db_restaurant;
Import your tables manually or create them as shown in your repo (food, cart, user, booktable, etc.).

3️⃣ Configure Environment Variables
Create a file named .env inside the backend/ folder:

env
Copy code
PORT=8001
DB_HOST=localhost
DB_USER=root
DB_PASSWORD=
DB_NAME=db_restaurant
4️⃣ Install Dependencies
📦 Backend
bash
Copy code
cd backend
npm install
💻 Frontend
bash
Copy code
cd ../frontend
npm install
5️⃣ Run the Application
▶️ Run Backend (Node + Express)
bash
Copy code
cd backend
npx nodemon index.js
Server runs at 👉 http://localhost:8001

🌐 Run Frontend (Vue)
bash
Copy code
cd frontend
npm run serve
Frontend runs at 👉 http://localhost:8080

🔗 API Endpoints (Examples)
Method	Endpoint	Description
GET	/api/food	Get all food items
POST	/api/food	Add a new food item
PUT	/api/food/:id	Update a food item
DELETE	/api/food/:id	Delete a food item
GET	/api/cart	Fetch user cart
POST	/api/booktable	Book a restaurant table

🧠 Common Issues & Fixes
❌ Error: Unknown database 'db_restaurant'
✅ Make sure the database name in .env exactly matches the one created in phpMyAdmin.

❌ Proxy Error: ECONNREFUSED
✅ Ensure your backend (nodemon index.js) is running before starting the frontend.

❌ MySQL Connection Error
✅ Start MySQL in XAMPP and verify credentials in .env.

📦 Build for Production
To build your Vue frontend for deployment:

bash
Copy code
cd frontend
npm run build
This creates a /dist folder that can be served using Express or any static hosting service.

🖥️ Deployment (Optional)
Layer	Recommended Platform
Backend (Node.js)	Render / Railway
Database (MySQL)	PlanetScale / Clever Cloud MySQL
Frontend (Vue)	Netlify / Vercel

📸 Screenshots (Optional)
You can include screenshots here:

markdown
Copy code
### 🧾 Example UI
![Home Page](screenshots/home.png)
![Food List](screenshots/food-list.png)
![Admin Dashboard](screenshots/admin.png)
👨‍💻 Author
Ajay / Abinav
💻 Full Stack Developer
📧 your-email@example.com
🌐 GitHub: https://github.com/<your-username>

🪪 License
This project is licensed under the MIT License — feel free to modify and use it.

⭐ Acknowledgements
Quang’s Restaurant System Repo

BezKoder Tutorials

Vue CLI and Express.js Documentation

MySQL Official Docs

yaml
Copy code

---

Would you like me to make this **version with GitHub badges (like "Made with Vue.js" / "License MIT")** and **
