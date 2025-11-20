# CodeAlpha_E-Commerce
# ShopHub - E-Commerce Platform

A full-stack e-commerce web application built with Node.js, Express, MongoDB, and vanilla JavaScript.

How to run
In terminal window write,
cd backend
npm run dev

## 📋 Table of Contents

- [Features](#features)
- [Tech Stack](#tech-stack)
- [Project Structure](#project-structure)
- [Installation](#installation)
- [Usage](#usage)
- [API Endpoints](#api-endpoints)
- [Screenshots](#screenshots)
- [Future Enhancements](#future-enhancements)
- [Contributing](#contributing)
- [License](#license)

## ✨ Features

### Customer Features
- 🛍️ **Product Browsing** - View all available products with images, prices, and ratings
- 🔍 **Product Details** - Detailed product information page
- 🛒 **Shopping Cart** - Add, remove, and update product quantities
- 👤 **User Authentication** - Secure registration and login system
- 💳 **Checkout Process** - Complete order placement with shipping details
- 📱 **Responsive Design** - Mobile-friendly interface

### Technical Features
- 🔐 **JWT Authentication** - Secure token-based authentication
- 🔒 **Password Encryption** - bcryptjs for secure password hashing
- 📊 **RESTful API** - Well-structured API endpoints
- 💾 **MongoDB Database** - NoSQL database for flexible data storage
- ⚡ **Real-time Updates** - Dynamic cart and order management

## 🛠️ Tech Stack

### Frontend
- **HTML5** - Structure
- **CSS3** - Styling with modern flexbox and grid
- **JavaScript (ES6+)** - Client-side logic
- **Fetch API** - HTTP requests

### Backend
- **Node.js** - Runtime environment
- **Express.js** - Web framework
- **MongoDB** - NoSQL database
- **Mongoose** - ODM for MongoDB

### Authentication & Security
- **JWT (jsonwebtoken)** - Token-based authentication
- **bcryptjs** - Password hashing
- **CORS** - Cross-Origin Resource Sharing

## 📁 Project Structure
```
E-commerce-store/
├── backend/
│   ├── config/
│   │   └── db.js                 # Database connection
│   ├── middleware/
│   │   └── auth.js               # Authentication middleware
│   ├── models/
│   │   ├── Product.js            # Product schema
│   │   ├── User.js               # User schema
│   │   └── Order.js              # Order schema
│   ├── routes/
│   │   ├── productRoutes.js      # Product API routes
│   │   ├── userRoutes.js         # User API routes
│   │   └── orderRoutes.js        # Order API routes
│   ├── .env                      # Environment variables
│   ├── .gitignore                # Git ignore file
│   ├── package.json              # Dependencies
│   └── server.js                 # Entry point
│
└── frontend/
    ├── css/
    │   └── style.css             # All styles
    ├── js/
    │   ├── main.js               # Main JavaScript
    │   ├── cart.js               # Cart functionality
    │   └── auth.js               # Authentication logic
    ├── images/                   # Product images
    ├── index.html                # Home page
    ├── product.html              # Product details page
    ├── cart.html                 # Shopping cart page
    ├── checkout.html             # Checkout page
    ├── login.html                # Login page
    └── register.html             # Registration page
```

## 🚀 Installation

### Prerequisites
- Node.js (v14 or higher)
- MongoDB (local installation or MongoDB Atlas account)
- npm or yarn package manager

### Step 1: Clone the repository
```bash
git clone https://github.com/yourusername/shophub-ecommerce.git
cd shophub-ecommerce
```

### Step 2: Install backend dependencies
```bash
cd backend
npm install
```

### Step 3: Set up environment variables

Create a `.env` file in the `backend` directory:
```env
PORT=5000
MONGODB_URI=mongodb://localhost:27017/ecommerce_db
JWT_SECRET=your_super_secret_key_change_this_in_production
```

### Step 4: Start MongoDB

**Local MongoDB:**
```bash
mongod
```

**Or use MongoDB Atlas** - Update the `MONGODB_URI` in `.env` with your Atlas connection string

### Step 5: Start the backend server
```bash
cd backend
npm run dev
```

The backend server will run on `http://localhost:5000`

### Step 6: Start the frontend

Option 1: Using Live Server (VS Code extension)
- Right-click on `frontend/index.html`
- Select "Open with Live Server"

Option 2: Open directly in browser
- Navigate to `frontend/index.html` and open in your browser

The frontend will run on `http://localhost:5500` (Live Server) or `file:///path/to/frontend/index.html`

## 💻 Usage

### For Development

1. **Start Backend Server:**
```bash
cd backend
npm run dev
```

2. **Start Frontend:**
   - Use Live Server extension in VS Code
   - Or open `frontend/index.html` in browser

### Default Test Account

You can register a new account or use these test credentials:
```
Email: test@example.com
Password: test123
```

## 📡 API Endpoints

### Products

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| GET | `/api/products` | Get all products | No |
| GET | `/api/products/:id` | Get single product | No |
| POST | `/api/products` | Create product | No |
| PUT | `/api/products/:id` | Update product | No |
| DELETE | `/api/products/:id` | Delete product | No |

### Users

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/api/users/register` | Register new user | No |
| POST | `/api/users/login` | Login user | No |

### Orders

| Method | Endpoint | Description | Auth Required |
|--------|----------|-------------|---------------|
| POST | `/api/orders` | Create new order | Yes |
| GET | `/api/orders/myorders` | Get user's orders | Yes |
| GET | `/api/orders/:id` | Get order by ID | Yes |

## 📸 Screenshots

### Home Page
![Home Page](screenshots/home.png)

### Product Details
![Product Details](screenshots/product-details.png)

### Shopping Cart
![Shopping Cart](screenshots/cart.png)

### Checkout
![Checkout](screenshots/checkout.png)

## 🔮 Future Enhancements

- [ ] Admin dashboard for product and order management
- [ ] Payment gateway integration (Stripe/PayPal)
- [ ] Product search and filtering
- [ ] Product reviews and ratings
- [ ] Order tracking system
- [ ] Email notifications
- [ ] Wishlist functionality
- [ ] Multiple product images
- [ ] Product categories management
- [ ] Inventory management
- [ ] Sales analytics dashboard

## 🤝 Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the project
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

## 📝 License

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## 👨‍💻 Author

**Your Name**
- GitHub: [@Anush0088] https://github.com/Anush0088
- LinkedIn:[Anush Karanapu] https://www.linkedin.com/in/anush-karanapu-043174290?utm_source=share&utm_campaign=share_via&utm_content=profile&utm_medium=ios_app
- Email: karanapuanush@gmail.com

## 🙏 Acknowledgments

- Product images from [Unsplash](https://unsplash.com)
- Icons from various sources
- Inspiration from modern e-commerce platforms

---

⭐ If you found this project helpful, please give it a star!

Made with ❤️ and ☕
