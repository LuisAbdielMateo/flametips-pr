# 🔥 FlameTipsPR

**Puerto Rico's #1 Automotive E-Commerce Platform**  
A full-stack web app for selling muffler tips and car accessories.

---

## Tech Stack

| Layer     | Technology               |
|-----------|--------------------------|
| Frontend  | React + Vite             |
| Backend   | Node.js + Express        |
| Database  | MongoDB + Mongoose       |
| HTTP      | Axios + REST API         |

---

## Project Structure

```
Flametipspr/
├── backend/
│   ├── config/
│   │   └── db.js          # MongoDB connection
│   ├── models/
│   │   └── Product.js     # Mongoose schema
│   ├── routes/
│   │   └── products.js    # CRUD API routes
│   ├── seeder.js          # Seed sample products
│   ├── server.js          # Express entry point
│   └── .env               # Environment variables
│
└── frontend/
    └── src/
        ├── components/
        │   ├── Navbar.jsx
        │   ├── ProductCard.jsx
        │   ├── ProductForm.jsx
        │   └── Toast.jsx
        ├── pages/
        │   ├── Home.jsx       # Public storefront
        │   └── Admin.jsx      # Admin panel
        ├── services/
        │   └── productService.js  # Axios API calls
        ├── App.jsx
        └── main.jsx
```

---

## 🚀 Getting Started

### Prerequisites
- [Node.js](https://nodejs.org/) (v18+)
- [MongoDB](https://www.mongodb.com/try/download/community) running locally on default port `27017`

---

### 1. Start MongoDB

Make sure MongoDB is running. On Windows, start the MongoDB service or run:

```bash
mongod
```

---

### 2. Start the Backend

```bash
cd backend
npm start
```

The API will be available at `http://localhost:5000`

**Optional – Seed the database with sample products:**

```bash
npm run seed
```

---

### 3. Start the Frontend

Open a **new terminal** window:

```bash
cd frontend
npm run dev
```

The app will be available at `http://localhost:3000`

---

## API Endpoints

| Method | Endpoint          | Description            |
|--------|-------------------|------------------------|
| GET    | `/products`       | Get all products       |
| GET    | `/products/:id`   | Get single product     |
| POST   | `/products`       | Create a new product   |
| PUT    | `/products/:id`   | Update a product       |
| DELETE | `/products/:id`   | Delete a product       |

---

## Features

- 🛒 **Public Storefront** – Browse all products with search/filter
- ⚙️ **Admin Panel** – Add, edit, and delete products via modal forms
- 📦 **Real-time CRUD** – Instant UI updates without page refresh
- 🔔 **Toast Notifications** – Success/error feedback
- 📱 **Responsive Design** – Works on mobile and desktop
- 🌑 **Dark Automotive Theme** – Flame accent colors & premium styling

---

## Environment Variables

Located in `backend/.env`:

```
PORT=5000
MONGO_URI=mongodb://localhost:27017/flametipspr
```
