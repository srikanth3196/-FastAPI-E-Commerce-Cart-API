# 🛒 FastAPI E-Commerce Cart API



A **FastAPI-based E-Commerce Backend API** that simulates a small online store system with **products, cart management, and order checkout**.

This project demonstrates **real backend development concepts** including:

* RESTful API design
* Cart system logic
* CRUD operations
* Request validation using Pydantic
* Inventory checks
* Checkout workflows
* Interactive API documentation with Swagger

---

# 🚀 Features

### 🏪 Product Management

* View all products
* Get product details by ID
* Add new products
* Update stock or price
* Delete products

### 🛒 Cart System

* Add products to cart
* Update quantity automatically
* Prevent adding out-of-stock items
* Remove items from cart
* View cart summary and totals

### 💳 Checkout System

* Convert cart items into orders
* Create separate orders per product
* Clear cart after checkout
* Validate empty cart checkout

### 📊 Inventory Utilities

* Filter products
* Compare products
* Inventory audit summary
* Bulk category discounts

---

# 📸 API Preview

### Swagger API Interface

Open Swagger after starting the server:

```id="readme001"
http://127.0.0.1:8000/docs
```

Example interface:

![Swagger UI](docs/swagger-ui.png)

---

# ⚙️ Tech Stack

| Technology | Purpose                 |
| ---------- | ----------------------- |
| Python     | Programming language    |
| FastAPI    | Backend API framework   |
| Pydantic   | Request validation      |
| Uvicorn    | ASGI server             |
| Swagger UI | Interactive API testing |

---

# 📦 Installation

### 1️⃣ Clone the repository

```bash id="readme002"
git clone https://github.com/your-username/fastapi-ecommerce-api.git
cd fastapi-ecommerce-api
```

---

### 2️⃣ Install dependencies

```bash id="readme003"
pip install fastapi uvicorn
```

---

### 3️⃣ Run the server

```bash id="readme004"
uvicorn main:app --reload
```

Server runs at:

```id="readme005"
http://127.0.0.1:8000
```

---

# 📚 API Endpoints

## 🏪 Products

| Method | Endpoint                 | Description        |
| ------ | ------------------------ | ------------------ |
| GET    | `/products`              | Get all products   |
| GET    | `/products/{product_id}` | Get a product      |
| POST   | `/products`              | Add new product    |
| PUT    | `/products/{product_id}` | Update price/stock |
| DELETE | `/products/{product_id}` | Delete product     |

---

## 🔍 Product Utilities

| Method | Endpoint             | Description          |
| ------ | -------------------- | -------------------- |
| GET    | `/products/filter`   | Filter products      |
| GET    | `/products/compare`  | Compare two products |
| GET    | `/products/audit`    | Inventory summary    |
| PUT    | `/products/discount` | Apply bulk discount  |

---

## 🛒 Cart System

| Method | Endpoint             | Description           |
| ------ | -------------------- | --------------------- |
| POST   | `/cart/add`          | Add product to cart   |
| GET    | `/cart`              | View cart             |
| DELETE | `/cart/{product_id}` | Remove item from cart |
| POST   | `/cart/checkout`     | Checkout cart         |

---

## 📦 Orders

| Method | Endpoint  | Description          |
| ------ | --------- | -------------------- |
| POST   | `/orders` | Place order directly |
| GET    | `/orders` | View all orders      |

---


# 🧠 Concepts Practiced

This project demonstrates key backend development skills:

* FastAPI routing
* REST API development
* Query parameters
* Business logic handling
* Cart system design
* Error handling with HTTPException
* Data validation with Pydantic
* API documentation






