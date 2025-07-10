# Product Management API

A RESTful API built with Express.js for managing products with CRUD operations, authentication, and advanced features.

## Features
- ✅ Full CRUD operations for products
- 🔒 API key authentication
- 📝 Request logging
- ✔️ Input validation
- 🚨 Error handling with proper status codes
- 🔍 Advanced features:
  - Filtering by category
  - Pagination
  - Search functionality
  - Product statistics

## Installation

1. Clone the repository:
   ```bash
   git clone https://github.com/PLP-MERN-Stack-Development/week-2-express-js-assignment-CelsusK.git
   cd week-2-express-js-assignment-CelsusK
# install dependencies
   npm install
# Start the server
   node server.js
# Base URL
   http://localhost:3000/api
# End points
 Products
   Method	Endpoint	Description	Auth Required
   GET	/products	Get all products (filterable)	No
   GET	/products/:id	Get single product	No
   POST	/products	Create new product	Yes
   PUT	/products/:id	Update product	Yes
   DELETE	/products/:id	Delete product	Yes
   GET	/products/stats	Get product statistics	No
# Request Examples
GET /api/products?category=Electronics&page=1&limit=5
   Response : {
  "data": [
    {
      "id": "1",
      "name": "Laptop",
      "price": 999.99,
      "category": "Electronics",
      "inStock": true
    }
  ],
  "pagination": {
    "page": 1,
    "limit": 5,
    "total": 1,
    "totalPages": 1
  }
}
# Error response
   {
  "error": {
    "message": "Product not found",
    "statusCode": 404
  }
}
# This README includes:
1. Clear setup instructions
2. Complete API documentation
3. Request/response examples
4. Error handling details
