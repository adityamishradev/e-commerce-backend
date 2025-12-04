🚀 MERN E-Commerce API (with Razorpay Payment Integration)

A complete MERN Stack E-Commerce backend featuring authentication, product management, cart system, shipping address, Razorpay payment gateway, and order confirmation APIs.

🧑‍💻 User API Endpoints
POST /api/user/register

Register a new user.

POST /api/user/login

Login an existing user.

GET /api/user/profile

Get user profile.
(Authentication Required)

GET /api/user/all

Get all users.

🛒 Product API Endpoints
POST /api/product/add

Create a new product.

GET /api/product/all

Retrieve all products.

GET /api/product/id/:id

Get specific product by ID.

PUT /api/product/id/:id

Update product by ID.

DELETE /api/product/id/:id

Delete product by ID.

🛍️ Cart API Endpoints
POST /api/cart/add

Add a product to cart.
(Authentication Required)

GET /api/cart/user

Retrieve user-specific cart.
(Authentication Required)

PUT /api/cart/qty

Decrease product quantity in cart.
(Authentication Required)

DELETE /api/cart/remove/productId

Remove a product from cart.
(Authentication Required)

DELETE /api/cart/clear

Clear entire cart.
(Authentication Required)

📦 Shipping Address API Endpoints
POST /api/address/add

Add user shipping address.
(Authentication Required)

GET /api/address/get

Get user address.
(Authentication Required)

💳 Payment API Endpoints (Razorpay)
POST /api/payment/checkout

Initiates Razorpay payment and creates order.

POST /api/payment/verify-payment

Verifies Razorpay payment & saves order to DB.

📄 Order Confirmation API Endpoints
GET /api/order/confirm

Get logged-in user's orders.
(Authentication Required)

GET /api/order/confirm/all

Get all users’ orders (Admin).
