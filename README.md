# 🛒 ShopSphere - Full-Stack E-Commerce Platform

> Built on top of the open-source project [ecommerce_project](https://github.com/dhrub404/ecommerce_project) by dhrub404 (original name: Cartify). Modified and extended by [codersingh74](https://github.com/codersingh74).
## ✨ Features

### 🎨 Modern UI/UX
- **Premium Design**: Gradient branding, glassmorphism headers, and polished typography ("Outfit" font).
- **Responsive Layout**: Mobile-first design using React Bootstrap and custom CSS.
- **Micro-interactions**: 
  - 3D-style Wishlist Heart toggle.
  - Animated "Empty Cart" and "Empty Wishlist" states.
  - Hover effects on product cards and buttons.

### 👤 User Authentication
- User registration and login
- JWT-based authentication (Access/Refresh tokens)
- Protected routes (Orders, Profile)

### 🛍️ Shopping Experience
- **Product Catalog**: Grid view with ratings (`4.5 ★`) and review counts.
- **Search**: Real-time product search functionality.
- **Product Details**: Comprehensive view with images, descriptions, and stock status.

### 🛒 Shopping Cart
- **Redesigned Cart**: Clean white-card layout with purple accents.
- **Smart Management**: Add/remove items, update quantities.
- **Live Summary**: Real-time subtotal and total calculation.
- **Persistence**: Cart state synced with backend/local storage.

### ❤️ Wishlist
- **Toggle Feature**: Heart icon on product cards toggles add/remove instantly.
- **Visual Feedback**: Red heart animation on selection.
- **Management Page**: Dedicated screen to view and remove saved items.
- **Empty State**: Beautiful animated heart pulse when wishlist is empty.

### 📦 Order Management
- **Seamless Checkout**: Streamlined process from Cart to Order placement.
- **Order Success Screen**: 
  - **Animation**: Green Checkmark pop-in effect.
  - **Details Card**: Full summary with images, order ID, and expected delivery date.
- **Order History**: View past orders with status and totals.

### 🎯 Additional Features
- **Toast Notifications**: Custom stacked toast messages for actions (though heavily refined for cleaner UX).
- **Profile Dashboard**: Sidebar navigation for Profile, Orders, and Addresses.
- **Interactive Elements**: animated buttons and loading states.

## 🚀 Tech Stack

### Frontend
- **React 19** - UI library
- **Redux Toolkit** - State management
- **React Bootstrap** - Responsive components
- **Vite** - High-speed build tool
- **CSS3** - Custom variables, animations, and gradients

### Backend
- **Django** - High-level Python web framework
- **Django REST Framework (DRF)** - Powerful API construction
- **SQLite** - Default database (easily scalable to PostgreSQL)
- **JWT** - Secure authentication

## 📁 Project Structure

```
ecommerce_project/
├── backend/
│   ├── manage.py              # Django entry point
│   ├── ecommerce_project/     # Project settings
│   ├── products/              # Product & Wishlist logic
│   ├── users/                 # Auth & Profile logic
│   ├── orders/                # Order management logic
│   └── cart/                  # Cart management logic
│
├── frontend/
│   ├── src/
│   │   ├── components/
│   │   │   ├── Navbar.jsx     # "Cartify" branded navbar
│   │   │   ├── ...
│   │   │
│   │   ├── screens/
│   │   │   ├── ProductListScreen.jsx  # Home page
│   │   │   ├── CartScreen.jsx         # Redesigned Cart
│   │   │   ├── WishlistScreen.jsx     # New Wishlist UI
│   │   │   ├── OrderSuccessScreen.jsx # Animated Success
│   │   │   ├── ...
│   │   │
│   │   ├── actions/           # Redux actions
│   │   ├── reducers/          # Redux reducers
│   │   ├── App.jsx            # Main routing
│   │   └── index.css          # Global premium styles
│   │
│   └── package.json
```

## 🛠️ Installation & Setup

### Backend (Django)

1. **Create virtual environment**
   ```bash
   python -m venv .venv
   # Windows
   .venv\Scripts\activate
   ```

2. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   cd backend
   ```

3. **Run migrations**
   ```bash
   python manage.py migrate
   ```

4. **Start server**
   ```bash
   python manage.py runserver
   ```
   Backend runs at: `http://127.0.0.1:8000`

### Frontend (React + Vite)

1. **Navigate to frontend**
   ```bash
   cd frontend
   ```

2. **Install dependencies**
   ```bash
   npm install
   ```

3. **Start development server**
   ```bash
   npm run dev
   ```
   Frontend runs at: `http://localhost:5173`

## 🔐 User-Specific Data

- **Cart & Orders**: Stored in database linked to the authenticated user.
- **Wishlist**: Currently utilizes LocalStorage for immediate interaction, with backend sync architecture ready.

## 🤝 Contributing

This project is part of a premium e-commerce portfolio.

**Happy Shopping with Cartify! 🛍️**