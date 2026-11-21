# Advanced Retail Super Shop

A **Spring Boot REST API** for managing a retail super shop including product management, customer management, and order processing with automatic stock control.

## 🚀 Features

* Product Management
* Customer Registration
* Order Processing
* Automatic Stock Reduction
* RESTful API Architecture

## 🏗 Architecture

Layered Spring Boot architecture:

Entity → Repository → Service → Controller

## 🛠 Tech Stack

* Java
* Spring Boot
* Spring Data JPA
* Lombok
* MySQL

## 📡 API Endpoints

| Method | Endpoint         | Description   |
| ------ | ---------------- | ------------- |
| POST   | `/shop/product`  | Add product   |
| POST   | `/shop/customer` | Add customer  |
| POST   | `/shop/order`    | Create order  |
| GET    | `/shop/products` | List products |
| GET    | `/shop/orders`   | List orders   |

## ▶ Run Project

1. Create the database:

   ```sql
   CREATE DATABASE supershop;
   ```

2. Set your MySQL credentials as environment variables (read by `application.yaml`):

   ```bash
   export DB_USERNAME=root
   export DB_PASSWORD=your_mysql_password
   ```

3. Start the app (needs Maven installed):

   ```bash
   cd advanced-retail-super-shop
   mvn spring-boot:run
   ```

The API runs at `http://localhost:8080`. Creating an order reduces the product's stock and fails if stock is too low.

## 📌 Author

Jisan – Data Science & Software Engineering Student
