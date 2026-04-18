# 🛍️ ShopMini — Full Stack Shopping Website

A clean, modern general store built with vanilla HTML/CSS/JS frontend and Node.js + Express backend.

---

## 📁 Folder Structure

```
shop/
├── frontend/
│   ├── pages/
│   │   └── index.html        ← Main app (open this in browser)
│   ├── components/
│   │   ├── Navbar.js         ← Navbar component
│   │   ├── ProductCard.js    ← Product card component
│   │   └── Cart.js           ← Cart sidebar component
│   ├── styles/
│   │   ├── variables.css     ← CSS variables & reset
│   │   └── main.css          ← All component styles
│   └── data/
│       └── products.js       ← Frontend product data
│
├── backend/
│   ├── server.js             ← Express app entry point
│   ├── package.json
│   ├── routes/
│   │   ├── products.js       ← GET /api/products routes
│   │   └── cart.js           ← Cart API routes
│   ├── controllers/
│   │   ├── productController.js
│   │   └── cartController.js
│   ├── models/
│   │   └── products.js       ← Product data / "database"
│   └── middleware/
│       └── cors.js           ← CORS middleware
│
└── README.md
```

---

## 🚀 Running the App

### Frontend Only (instant, no install needed)
Just open `frontend/pages/index.html` in your browser. Everything works standalone.

### Full Stack (Frontend + Backend API)
```bash
cd backend
npm install
npm start
# API runs at http://localhost:3001
```

**API Endpoints:**
| Method | Endpoint | Description |
|--------|----------|-------------|
| GET | /api/products | List all products |
| GET | /api/products?category=Electronics | Filter by category |
| GET | /api/products?sort=price-asc | Sort products |
| GET | /api/products?search=watch | Search products |
| GET | /api/products/:id | Get single product |
| GET | /api/products/categories | List all categories |
| GET | /api/cart | View cart |
| POST | /api/cart/add | Add item `{ productId, quantity }` |
| PUT | /api/cart/update | Update qty `{ productId, quantity }` |
| DELETE | /api/cart/clear | Clear cart |
| POST | /api/cart/checkout | Place order |

---

## ✨ Features
- 🛍️ Browse 8 products across Electronics, Fashion & Home
- 🔍 Live search & category filter
- 📊 Sort by price or rating
- 🛒 Add to cart with quantity control
- 💳 Checkout with order confirmation
- ❤️ Wishlist toggle
- 📱 Fully responsive (mobile-friendly)
- 🎨 Modern & minimal design (Playfair Display + DM Sans)
- ✨ Smooth animations & toast notifications

---

## 🛠 Tech Stack
| Layer | Tech |
|-------|------|
| Frontend | Vanilla HTML, CSS, JavaScript |
| Backend | Node.js, Express |
| Database | In-memory (easy to swap with MongoDB/PostgreSQL) |
| Fonts | Google Fonts (Playfair Display, DM Sans) |
| Images | Unsplash |
