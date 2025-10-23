# 🛍 MERN E-Commerce API Documentation

## User API Endpoints

  Method   Endpoint             Description
  -------- -------------------- --------------------------------------------
  POST     /api/user/register   Register a new user
  POST     /api/user/login      Login existing user
  GET      /api/user/profile    Get User Profile (Authentication Required)
  GET      /api/user/all        Get All Users

------------------------------------------------------------------------

## Product API Endpoints

  Method   Endpoint           Description
  -------- ------------------ ------------------------------
  POST     /api/product/add   Create a new product
  GET      /api/product/all   Retrieve all products
  GET      /api/product/:id   Get a specific product by ID
  PUT      /api/product/:id   Update a product by ID
  DELETE   /api/product/:id   Delete a product by ID

------------------------------------------------------------------------

## Cart API Endpoints

  -----------------------------------------------------------------------
  Method            Endpoint                 Description
  ----------------- ------------------------ ----------------------------
  POST              /api/cart/add            Add a product to the cart
                                             (Authentication Required)

  GET               /api/cart/user           Retrieve the user-specific
                                             cart (Authentication
                                             Required)

  PUT               /api/cart/:id            Decrease the quantity of a
                                             product in the cart
                                             (Authentication Required)

  DELETE            /api/cart/remove/:id     Remove a product from the
                                             cart (Authentication
                                             Required)

  DELETE            /api/cart/clear          Delete all products from the
                                             cart (Authentication
                                             Required)
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## Shipping Address API Endpoints

  -----------------------------------------------------------------------
  Method            Endpoint                 Description
  ----------------- ------------------------ ----------------------------
  POST              /api/address/add         Add User Shipping Address
                                             (Authentication Required)

  GET               /api/address/get         Get User Shipping Address
                                             (Authentication Required)
  -----------------------------------------------------------------------

------------------------------------------------------------------------

## Payment API Endpoints

  ----------------------------------------------------------------------------
  Method            Endpoint                      Description
  ----------------- ----------------------------- ----------------------------
  POST              /api/payment/checkout         Initiates the payment
                                                  process

  POST              /api/payment/verify-payment   Confirms the payment & saves
                                                  to DB
  ----------------------------------------------------------------------------

------------------------------------------------------------------------

## Order Confirmation API Endpoints

  -----------------------------------------------------------------------
  Method            Endpoint                 Description
  ----------------- ------------------------ ----------------------------
  GET               /api/order/confirm       User-specific orders
                                             (Authentication Required)

  GET               /api/order/confirm/all   All users' orders
  -----------------------------------------------------------------------
