# Meesho Clone - E-commerce Website

## Overview
The **Meesho Clone** is a comprehensive e-commerce platform designed to replicate the features and functionality of Meesho. This application empowers users to browse, buy, and sell products effortlessly. It includes features like product listing, order management, social sharing for resellers, and secure payment integration.

## Features
- **User Roles**:
  - Buyers: Browse and purchase products.
  - Sellers: List products and manage orders.
- **Product Management**:
  - Add, edit, and delete products.
  - Categorize products for better discoverability.
- **Order Management**:
  - Track orders with detailed statuses.
  - Easy returns and refunds.
- **Social Sharing for Resellers**:
  - Share products on social media platforms.
  - Generate reseller commissions on sales.
- **Secure Payments**:
  - Integrated payment gateways (Razorpay, PayPal, etc.).
  - Cash-on-delivery support.
- **Discounts and Offers**:
  - Coupons, bulk discounts, and referral bonuses.
- **Mobile-Responsive Design**: Optimized for smartphones, tablets, and desktops.
- **Customer Support**: In-app chat and ticketing system.

## Tech Stack
- **Frontend**: ReactJS, Redux Toolkit, TailwindCSS
- **Backend**: Node.js, Express.js
- **Database**: MongoDB
- **Authentication**: Firebase Authentication, JSON Web Tokens (JWT)
- **Payments**: Razorpay SDK, PayPal API
- **Cloud Services**: AWS S3 for image hosting

## Installation

### Prerequisites
- Node.js (v14 or above)
- MongoDB (local or cloud instance)
- npm or yarn

### Steps to Run Locally

1. Clone the repository:
   ```bash
   git clone https://github.com/username/meesho-clone.git
   cd meesho-clone
   ```

2. Install dependencies for both frontend and backend:
   ```bash
   cd client
   npm install
   cd ../server
   npm install
   ```

3. Set up environment variables:
   Create a `.env` file in the `server` directory with the following:
   ```env
   MONGO_URI=your_mongodb_connection_string
   JWT_SECRET=your_jwt_secret
   RAZORPAY_KEY_ID=your_razorpay_key_id
   RAZORPAY_KEY_SECRET=your_razorpay_key_secret
   AWS_ACCESS_KEY=your_aws_access_key
   AWS_SECRET_KEY=your_aws_secret_key
   ```

4. Start the development servers:
   ```bash
   # Start backend server
   cd server
   npm run dev

   # Start frontend server
   cd ../client
   npm start
   ```

5. Open your browser and navigate to `http://localhost:3000` to access the app.

## Folder Structure
```
meesho-clone/
├── client/               # ReactJS frontend
│   ├── src/
│   │   ├── components/   # Reusable components
│   │   ├── pages/        # Application pages
│   │   ├── hooks/        # Custom hooks
│   │   └── utils/        # Utility functions
│   ├── public/           # Public assets
│   └── package.json      # Frontend dependencies
├── server/               # Node.js backend
│   ├── models/           # Database models
│   ├── routes/           # API routes
│   ├── controllers/      # Business logic
│   ├── middleware/       # Express middleware
│   └── package.json      # Backend dependencies
├── README.md             # Project documentation
└── .gitignore            # Ignored files and folders
```

## API Endpoints

### Authentication
- **POST** `/api/auth/register` - Register a new user
- **POST** `/api/auth/login` - Login user

### Products
- **GET** `/api/products` - Fetch all products
- **POST** `/api/products` - Add a new product (seller only)
- **PUT** `/api/products/:id` - Update a product (seller only)
- **DELETE** `/api/products/:id` - Delete a product (seller only)

### Orders
- **GET** `/api/orders` - Fetch all orders (buyer or seller specific)
- **POST** `/api/orders` - Place a new order
- **PUT** `/api/orders/:id` - Update order status
- **DELETE** `/api/orders/:id` - Cancel an order

### Payments
- **POST** `/api/payments` - Initiate payment
- **GET** `/api/payments/status` - Check payment status

### Resellers
- **GET** `/api/resellers/commissions` - Fetch reseller commissions

## Contribution

1. Fork the repository and create your branch:
   ```bash
   git checkout -b feature/your-feature
   ```

2. Commit your changes:
   ```bash
   git commit -m "Add your message"
   ```

3. Push to the branch:
   ```bash
   git push origin feature/your-feature
   ```

4. Open a pull request.

## License
This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

## Contact
For queries or issues, please contact:
- **Md Jasim Ansari**  

